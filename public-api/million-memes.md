---
description: Access the Million Token Memes collection.
---

# Million Memes

{% hint style="warning" %}
Features aren't implemented yet. Next release will come soon !
{% endhint %}

{% swagger baseUrl="https://api.milliontoken.cloud" path="/memes/random" method="get" summary="Get a Random Meme Image for Million Token" %}
{% swagger-description %}
Will send a different random meme picture on each request.
{% endswagger-description %}

{% swagger-parameter in="query" name="format" type="string" %}
Chose the format you want: png, jpeg, gif, mp4, webm
{% endswagger-parameter %}

{% swagger-parameter in="query" name="ratio" type="string" %}
Get a picture that have specific w/h ratio 

\


1-16, 3-4, 3-2, 1-1
{% endswagger-parameter %}

{% swagger-parameter in="query" name="width" type="integer" %}
Get a Picture that have this exact width, or nearest.
{% endswagger-parameter %}

{% swagger-parameter in="query" name="height" type="integer" %}
Get a Picture that have this exact height, or nearest.
{% endswagger-parameter %}

{% swagger-response status="200" description="" %}
```
```
{% endswagger-response %}
{% endswagger %}

{% swagger baseUrl="https://api.milliontoken.cloud" path="/memes" method="get" summary="Get the meme images List" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-parameter in="query" name="limit" type="string" %}
Limit the number of rows to get.

\


Default is 100.
{% endswagger-parameter %}

{% swagger-response status="200" description="" %}
```
```
{% endswagger-response %}
{% endswagger %}

{% swagger baseUrl="https://api.milliontoken.cloud" path="/memes/:id" method="get" summary="Get the meme image by ID" %}
{% swagger-description %}
Return the meme image by ID.
{% endswagger-description %}

{% swagger-parameter in="path" name="id" type="string" %}
Get the meme image by id.
{% endswagger-parameter %}

{% swagger-response status="200" description="" %}
```
```
{% endswagger-response %}
{% endswagger %}

{% swagger baseUrl="https://api.milliontoken.cloud" path="/memes/:slug" method="get" summary="Get the meme image by Slug" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-parameter in="path" name="slug" type="string" %}
Get the meme image by slug.
{% endswagger-parameter %}

{% swagger-response status="200" description="" %}
```
```
{% endswagger-response %}
{% endswagger %}
