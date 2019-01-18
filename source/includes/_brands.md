# Brands

A brand resource represents a franchise name.  This object contains a hiearchy of businesses.  For example if there is a McDonald's store in San Francisco and San Diego, the businesses would be the locations in San Francisco and San Diego and the brand would be McDonalds.

<code>
 &nbsp; &nbsp; -- McDonalds <i class="item-label">brand</i><br />
 &nbsp; &nbsp; &nbsp; |-- San Francisco McDonalds <i class="item-label">business</i><br />
 &nbsp; &nbsp; &nbsp; |-- San Deigo McDonalds <i class="item-label">business</i>
</code>


## Brand Object

Attribute |   | Description
--------- | - | -----------
id | <i class="item-label">integer</i> | Internal unique identifier for the object.
name | <i class="item-label">string</i> | Name of the brand.

## Retrieve A Brand List

> <b>GET /api/v1/brands</b>

> Example Request

 ```shell
# With shell, you can just pass the correct header with each request
curl "https://dev.qebot.com/api/v1/brands"
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
    "brands": [
        {...}
    ]
}
```

```php
{
    "brands": [
        {...}
    ]
}
```

```ruby
{
    "brands": [
        {...}
    ]
}
```

```python
{
    "brands": [
        {...}
    ]
}
```

```go
{
    "brands": [
        {...}
    ]
}
```

```javascript
{
    "brands": [
        {...}
    ]
}
```

<span title="get" class="pg-type type-get">get</span>

Retrieves a list of accessible brands.

### HTTP Request

`GET https://dev.qebot.com/api/v1/brands`

### Returns
 Returns an array of brands.

## Create Brand

> <b>POST /api/v1/brands</b>

> Example Request

 ```shell
# With shell, you can just pass the correct header with each request
curl "https://dev.qebot.com/api/v1/brands"
    -X POST
  -u "<API_TOKEN>"
  -d brand[name]="Brand Name"
  -d brand[status]=active
  -d businesses[][business_name]="Business Name"
  -d businesses[][category_id]=1
  -d businesses[][phone]=1234567890
  -d businesses[][fax]=1234567890
  -d businesses[][address]="123 fake st"
  -d businesses[][address2]="Suite #2"
  -d businesses[][city]="San Francisco"
  -d businesses[][state_id]=1
  -d businesses[][country_id]=1
  -d businesses[][zipcode]=12345
  -d businesses[][email]=user@example.com
  -d businesses[][website]="http://example.com"
  -d businesses[][status]=active
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
    "brands": [
        {...}
    ],
    "businesses":[
        {...}
    ]
}
```

```php
{
    "brands": [
        {...}
    ],
    "businesses":[
        {...}
    ]
}
```

```ruby
{
    "brands": [
        {...}
    ],
    "businesses":[
        {...}
    ]
}
```

```python
{
    "brands": [
        {...}
    ],
    "businesses":[
        {...}
    ]
}
```

```go
{
    "brands": [
        {...}
    ],
    "businesses":[
        {...}
    ]
}
```

```javascript
{
    "brands": [
        {...}
    ],
    "businesses":[
        {...}
    ]
}
```

<span title="post" class="pg-type type-post">post</span>

Create a new brand with corresponding businesses.

### HTTP Request

`POST https://dev.qebot.com/api/v1/brands`

<aside class="notice">
The dot notation indicates that the property is one level deep inside a hash.<br />
The `[]` indicates the property is an array of objects
</aside>

<aside class="notice">
Either state or state id should exist.
</aside>
<h5 class="sidebar-nav-heading">Request Arguments</h5>
Param |   | Description
----- | - | -----------
brand.name<br /><var>requried</var> | <i class="item-label">string</i> | Name of brand or franchise.
brand.status<br /><var>requried</var> | <i class="item-label">string</i> | Status of brand.<br />Possible values: (<b>active</b>, <b>inactive</b>)
businesses[]business | <i class="item-label">array</i> | A business hash with an array of Business objects.
 | business_name<br /><i class="item-label">string</i><br><var>required</var> | Name of the business.
 | category_id<br /><i class="item-label">integer</i> | Identifier for what category a business belongs to.  See [Category](#category-object) object
 | phone <br /><i class="item-label">string</i><var>required</var> | A phone contact number of the busieness.
 | fax <br /><i class="item-label">string</i> | A fax number for the busieness.
 | address <br /><i class="item-label">string</i><var>required</var> | Address of the business.
 | address2 <br /><i class="item-label">string</i> | Extra information for business address.
 | city <br /><i class="item-label">string</i><var>required</var> | City of the business.
 | state_id <br /><i class="item-label">integer</i> | Extra information State identifier for the business. See [State](#state-object) object
 | state_name <br /><i class="item-label">string</i> | Name of the state where address resides.
 | country_id <br /><i class="item-label">integer</i><var>required</var> | Country identifier for the business. See [Country](#country-object) object
 | zipcode <br /><i class="item-label">string</i><var>required</var> | Zipcode of the business.
 | email <br /><i class="item-label">string</i><var>required</var> | Contact email for the business.
 | website <br /><i class="item-label">string</i>| Website for the business.
 | status <br /><i class="item-label">string</i>| Status of the business.<br />Possible values: (<b>active</b>, <b>inactive</b>)

### Returns
 Returns a hash with keys brands with an array of a brand and businesses with an array of bussinesses.

## Retrieve Brand

> <b>GET /api/v1/brands/ <var>id</var></b>

> Example Request

 ```shell
# With shell, you can just pass the correct header with each request
curl "https://dev.qebot.com/api/v1/brands/<ID>"
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
    "brands": [
        {...}
    ]
}
```

```php
{
    "brands": [
        {...}
    ]
}
```

```ruby
{
    "brands": [
        {...}
    ]
}
```

```python
{
    "brands": [
        {...}
    ]
}
```

```go
{
    "brands": [
        {...}
    ]
}
```

```javascript
{
    "brands": [
        {...}
    ]
}
```

<span title="get" class="pg-type type-get">get</span>

Retrieves a brand from a previously created brand object.

To retrieve a brand object you must supply the uniqe identifier <var>id</var> to brand's resouce link
<i class="item-label">/api/v1/brands/ <var>id</var></i> 

### HTTP Request

`GET https://dev.qebot.com/api/v1/brands/<ID>`

### Returns
 Returns an array of a brand.

## Update Brand

> <b>PUT /api/v1/brands/ <var>id</var></b>

> <b>PATCH /api/v1/brands/ <var>id</var></b>

> Example Request

 ```shell
# Brand id needs to be appended after api uri
curl "https://dev.qebot.com/api/v1/brands/<ID>"
    -X PATCH
  -u "<API_TOKEN>"
  -d name="Brand Name"
  -d status=active
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
    "brands": [
        {...}
    ]
}
```

```php
{
    "brands": [
        {...}
    ]
}
```

```ruby
{
    "brands": [
        {...}
    ]
}
```

```python
{
    "brands": [
        {...}
    ]
}
```

```go
{
    "brands": [
        {...}
    ]
}
```

```javascript
{
    "brands": [
        {...}
    ]
}
```

<span title="put" class="pg-type type-put">post</span>
<span title="patch" class="pg-type type-patch">post</span>

Updates a brand object.

To update a brand object you must supply the uniqe identifier <var>id</var> to brand's resouce link
<i class="item-label">/api/v1/brands/ <var>id</var></i>

### HTTP Request

`PUT https://dev.qebot.com/api/v1/brands/<ID>`

`PATCH https://dev.qebot.com/api/v1/brands/<ID>`

<aside class="notice">
Even though all brand params are optional.  If an empty request is passed an error will be thrown.
</aside>

<h5 class="sidebar-nav-heading">Request Arguments</h5>
Param |   | Description
----- | - | -----------
name | <i class="item-label">string</i> | Name of brand or franchise.
status | <i class="item-label">string</i> | Status of brand.<br />Possible values: (<b>active</b>, <b>inactive</b>)


### Returns
 Returns an array of a brand.

## Delete Brand

> <b>DELETE /api/v1/brands/ <var>id</var></b>

> Example Request

 ```shell
# Brand id needs to be appended after api uri
curl "https://dev.qebot.com/api/v1/brands/<ID>"
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

Deletes a brand object.

To delete a brand object you must supply the uniqe identifier <var>id</var> to brand's resouce link
<i class="item-label">/api/v1/brands/ <var>id</var></i>

### HTTP Request

`DELETE https://dev.qebot.com/api/v1/brands/<ID>`

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

