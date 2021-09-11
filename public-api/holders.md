---
description: API Endpoints concerning the Million Token holders.
---

# Holders

{% hint style="warning" %}
Features aren't implemented yet. Next release will come soon !
{% endhint %}

{% api-method method="get" host="https://api.milliontoken.cloud" path="/v1/holders" %}
{% api-method-summary %}
Million Token Holders List
{% endapi-method-summary %}

{% api-method-description %}
Get the Holders JSON list.  
https://api.milliontoken.cloud/v1/holders?blockchain=eth
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-query-parameters %}
{% api-method-parameter name="limit" type="integer" required=false %}
Limit the number of rows.
{% endapi-method-parameter %}

{% api-method-parameter name="split" type="boolean" required=false %}
Split holders in sub arrays for each blockchains.  
Default is true.
{% endapi-method-parameter %}

{% api-method-parameter name="blockchain" type="string" required=false %}
Select holders of the specified blockchains only
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Cake successfully retrieved.
{% endapi-method-response-example-description %}

```
{
    "ethereum": [
        {
            "wallet": "0x0000000000000000000000000000000000000000",    
            "mm-balance": "123000000000000",    
            "mm-usd-value": "1452145200000000"
        },
        {
            "wallet": "0x0000000000000000000000000000000000000000",    
            "mm-balance": "123000000000000",    
            "mm-usd-value": "1452145200000000"
        }
    ]
}
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=404 %}
{% api-method-response-example-description %}
Could not find a cake matching this query.
{% endapi-method-response-example-description %}

```
{    "message": "There is no holders, or an error during the request"}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="https://api.milliontoken.cloud" path="/v1/holders/:address" %}
{% api-method-summary %}
Million Token Holder Details
{% endapi-method-summary %}

{% api-method-description %}
https://api.milliontoken.cloud/v1/holders/0x0000000000000000000000000000000000000000
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
{
    "wallet-address": "0x0000000000000000000000000000000000000000", 
    "mm-balance": 123000000000000,
    "mm-usd-value": 1452145200000000
}
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=404 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
{    "message": "The Wallet Address don't hold any MM Token"}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



