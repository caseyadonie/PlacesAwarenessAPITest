---
description: 'Entry Point: http://184.107.228.154/PayEaziConnect/b1/'
---

# User Details

{% api-method method="post" host="EndPoint" path="/users/UpdateCredetialsUser" %}
{% api-method-summary %}
 UpdateCredetialsUser
{% endapi-method-summary %}

{% api-method-description %}
This endpoint allows you to get free cakes.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-body-parameters %}
{% api-method-parameter name="Email" type="string" required=false %}

{% endapi-method-parameter %}

{% api-method-parameter name="IsForceUpdate" type="boolean" required=false %}

{% endapi-method-parameter %}

{% api-method-parameter name="Surname" type="string" required=true %}

{% endapi-method-parameter %}

{% api-method-parameter name="OtherNames" type="string" required=true %}

{% endapi-method-parameter %}

{% api-method-parameter name="Passcode" type="string" required=true %}

{% endapi-method-parameter %}

{% api-method-parameter name="MobileNo" type="string" required=true %}

{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Cake successfully retrieved.
{% endapi-method-response-example-description %}

```javascript
{
    "name": "Cake's name",
    "recipe": "Cake's recipe name",
    "cake": "Binary cake"
}
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=404 %}
{% api-method-response-example-description %}
Could not find a cake matching this query.
{% endapi-method-response-example-description %}

```javascript
{
    "message": "Ain't no cake like that."
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



