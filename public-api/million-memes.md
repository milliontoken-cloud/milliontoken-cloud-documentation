---
description: Access the Million Token Memes collection.
---

# Million Memes

{% hint style="warning" %}
Features aren't implemented yet. Next release will come soon !
{% endhint %}

{% api-method method="get" host="https://api.milliontoken.cloud" path="/memes/random" %}
{% api-method-summary %}
Get a Random Meme Image for Million Token
{% endapi-method-summary %}

{% api-method-description %}
Will send a different random meme picture on each request.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-query-parameters %}
{% api-method-parameter name="format" type="string" required=false %}
Chose the format you want: png, jpeg, gif, mp4, webm
{% endapi-method-parameter %}

{% api-method-parameter name="ratio" type="string" required=false %}
Get a picture that have specific w/h ratio   
1-16, 3-4, 3-2, 1-1
{% endapi-method-parameter %}

{% api-method-parameter name="width" type="integer" required=false %}
Get a Picture that have this exact width, or nearest.
{% endapi-method-parameter %}

{% api-method-parameter name="height" type="integer" required=false %}
Get a Picture that have this exact height, or nearest.
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

{% api-method method="get" host="https://api.milliontoken.cloud" path="/memes" %}
{% api-method-summary %}
Get the meme images List
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-query-parameters %}
{% api-method-parameter name="limit" type="string" required=false %}
Limit the number of rows to get.  
Default is 100.
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

{% api-method method="get" host="https://api.milliontoken.cloud" path="/memes/:id" %}
{% api-method-summary %}
Get the meme image by ID
{% endapi-method-summary %}

{% api-method-description %}
Return the meme image by ID.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="id" type="string" required=false %}
Get the meme image by id.
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

{% api-method method="get" host="https://api.milliontoken.cloud" path="/memes/:name\_slug" %}
{% api-method-summary %}
Get the meme image by Slug Name
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="name\_slug" type="string" required=false %}
Get the meme image by slug name.
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

