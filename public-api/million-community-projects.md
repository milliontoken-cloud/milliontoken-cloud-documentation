---
description: Access data about the community Projects.
---

# Million Community Projects

{% hint style="warning" %}
Features aren't implemented yet. Next release will come soon !
{% endhint %}

{% api-method method="get" host="https://api.milliontoken.cloud" path="/community-projects" %}
{% api-method-summary %}
Community projects List
{% endapi-method-summary %}

{% api-method-description %}
List all the community projects referenced by MillionTokenCloud.  
Want to add your project to the list ? A form will be made.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-query-parameters %}
{% api-method-parameter name="tags\_but" type="array" required=false %}
List projects that don't have this tags.
{% endapi-method-parameter %}

{% api-method-parameter name="tags" type="array" %}
Used to filter projects by tags.
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Cake successfully retrieved.
{% endapi-method-response-example-description %}

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
{% endapi-method-response-example %}

{% api-method-response-example httpCode=404 %}
{% api-method-response-example-description %}
Could not find a cake matching this query.
{% endapi-method-response-example-description %}

```
{ "message": "No community projects found." }
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="https://api.milliontoken.cloud" path="/community-projects/:id" %}
{% api-method-summary %}
Community project by ID
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="id" type="string" required=false %}
Get a community project by ID.
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

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
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="https://api.milliontoken.cloud" path="/community-projects/:slug" %}
{% api-method-summary %}
Community project by Slug
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="slug" type="string" required=false %}
Get a community project by slug.
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

{% api-method method="get" host="https://api.milliontoken.cloud" path="/community-projects/:id" %}
{% api-method-summary %}

{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="id" type="string" required=false %}
Get a community project by ID.
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

