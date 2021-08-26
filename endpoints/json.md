---
description: Endpoints with a JSON response.
---

# JSON

{% api-method method="get" host="https://api.willz.repl.co" path="/videos/spanish" %}
{% api-method-summary %}
Videos Spanish
{% endapi-method-summary %}

{% api-method-description %}
Return a spanish video URL.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="key" type="string" required=true %}
Your API token access.
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Video
{% endapi-method-response-example-description %}

```
{
"url":"link.mp4"
}
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=404 %}
{% api-method-response-example-description %}
Not found because not key given or invalid key.
{% endapi-method-response-example-description %}

```
{ 
"error": ""The key to the API access that you provided is invalid! Make sure you have written it correctly. Any issue? Join us: https://api.willz.repl.co""
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



