---
description: 'Entry Point: http://184.107.228.154/PayEaziConnect/b1/'
---

# PayEazi Web API

{% api-method method="post" host="End Point " path="sms/NewRegistrationSMS" %}
{% api-method-summary %}
Registration Step 1
{% endapi-method-summary %}

{% api-method-description %}
This is Used to Check if Mobile No is already Registered and also triggers an OTP for registration
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-body-parameters %}
{% api-method-parameter name="keyword" type="string" required=false %}
Example PayEazi
{% endapi-method-parameter %}

{% api-method-parameter name="message" type="string" required=false %}
Leave blank
{% endapi-method-parameter %}

{% api-method-parameter name="to" type="string" required=true %}

{% endapi-method-parameter %}

{% api-method-parameter name="from" type="string" required=true %}

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
    "status": "Success"
}
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=404 %}
{% api-method-response-example-description %}
Could not find a cake matching this query.
{% endapi-method-response-example-description %}

```javascript
{
    "message": "Bad Request"
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



