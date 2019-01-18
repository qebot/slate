# Purchases

The purchases resource is the gateway to connect tools to businesses and users.  To charge a credit or a debit card, you [create a purchase](#create-a-purchase) object.

<aside class="notice">
Please take note that all purchases will create a subscription transaction.  The transaction will re-occur every month on the first.
</aside>

## Purchase Object

Attribute |   | Description
--------- | - | -----------
id | <i class="item-label">integer</i> | Internal unique identifier for the object.
payment_date | <i class="item-label">date</i> | The occurence of the charged subscription.
brand | <i class="item-label">Brand</i> | See [Brand](#brand-object) object
whitelabel | <i class="item-label">Whitelabel</i> | Whitelabel object
business | <i class="item-label">Business</i> | See [Business](#business-object) object
tool | <i class="item-label">Tool</i> | See [Tool](#tool-object) object
user | <i class="item-label">User</i> | See [User](#user-object) object

## Retrieve a Purchase List

> <b>GET /api/v1/purchases</b>

> Example Request

 ```shell
# With shell, you can just pass the correct header with each request
curl "https://dev.qebot.com/api/v1/purchases"
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
    "purchases": [
        {...},
        {...}
    ]
}
```

```php
{
    "purchases": [
        {...},
        {...}
    ]
}
```

```ruby
{
    "purchases": [
        {...},
        {...}
    ]
}
```

```python
{
    "purchases": [
        {...},
        {...}
    ]
}
```

```go
{
    "purchases": [
        {...},
        {...}
    ]
}
```

```javascript
{
    "purchases": [
        {...},
        {...}
    ]
}
```

<span title="get" class="pg-type type-get">get</span>

Retrieves a list of subscriptions purchases

### HTTP Request

`GET https://dev.qebot.com/api/v1/purchases`

### Returns
 Returns an array of purchases.

## Create a Purchase

> <b>POST /api/v1/purchases</b>

> Example Request

 ```shell
# With shell, you can just pass the correct header with each request
curl "https://dev.qebot.com/api/v1/purchases"
  -X POST
  -u "<API_TOKEN>"
  -d tool_id=1
  -d billing[id]=1
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
    "purchases": [
        {...}
    ]
}
```

```php
{
    "purchases": [
        {...}
    ]
}
```

```ruby
{
    "purchases": [
        {...}
    ]
}
```

```python
{
    "purchases": [
        {...}
    ]
}
```

```go
{
    "purchases": [
        {...}
    ]
}
```

```javascript
{
    "purchasess": [
        {...}
    ]
}
```

<span title="post" class="pg-type type-post">post</span>

Create a purchase object.

### HTTP Request

`POST https://dev.qebot.com/api/v1/purchases`

<aside class="notice">
If you supply a billing id there is no need to fill out the rest of the billing information.
Specifying a billing id is simply using a previously stored billing account.
</aside>

<aside class="notice">
The dot notation indicates that the property is one level deep inside a hash.
</aside>

<h5 class="sidebar-nav-heading">Request Arguments</h5>
Param |   | Description
----- | - | -----------
tool_id | <i class="item-label">string</i><var>required</var> | A unique identifier of the tool you want to purchase. See [Retrieve A Tool List](#retrieve-a-tool-list) to see tools available.
first_name | <i class="item-label">string</i><var>required</var> | First name of the user on this subscription account.
last_name | <i class="item-label">string</i><var>required</var> | Last name of the user on this subscription account.
billing.id | <i class="item-label">string</i> | Unique identifier of billing acconnt on file you want to reuse.
billing.card_number | <i class="item-label">string</i> | Credit card number, spaces and dashes are accepted. (<var>required</var> only if no billing id is specified).
billing.exipry_month | <i class="item-label">integer</i> | Expiration month of billing card on file. (<var>required</var> only if no billing id is specified).
billing.exipry_year | <i class="item-label">integer</i> | Expiration year of billing card on file. (<var>required</var> only if no billing id is specified).
billing.cvv | <i class="item-label">string</i> | Security code or CVV, 3-4 digits <b>STRONGLY RECOMMENDED</b>.
billing.address | <i class="item-label">string</i> | Address line 1 on billing info.
billing.address2 | <i class="item-label">string</i> | Address lin2 on billing info.
billing.city | <i class="item-label">string</i> | City of billing on file.
billing.state | <i class="item-label">string</i> | State of billing on file.
billing.zip | <i class="item-label">string</i> | Zip or postal of billing on file.
billing.country | <i class="item-label">string</i> | Country, [2-letter ISO](https://www.iso.org/iso-3166-country-codes.html) code of billing on file.

### Returns
 Returns an array of a billing info.

## Retrieve a Purchase

> <b>GET /api/v1/purchases/ <var>id</var></b>

> Example Request

 ```shell
# With shell, you can just pass the correct header with each request
curl "https://dev.qebot.com/api/v1/purchases/<ID>"
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
    "purchases": [
        {...}
    ]
}
```

```php
{
    "purchases": [
        {...}
    ]
}
```

```ruby
{
    "purchases": [
        {...}
    ]
}
```

```python
{
    "purchases": [
        {...}
    ]
}
```

```go
{
    "purchases": [
        {...}
    ]
}
```

```javascript
{
    "purchases": [
        {...}
    ]
}
```

<span title="get" class="pg-type type-get">get</span>

Retrieves a purchase from a previously created purchase object.

To retrieve a purchase object you must supply the uniqe identifier <var>id</var> to purchase's resouce link
<i class="item-label">/api/v1/purchases/ <var>id</var></i> 

### HTTP Request

`GET https://dev.qebot.com/api/v1/purchases/<ID>`

### Returns
 Returns an array of a purchase.