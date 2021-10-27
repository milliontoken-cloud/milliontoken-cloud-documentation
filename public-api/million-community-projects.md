---
description: Access data about the community Projects.
---

# Million Community Projects

{% hint style="warning" %}
Features aren't implemented yet. Next release will come soon !
{% endhint %}

{% swagger baseUrl="https://api.milliontoken.cloud" path="/community-projects" method="get" summary="Community projects List" %}
{% swagger-description %}
List all the community projects referenced by MillionTokenCloud.

\


Want to add your project to the list ? A form will be made.
{% endswagger-description %}

{% swagger-parameter in="query" name="tags_but" type="array" %}
List projects that don't have this tags.
{% endswagger-parameter %}

{% swagger-parameter in="query" name="tags" type="array" %}
Used to filter projects by tags.
{% endswagger-parameter %}

{% swagger-response status="200" description="Cake successfully retrieved." %}
```
[{    
    "id": "x19y2ue2a0jc",
    "url": "https://milliontoken.cloud",
    "name": "milliontoken.cloud",
    "name_slug": "milliontoken-cloud",
    "description-short": "Provide resources and APIs endpoints for the MM Community.",
    "description": "Provide resources and APIs endpoints for the MM Community.",    
    "date_added_at": "2021-09-11",
    "date_edited_at": "2021-09-11",
    "tags": [
        "api",
        "data",
        "documentation"
    ],
    "social-links": {
        "twitter": "",
        "facebook": "",
        "reddit": "",
        "medium": "",
        "instagram": "",
        "pinterest": "",
        "discord": "",
        "telegram": "",
        "tumblr": ""
    }
}]
```
{% endswagger-response %}

{% swagger-response status="404" description="Could not find a cake matching this query." %}
```
{ "message": "No community projects found." }
```
{% endswagger-response %}
{% endswagger %}

{% swagger baseUrl="https://api.milliontoken.cloud" path="/community-projects/:id" method="get" summary="Community project by ID" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-parameter in="path" name="id" type="string" %}
Get a community project by ID.
{% endswagger-parameter %}

{% swagger-response status="200" description="" %}
```
{    
    "id": "x19y2ue2a0jc",
    "url": "https://milliontoken.cloud",
    "name": "milliontoken.cloud",
    "name_slug": "milliontoken-cloud",
    "description-short": "Provide resources and APIs endpoints for the MM Community.",
    "description": "Provide resources and APIs endpoints for the MM Community.",    
    "date_added_at": "2021-09-11",
    "date_edited_at": "2021-09-11",
    "tags": [
        "api",
        "data",
        "documentation"
    ],
    "social-links": {
        "twitter": "",
        "facebook": "",
        "reddit": "",
        "medium": "",
        "instagram": "",
        "pinterest": "",
        "discord": "",
        "telegram": "",
        "tumblr": ""
    }
}
```
{% endswagger-response %}
{% endswagger %}

{% swagger baseUrl="https://api.milliontoken.cloud" path="/community-projects/:slug" method="get" summary="Community project by Slug" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-parameter in="path" name="slug" type="string" %}
Get a community project by slug.
{% endswagger-parameter %}

{% swagger-response status="200" description="" %}
```
```
{% endswagger-response %}
{% endswagger %}

{% swagger baseUrl="https://api.milliontoken.cloud" path="/community-projects/:id" method="get" summary="" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-parameter in="path" name="id" type="string" %}
Get a community project by ID.
{% endswagger-parameter %}

{% swagger-response status="200" description="" %}
```
```
{% endswagger-response %}
{% endswagger %}
