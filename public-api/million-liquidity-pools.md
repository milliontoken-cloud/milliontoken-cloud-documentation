---
description: Access the Million Token Liquidity Data for each blockchain.
---

# Million Liquidity Pools

{% hint style="warning" %}
Features aren't implemented yet. Next release will come soon !
{% endhint %}

{% api-method method="get" host="https://api.milliontoken.cloud" path="/liquidity" %}
{% api-method-summary %}
Total Liquidity amounts per blockchain
{% endapi-method-summary %}

{% api-method-description %}
https://api.milliontoken.cloud/liquidity?blockchain=eth
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-query-parameters %}
{% api-method-parameter name="blockchain" type="string" required=false %}
Get the MM liquidity for the specified blockchain  
parameter's list: eth, ether, ethereum, sol, solana, matic, polygon, ada, cardano.
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
{
    "solana": {
        "total-usd-value": 890343, 
        "total-mm-stored": 27000,
        "total-mm-value": 445223
    }
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="https://api.milliontoken.cloud" path="/liquidity-pairs" %}
{% api-method-summary %}
Liquidity Pairs per blockchain
{% endapi-method-summary %}

{% api-method-description %}
https://api.milliontoken.cloud/liquidity-pairs?blockchain=eth,matic
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="blockchain" type="string" required=false %}
Get the MM liquidity pairs for the specified blockchain
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
{
    "ethereum": [
        "MM-USDC",
        "MM-ETH",
        "MM-BUSD",
        "MM-USDT"
    ],
    "polygon": [
        "MM-USDC",
        "MM-ETH"
    ]
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

