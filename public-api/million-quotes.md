---
description: Access the Million Token Quotes.
---

# Million Quotes

{% hint style="warning" %}
Features aren't implemented yet. Next release will come soon !
{% endhint %}

{% swagger baseUrl="https://api.milliontoken.cloud" path="/quotes/random" method="get" summary="Get a Random quote for Million Token" %}
{% swagger-description %}
This endpoint allows you to get free cakes.
{% endswagger-description %}

{% swagger-parameter in="query" name="all" type="boolean" %}
Get all the quotes data columns.

\


Default is false.
{% endswagger-parameter %}

{% swagger-response status="200" description="Cake successfully retrieved." %}
```
{   
    "id": "iu29UEoeu2e3",
    "slug": "million-to-the-moon",
    "quote": "Million to the moon !",
    "webUrl": "https://milliontoken.cloud/quotes/million-to-the-moon",
    "apiUrl": "https://milliontoken.cloud/quotes/million-to-the-moon"
}
```
{% endswagger-response %}

{% swagger-response status="404" description="Could not find a cake matching this query." %}
```
{
    "message": "Ain't no quotes here !" 
}
```
{% endswagger-response %}
{% endswagger %}

{% swagger baseUrl="https://api.milliontoken.cloud" path="/quotes/:slug" method="get" summary="Get a Quote by Slug" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-parameter in="path" name="slug" type="string" %}
Get a Quote by slug
{% endswagger-parameter %}

{% swagger-response status="200" description="" %}
```
```
{% endswagger-response %}
{% endswagger %}

{% swagger baseUrl="https://api.milliontoken.cloud" path="/quotes/:id" method="get" summary="Get a Quote by ID" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-parameter in="path" name="" type="string" %}
Get a Quote by ID
{% endswagger-parameter %}

{% swagger-response status="200" description="" %}
```
```
{% endswagger-response %}
{% endswagger %}

{% swagger baseUrl="https://api.milliontoken.cloud" path="/quotes" method="get" summary="Get Quotes List" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-parameter in="query" name="sort_by" type="string" %}
text, length, author, created_at, source
{% endswagger-parameter %}

{% swagger-parameter in="query" name="order" type="string" %}
asc or desc
{% endswagger-parameter %}

{% swagger-parameter in="query" name="limit" type="string" %}
Set the number of requested Quotes.

\


Default is 20.
{% endswagger-parameter %}

{% swagger-response status="200" description="" %}
```
```
{% endswagger-response %}
{% endswagger %}

{% swagger baseUrl="https://api.milliontoken.cloud" path="/quotes/authors" method="get" summary="Get the quotes authors List" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-response status="200" description="" %}
```
```
{% endswagger-response %}
{% endswagger %}

{% swagger baseUrl="https://api.milliontoken.cloud" path="/quotes/sources" method="get" summary="Get the quotes sources List" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-response status="200" description="" %}
```
```
{% endswagger-response %}
{% endswagger %}
