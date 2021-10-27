---
description: Access the Million Token Liquidity Data for each blockchain.
---

# Million Liquidity Pools

{% hint style="warning" %}
Features aren't implemented yet. Next release will come soon !
{% endhint %}

{% swagger baseUrl="https://api.milliontoken.cloud" path="/liquidity" method="get" summary="Total Liquidity amounts per blockchain" %}
{% swagger-description %}
https://api.milliontoken.cloud/liquidity?blockchain=eth
{% endswagger-description %}

{% swagger-parameter in="query" name="blockchain" type="string" %}
Get the MM liquidity for the specified blockchain

\


parameter's list: eth, ether, ethereum, sol, solana, matic, polygon, ada, cardano.
{% endswagger-parameter %}

{% swagger-response status="200" description="" %}
```
{
    "solana": {
        "total-usd-value": 890343, 
        "total-mm-stored": 27000,
        "total-mm-value": 445223
    }
}
```
{% endswagger-response %}
{% endswagger %}

{% swagger baseUrl="https://api.milliontoken.cloud" path="/liquidity-pairs" method="get" summary="Liquidity Pairs per blockchain" %}
{% swagger-description %}
https://api.milliontoken.cloud/liquidity-pairs?blockchain=eth,matic
{% endswagger-description %}

{% swagger-parameter in="path" name="blockchain" type="string" %}
Get the MM liquidity pairs for the specified blockchain
{% endswagger-parameter %}

{% swagger-response status="200" description="" %}
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
{% endswagger-response %}
{% endswagger %}
