# Billings

The Billings resource is responsible for creating billing information for purchases.  Currently we support billing information for credit card purchases.
This resource is also responsible for storing cards on file to ease the redundancy of re-entering business information for each purchase. 


## Billing Object

Attribute |   | Description
--------- | - | -----------
id | <i class="item-label">integer</i> | Internal unique identifier for the object.
first_name | <i class="item-label">string</i> | First name of the user on billing info.
last_name | <i class="item-label">string</i> | Last name of the user on billing info.
company | <i class="item-label">string</i> | Name of company on billing info.
address | <i class="item-label">string</i> | Address line 1 on billing info.
address2 | <i class="item-label">string</i> | Address lin2 on billing info.
city | <i class="item-label">string</i> | City of billing on file.
state | <i class="item-label">string</i> | State of billing on file.
zip | <i class="item-label">string</i> | Zip or postal of billing on file.
country | <i class="item-label">string</i> | Country, [2-letter ISO](https://www.iso.org/iso-3166-country-codes.html) code of billing on file.
card_type | <i class="item-label">string</i> | Type of card on billing info. Possible values: (<b>Visa</b>, <b>MasterCard</b>, <b>American Express</b>, <b>Discover</b>, <b>JCB</b>, <b>etc</b>)
zip | <i class="item-label">string</i> | Zip or postal of billing on file.
expiry_month | <i class="item-label">integer</i> | Expiration month of billing card on file.
expiry_year | <i class="item-label">integer</i> | Expiration year of billing card on file.
first_six | <i class="item-label">integer</i> | First six digits of billing card on file.
last_four | <i class="item-label">integer</i> | Last four digits of billing card on file.
vat_number | <i class="item-label">string</i> | Customer's VAT number.
ip_address | <i class="item-label">string</i> | Customer's IPv4 address when updating their billing information <b>STRONGLY RECOMMENDED</b>
ip_address_country | <i class="item-label">string</i> | 2-letter Country of IP Address of billing info.
<!--
"amazon_billing_agreement_id": null,
"Amazon Billing Agreement ID": null,
"braintree_payment_nonce": null,
"paypal_billing_agreement_id": null,
"roku_billing_agreement_id": null,
"name_on_account": null,
"routing_number": null,
"account_number": null,
"account_type": null>
-->

## Retrieve A Billings List

> <b>GET /api/v1/billings</b>

> Example Request

 ```shell
# With shell, you can just pass the correct header with each request
curl "https://dev.qebot.com/api/v1/billings"
  -u "<API_TOKEN>"
```

 ```php
 ```

```ruby
```

```python
```

```go
```

```javascript
```

> Example Response

```shell
{
    "billings": [
        {...},
        {...}
    ]
}
```

```php
{
    "billings": [
        {...},
        {...}
    ]
}
```

```ruby
{
    "billings": [
        {...},
        {...}
    ]
}
```

```python
{
    "billings": [
        {...},
        {...}
    ]
}
```

```go
{
    "billings": [
        {...},
        {...}
    ]
}
```

```javascript
{
    "billings": [
        {...},
        {...}
    ]
}
```

<span title="get" class="pg-type type-get">get</span>

Retrieves a list of billing info.

### HTTP Request

`GET https://dev.qebot.com/api/v1/billings`

### Returns
 Returns an array of billing info.

## Create Billings

> <b>POST /api/v1/billings</b>

> Example Request

 ```shell
# With shell, you can just pass the correct header with each request
curl "https://dev.qebot.com/api/v1/billings"
  -X POST
  -u "<API_TOKEN>"
  -d number=123456789012
  -d address1="123 fake st"
  -d address2="Suite 2"
  -d city="San Francisco"
  -d state=CA
```

 ```php
 ```

```ruby
```

```python
```

```go
```

```javascript
```

> Example Response

```shell
{
    "billings": [
        {...}
    ]
}
```

```php
{
    "billings": [
        {...}
    ]
}
```

```ruby
{
    "billings": [
        {...}
    ]
}
```

```python
{
    "billings": [
        {...}
    ]
}
```

```go
{
    "billings": [
        {...}
    ]
}
```

```javascript
{
    "billings": [
        {...}
    ]
}
```

<span title="post" class="pg-type type-post">post</span>

Create a billing object.

### HTTP Request

`POST https://dev.qebot.com/api/v1/billings`

<h5 class="sidebar-nav-heading">Request Arguments</h5>
Param |   | Description
----- | - | -----------
first_name | <i class="item-label">string</i><var>required</var> | First name of the user on billing info.
last_name | <i class="item-label">string</i><var>required</var> | Last name of the user on billing info.
card_number | <i class="item-label">string</i><var>required</var> | Credit card number, spaces and dashes are accepted.
company | <i class="item-label">string</i> | Name of company on billing info.
address | <i class="item-label">string</i> | Address line 1 on billing info.
address2 | <i class="item-label">string</i> | Address lin2 on billing info.
city | <i class="item-label">string</i> | City of billing on file.
state | <i class="item-label">string</i> | State of billing on file.
zip | <i class="item-label">string</i> | Zip or postal of billing on file.
country | <i class="item-label">string</i> | Country, [2-letter ISO](https://www.iso.org/iso-3166-country-codes.html) code of billing on file.
card_type | <i class="item-label">string</i> | Type of card on billing info. Possible values: (<b>Visa</b>, <b>MasterCard</b>, <b>American Express</b>, <b>Discover</b>, <b>JCB</b>, <b>etc</b>)
zip | <i class="item-label">string</i> | Zip or postal of billing on file.
phone | <i class="item-label">string</i> | Phone number, this field can be 10 digits.
expiry_month | <i class="item-label">integer</i><var>required</var> | Expiration month of billing card on file.
expiry_year | <i class="item-label">integer</i><var>required</var> | Expiration year of billing card on file.
first_six | <i class="item-label">integer</i> | First six digits of billing card on file.
last_four | <i class="item-label">integer</i> | Last four digits of billing card on file.
vat_number | <i class="item-label">string</i> | Customer's VAT number.
currency |	<i class="item-label">string</i> | Currency in which invoices will be posted. Only applicable if this account is enrolled in a plan has a different currency than your site's default.
cvv | <i class="item-label">string</i> | Security code or CVV, 3-4 digits <b>STRONGLY RECOMMENDED</b>.
ip_address | <i class="item-label">string</i> | Customer's IPv4 address when updating their billing information <b>STRONGLY RECOMMENDED</b>

### Returns
 Returns an array of a billing info.

## Retrieve Billing

> <b>GET /api/v1/billings/ <var>id</var></b>

> Example Request

 ```shell
# With shell, you can just pass the correct header with each request
curl "https://dev.qebot.com/api/v1/billings/<ID>"
  -u "<API_TOKEN>"
```

 ```php
 ```

```ruby
```

```python
```

```go
```

```javascript
```

> Example Response

```shell
{
    "billings": [
        {...}
    ]
}
```

```php
{
    "billings": [
        {...}
    ]
}
```

```ruby
{
    "billings": [
        {...}
    ]
}
```

```python
{
    "billings": [
        {...}
    ]
}
```

```go
{
    "billings": [
        {...}
    ]
}
```

```javascript
{
    "billings": [
        {...}
    ]
}
```

<span title="get" class="pg-type type-get">get</span>

Retrieves a billing from a previously created billing object.

To retrieve a billing object you must supply the uniqe identifier <var>id</var> to billing's resouce link
<i class="item-label">/api/v1/billings/ <var>id</var></i> 

### HTTP Request

`GET https://dev.qebot.com/api/v1/billings/<ID>`

### Returns
 Returns an array of a billing.

## Update Billing

> <b>PUT /api/v1/billings/ <var>id</var></b>

> <b>PATCH /api/v1/billings/ <var>id</var></b>

> Example Request

 ```shell
# User id needs to be appended after api uri
curl "https://dev.qebot.com/api/v1/billings/<ID>"
  -X PATCH
  -u "<API_TOKEN>"
  -d first_name=John
  -d last_name=Doe
  -d role_id=2
```

 ```php
 ```

```ruby
```

```python
```

```go
```

```javascript
```

> Example Response

```shell
{
    "billings": [
        {...}
    ]
}
```

```php
{
    "billings": [
        {...}
    ]
}
```

```ruby
{
    "billings": [
        {...}
    ]
}
```

```python
{
    "billings": [
        {...}
    ]
}
```

```go
{
    "billings": [
        {...}
    ]
}
```

```javascript
{
    "billings": [
        {...}
    ]
}
```

<span title="put" class="pg-type type-put">post</span>
<span title="patch" class="pg-type type-patch">post</span>

Updates a billing object.

To update a billing object you must supply the uniqe identifier <var>id</var> to billing's resouce link
<i class="item-label">/api/v1/billings/ <var>id</var></i>

### HTTP Request

`PUT https://dev.qebot.com/api/v1/billings/<ID>`

`PATCH https://dev.qebot.com/api/v1/billings/<ID>`

<aside class="notice">
Even though all billing params are optional.  If an empty request is passed an error will be thrown.
</aside>

<h5 class="sidebar-nav-heading">Request Arguments</h5>
Param |   | Description
----- | - | -----------
first_name | <i class="item-label">string</i> | First name of the user on billing info.
last_name | <i class="item-label">string</i> | Last name of the user on billing info.
card_number | <i class="item-label">string</i> | Credit card number, spaces and dashes are accepted.
company | <i class="item-label">string</i> | Name of company on billing info.
address | <i class="item-label">string</i> | Address line 1 on billing info.
address2 | <i class="item-label">string</i> | Address lin2 on billing info.
city | <i class="item-label">string</i> | City of billing on file.
state | <i class="item-label">string</i> | State of billing on file.
zip | <i class="item-label">string</i> | Zip or postal of billing on file.
country | <i class="item-label">string</i> | Country, [2-letter ISO](https://www.iso.org/iso-3166-country-codes.html) code of billing on file.
card_type | <i class="item-label">string</i> | Type of card on billing info. Possible values: (<b>Visa</b>, <b>MasterCard</b>, <b>American Express</b>, <b>Discover</b>, <b>JCB</b>, <b>etc</b>)
zip | <i class="item-label">string</i> | Zip or postal of billing on file.
phone | <i class="item-label">string</i> | Phone number, this field can be 10 digits.
expiry_month | <i class="item-label">integer</i> | Expiration month of billing card on file.
expiry_year | <i class="item-label">integer</i> | Expiration year of billing card on file.
first_six | <i class="item-label">integer</i> | First six digits of billing card on file.
last_four | <i class="item-label">integer</i> | Last four digits of billing card on file.
vat_number | <i class="item-label">string</i> | Customer's VAT number.
currency |	<i class="item-label">string</i> | Currency in which invoices will be posted. Only applicable if this account is enrolled in a plan has a different currency than your site's default.
cvv | <i class="item-label">string</i> | Security code or CVV, 3-4 digits <b>STRONGLY RECOMMENDED</b>.
ip_address | <i class="item-label">string</i> | Customer's IPv4 address when updating their billing information <b>STRONGLY RECOMMENDED</b>

### Returns
 Returns an array of a billing info.

## Delete Billing

> <b>DELETE /api/v1/billings/ <var>id</var></b>

> Example Request

 ```shell
# User id needs to be appended after api uri
curl "https://dev.qebot.com/api/v1/billings/<ID>"
    -X PATCH
  -u "<API_TOKEN>"
```

 ```php
 ```

```ruby
```

```python
```

```go
```

```javascript
```

> Example Response

```shell
```

 ```php
 ```

```ruby
```

```python
```

```go
```

```javascript
```

<span title="delete" class="pg-type type-delete">delete</span>

Deletes a billings object.

To delete a billing object you must supply the uniqe identifier <var>id</var> to billing's resouce link
<i class="item-label">/api/v1/billings/ <var>id</var></i>

### HTTP Request

`DELETE https://dev.qebot.com/api/v1/billings/<ID>`

<aside class="notice">
When a success is rendered there will be an empty response body.  You must examine status code in header to determine validity of the request.
</aside>



### Returns
 Returns an empty response.
<aside class="success">
Status code 204 is a successful response.
</aside>

<aside class="warning">
A status code of 4XX or 5XX is an unsuccesful response.
</aside>

