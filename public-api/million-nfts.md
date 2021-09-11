---
description: Getting Million Token related NFTs Information's.
---

# Million NFTs

Use the API to know if the current wallet address own an NFTs on the blockchain.

{% hint style="warning" %}
Features aren't implemented yet. Next release will come soon !
{% endhint %}

{% api-method method="get" host="https://api.million.cloud" path="/v1/million-nfts" %}
{% api-method-summary %}
Million NFTs References
{% endapi-method-summary %}

{% api-method-description %}
Get all the referenced NFTs per artist for Million Token.  
A local database reference all the actual NFTs creators for Million Token.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="artist" type="string" required=false %}
Get the NFTs references only for a specified artist.
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="https://api.milliontoken.cloud" path="/v1/million-nfts/artists" %}
{% api-method-summary %}
Million NFTs Artists
{% endapi-method-summary %}

{% api-method-description %}
Get all the million NFTs artists information.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-query-parameters %}
{% api-method-parameter name="tags" type="string" required=false %}
Filters the artists list by Tags
{% endapi-method-parameter %}

{% api-method-parameter name="artist" type="string" required=false %}
Get the specified NFT Artist information.
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

