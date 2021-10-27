---
description: Access the Million Token related NFTs data.
---

# Million NFTs

{% hint style="warning" %}
Features aren't implemented yet. Next release will come soon !
{% endhint %}

{% swagger baseUrl="https://api.milliontoken.cloud" path="/million-nfts" method="get" summary="Get Million NFTs References" %}
{% swagger-description %}
Get all the referenced NFTs per artist for Million Token.

\


A local database reference all the actual NFTs creators for Million Token.
{% endswagger-description %}

{% swagger-parameter in="path" name="artist" type="string" %}
Get the NFTs references only for a specified artist.
{% endswagger-parameter %}

{% swagger-response status="200" description="" %}
```
```
{% endswagger-response %}
{% endswagger %}

{% swagger baseUrl="https://api.milliontoken.cloud" path="/million-nfts/artists" method="get" summary="Get Million NFTs Artists" %}
{% swagger-description %}
Get all the million NFTs artists information.
{% endswagger-description %}

{% swagger-parameter in="query" name="tags" type="string" %}
Filters the artists list by Tags
{% endswagger-parameter %}

{% swagger-parameter in="query" name="artist" type="string" %}
Get the specified NFT Artist information.
{% endswagger-parameter %}

{% swagger-response status="200" description="" %}
```
```
{% endswagger-response %}
{% endswagger %}
