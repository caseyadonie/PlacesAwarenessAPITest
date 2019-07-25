---
description: 'Entry Point: http://184.107.228.154/PayEaziConnect/b1/'
---

# Registration OTP

{% api-method method="post" host="Endpoint " path="users/ValidateSMSCodeUser?isValidation=true" %}
{% api-method-summary %}
Validate OTP
{% endapi-method-summary %}

{% api-method-description %}
This endpoint allows you to get free cakes.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-query-parameters %}
{% api-method-parameter name="MobileNo" type="string" required=true %}
Mobile No of the User
{% endapi-method-parameter %}

{% api-method-parameter name="SMSVerificationCode" type="boolean" required=true %}
the OTP from User
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Cake successfully retrieved.
{% endapi-method-response-example-description %}

```javascript
{
    "PassCode": "null",
    "Surname": "null",
    "OtherNames": "null"
    ...
}
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=404 %}
{% api-method-response-example-description %}
Could not find a cake matching this query.
{% endapi-method-response-example-description %}

```javascript
{
    "message": "Expectation Failed"
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



