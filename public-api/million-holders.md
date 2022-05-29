---
description: Access the Million Token Holders Data.
---

# Million Holders

{% hint style="warning" %}
Features aren't implemented yet. Next release will come soon !
{% endhint %}

{% swagger baseUrl="https://api.millioncloud.org" path="/holders" method="get" summary="Million Token Holders List" %}
{% swagger-description %}
Get the Holders JSON list.

\


https://api.milliontoken.cloud/holders?blockchain=eth
{% endswagger-description %}

{% swagger-parameter in="query" name="limit" type="integer" %}
Limit the number of rows.
{% endswagger-parameter %}

{% swagger-parameter in="query" name="split" type="boolean" %}
Split holders in sub arrays for each blockchains.

\


Default is true.
{% endswagger-parameter %}

{% swagger-parameter in="query" name="blockchain" type="string" %}
Select holders of the specified blockchains only
{% endswagger-parameter %}

{% swagger-response status="200" description="Cake successfully retrieved." %}
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
{% endswagger-response %}

{% swagger-response status="404" description="Could not find a cake matching this query." %}
```
{    "message": "There is no holders, or an error during the request"}
```
{% endswagger-response %}
{% endswagger %}

{% swagger baseUrl="https://api.millioncloud.org" path="/holders/:address" method="get" summary="Million Token Holder Details" %}
{% swagger-description %}
https://api.milliontoken.cloud/holders/0x0000000000000000000000000000000000000000
{% endswagger-description %}

{% swagger-response status="200" description="" %}
```
{
    "address": "0x0000000000000000000000000000000000000000", 
    "mm_balance": 123000000000000,
    "mm_usd_value": 1452145200000000
}
```
{% endswagger-response %}

{% swagger-response status="404" description="" %}
```
{    "message": "The Wallet Address don't hold any MM Token"}
```
{% endswagger-response %}
{% endswagger %}

