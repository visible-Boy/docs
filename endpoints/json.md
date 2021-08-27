---
description: Endpoints with a JSON response.
---

# JSON

{% api-method method="get" host="https://api.willz.repl.co" path="/videos/spanish" %}
{% api-method-summary %}
Videos Spanish
{% endapi-method-summary %}

{% api-method-description %}
Returns a spanish video URL.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-query-parameters %}
{% api-method-parameter name="key" type="string" required=true %}
Your API token access.
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Video
{% endapi-method-response-example-description %}

```javascript
{
"url":"link.mp4"
}
```json
{% endapi-method-response-example %}

{% api-method-response-example httpCode=404 %}
{% api-method-response-example-description %}
Not found because not key given or invalid key.
{% endapi-method-response-example-description %}

```json
{ 
"error": ""The key to the API access that you provided is invalid! Make sure you have written it correctly. Any issue? Join us: https://api.willz.repl.co""
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="https://api.willz.repl.co" path="/memes-spanish" %}
{% api-method-summary %}
Memes Spanish
{% endapi-method-summary %}

{% api-method-description %}
Returns a spanish meme URL.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-query-parameters %}
{% api-method-parameter name="key" type="string" required=true %}
Your API token access.
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Meme
{% endapi-method-response-example-description %}

```javascript
{
"url":"link"
}
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=404 %}
{% api-method-response-example-description %}
Not found because not key given or invalid key.
{% endapi-method-response-example-description %}

```javascript
{ 
"error": ""The key to the API access that you provided is invalid! Make sure you have written it correctly. Any issue? Join us: https://api.willz.repl.co""
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="https://api.willz.repl.co" path="/image-search" %}
{% api-method-summary %}
Image Search
{% endapi-method-summary %}

{% api-method-description %}
Returns a URL of a image searched.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-query-parameters %}
{% api-method-parameter name="search" type="string" required=true %}
Query to search.
{% endapi-method-parameter %}

{% api-method-parameter name="key" type="string" required=true %}
Your API token access.
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Meme
{% endapi-method-response-example-description %}

```javascript
{
"image":"link"
}
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=404 %}
{% api-method-response-example-description %}
Not found because not key given or invalid key.
{% endapi-method-response-example-description %}

```javascript
{ 
"error": "The key to the API access that you provided is invalid! Make sure you have written it correctly. Any issue? Join us: https://api.willz.repl.co"
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

