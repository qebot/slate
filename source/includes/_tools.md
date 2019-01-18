# Tools

The tools are the life blood of the Qebot ecosystem.  This resource will show what tools you have at your disposal to purchase from our system.


## Tool Object

Attribute |   | Description
--------- | - | -----------
id | <i class="item-label">integer</i> | Internal unique identifier for the object.
tool | <i class="item-label">string</i> | The name of the tool
plan_code | <i class="item-label">string</i> | The code used for purchasing a tool.
amount | <i class="item-label">decimal</i> | The amount the tool costs.

## Retrieve A Tool List

> <b>GET /api/v1/tools</b>

> Example Request

 ```shell
# With shell, you can just pass the correct header with each request
curl "https://dev.qebot.com/api/v1/tools"
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
    "tools": [
        {
            "id": 1,
            "tool": "Qebot Tool",
            "plan_code": "qebot_tool",
            "amount": 20
        },
        {...}
    ]
}
```

```php
{
    "tools": [
        {
            "id": 1,
            "tool": "Qebot Tool",
            "plan_code": "qebot_tool",
            "amount": 20
        },
        {...}
    ]
}
```

```ruby
{
    "tools": [
        {
            "id": 1,
            "tool": "Qebot Tool",
            "plan_code": "qebot_tool",
            "amount": 20
        },
        {...}
    ]
}
```

```python
{
    "tools": [
        {
            "id": 1,
            "tool": "Qebot Tool",
            "plan_code": "qebot_tool",
            "amount": 20
        },
        {...}
    ]
}
```

```go
{
    "tools": [
        {
            "id": 1,
            "tool": "Qebot Tool",
            "plan_code": "qebot_tool",
            "amount": 20
        },
        {...}
    ]
}
```

```javascript
{
    "tools": [
        {
            "id": 1,
            "tool": "Qebot Tool",
            "plan_code": "qebot_tool",
            "amount": 20
        },
        {...}
    ]
}
```

<span title="get" class="pg-type type-get">get</span>

Retrieves a list of accessible tools.

### HTTP Request

`GET https://dev.qebot.com/api/v1/tools`

### Returns
 Returns an array of tools.


## Retrieve Tool

> <b>GET /api/v1/tools/ <var>id</var></b>

> Example Request

 ```shell
# With shell, you can just pass the correct header with each request
curl "https://dev.qebot.com/api/v1/tools/<ID>"
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
    "tools": [
        {
            "id": 1,
            "tool": "Qebot Tool",
            "plan_code": "qebot_tool",
            "amount": 20
        }
    ]
}
```

```php
{
    "tools": [
        {
            "id": 1,
            "tool": "Qebot Tool",
            "plan_code": "qebot_tool",
            "amount": 20
        }
    ]
}
```

```ruby
{
    "tools": [
        {
            "id": 1,
            "tool": "Qebot Tool",
            "plan_code": "qebot_tool",
            "amount": 20
        }
    ]
}
```

```python
{
    "tools": [
        {
            "id": 1,
            "tool": "Qebot Tool",
            "plan_code": "qebot_tool",
            "amount": 20
        }
    ]
}
```

```go
{
    "tools": [
        {
            "id": 1,
            "tool": "Qebot Tool",
            "plan_code": "qebot_tool",
            "amount": 20
        }
    ]
}
```

```javascript
{
    "tools": [
        {
            "id": 1,
            "tool": "Qebot Tool",
            "plan_code": "qebot_tool",
            "amount": 20
        }
    ]
}
```

<span title="get" class="pg-type type-get">get</span>

Retrieves a tool from a previously created tool object.

To retrieve a tool object you must supply the uniqe identifier <var>id</var> to tool's resouce link
<i class="item-label">/api/v1/tools/ <var>id</var></i> 

### HTTP Request

`GET https://dev.qebot.com/api/v1/tools/<ID>`

### Returns
 Returns an array of a tool.
 