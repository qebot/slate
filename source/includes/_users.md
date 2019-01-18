# Users

The User resource lets you retrieve information associated with a Qebot user, such as a person’s name, role, and status.


## User Object

Attribute |   | Description
--------- | - | -----------
id | <i class="item-label">integer</i> | Internal unique identifier for the object.
parent_id | <i class="item-label">integer</i> | Unique identifier for the parent of the user object.
first_name | <i class="item-label">string</i> | First name of the user.
last_name | <i class="item-label">string</i> | Last name of the user.
username | <i class="item-label">string</i> | Username, email of the user.
created_date | <i class="item-label">date</i> | The date of when user was created.
status | <i class="item-label">string</i> | The status of the user. Possible values: (<b>active</b>, <b>inactive</b>)
role | <i class="item-label">Role</i> | Role Object.

## Role Object

Attribute |   | Description
--------- | - | -----------
id | <i class="item-label">integer</i> | Internal unique identifier for the object.
name | <i class="item-label">integer</i> | Name of the role object.

### Possible Roles


<code>
  Roles<br />
&nbsp; <var><b>id</b> 1<br /><b>name</b> Super Admin</var><br /><br />
&nbsp; <var><b>id</b> 2<br /><b>name</b> Corporate Admin</var><br /><br />
&nbsp; <var><b>id</b> 3<br /><b>name</b> Business Admin</var><br /><br />
&nbsp; <var><b>id</b> 4<br /><b>name</b> User</var><br />
</code>

## Retrieve A User List

> <b>GET /api/v1/users</b>

> Example Request

 ```shell
# With shell, you can just pass the correct header with each request
curl "https://dev.qebot.com/api/v1/users"
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
    "users": [
        {
            "id": 1,
            "parent_id": 1,
            "first_name": "John",
            "last_name": "Doe",
            "username": "user@example.com",
            "created_date": "2016-10-06T13:28:27+00:00",
            "status": "active",
            "role": {
                "id": 2,
                "name": "Corporate Admin",
            }
        },
        {...}
    ]
}
```

```php
{
    "users": [
        {
            "id": 1,
            "parent_id": 1,
            "first_name": "John",
            "last_name": "Doe",
            "username": "user@example.com",
            "created_date": "2016-10-06T13:28:27+00:00",
            "status": "active",
            "role": {
                "id": 2,
                "name": "Corporate Admin",
            }
        },
        {...}
    ]
}
```

```ruby
{
    "users": [
        {
            "id": 1,
            "parent_id": 1,
            "first_name": "John",
            "last_name": "Doe",
            "username": "user@example.com",
            "created_date": "2016-10-06T13:28:27+00:00",
            "status": "active",
            "role": {
                "id": 2,
                "name": "Corporate Admin",
            }
        },
        {...}
    ]
}
```

```python
{
    "users": [
        {
            "id": 1,
            "parent_id": 1,
            "first_name": "John",
            "last_name": "Doe",
            "username": "user@example.com",
            "created_date": "2016-10-06T13:28:27+00:00",
            "status": "active",
            "role": {
                "id": 2,
                "name": "Corporate Admin",
            }
        },
        {...}
    ]
}
```

```go
{
    "users": [
        {
            "id": 1,
            "parent_id": 1,
            "first_name": "John",
            "last_name": "Doe",
            "username": "user@example.com",
            "created_date": "2016-10-06T13:28:27+00:00",
            "status": "active",
            "role": {
                "id": 2,
                "name": "Corporate Admin",
            }
        },
        {...}
    ]
}
```

```javascript
{
    "users": [
        {
            "id": 1,
            "parent_id": 1,
            "first_name": "John",
            "last_name": "Doe",
            "username": "user@example.com",
            "created_date": "2016-10-06T13:28:27+00:00",
            "status": "active",
            "role": {
                "id": 2,
                "name": "Corporate Admin",
            }
        },
        {...}
    ]
}
```

<span title="get" class="pg-type type-get">get</span>

Retrieves a list of accessible all users.

### HTTP Request

`GET https://dev.qebot.com/api/v1/users`

### Returns
 Returns an array of users.

## Create User

> <b>POST /api/v1/users</b>

> Example Request

 ```shell
# With shell, you can just pass the correct header with each request
curl "https://dev.qebot.com/api/v1/users"
  -X POST
  -u "<API_TOKEN>"
  -d first_name=John
  -d last_name=Doe
  -d role_id=1
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
    "users": [
        {
            "id": 1,
            "parent_id": 1,
            "first_name": "John",
            "last_name": "Doe",
            "username": "user@example.com",
            "created_date": "2016-10-06T13:28:27+00:00",
            "status": "active",
            "role": {
                "id": 2,
                "name": "Corporate Admin",
            }
        }
    ]
}
```

```php
{
    "users": [
        {
            "id": 1,
            "parent_id": 1,
            "first_name": "John",
            "last_name": "Doe",
            "username": "user@example.com",
            "created_date": "2016-10-06T13:28:27+00:00",
            "status": "active",
            "role": {
                "id": 2,
                "name": "Corporate Admin",
            }
        }
    ]
}
```

```ruby
{
    "users": [
        {
            "id": 1,
            "parent_id": 1,
            "first_name": "John",
            "last_name": "Doe",
            "username": "user@example.com",
            "created_date": "2016-10-06T13:28:27+00:00",
            "status": "active",
            "role": {
                "id": 2,
                "name": "Corporate Admin",
            }
        }
    ]
}
```

```python
{
    "users": [
        {
            "id": 1,
            "parent_id": 1,
            "first_name": "John",
            "last_name": "Doe",
            "username": "user@example.com",
            "created_date": "2016-10-06T13:28:27+00:00",
            "status": "active",
            "role": {
                "id": 2,
                "name": "Corporate Admin",
            }
        }
    ]
}
```

```go
{
    "users": [
        {
            "id": 1,
            "parent_id": 1,
            "first_name": "John",
            "last_name": "Doe",
            "username": "user@example.com",
            "created_date": "2016-10-06T13:28:27+00:00",
            "status": "active",
            "role": {
                "id": 2,
                "name": "Corporate Admin",
            }
        }
    ]
}
```

```javascript
{
    "users": [
        {
            "id": 1,
            "parent_id": 1,
            "first_name": "John",
            "last_name": "Doe",
            "username": "user@example.com",
            "created_date": "2016-10-06T13:28:27+00:00",
            "status": "active",
            "role": {
                "id": 2,
                "name": "Corporate Admin",
            }
        }
    ]
}
```

<span title="post" class="pg-type type-post">post</span>

Create a user object.

### HTTP Request

`POST https://dev.qebot.com/api/v1/users`

<aside class="notice">
Username should be a valide email address.
</aside>

<aside class="notice">
The possible values for role_id can decrease based on role of authorized entity.
(e.g. a lower level role can not create a user with a higher role than itself)
</aside>

<h5 class="sidebar-nav-heading">Request Arguments</h5>
Param |   | Description
----- | - | -----------
first_name<br /><var>requried</var> | <i class="item-label">string</i> | First name of the user.
last_name<br /><var>requried</var> | <i class="item-label">string</i> | Last name of the user.
username<br /><var>requried</var> | <i class="item-label">string</i> | Username of the user.
password<br /><var>requried</var> | <i class="item-label">string</i> | Password of the user.
role_id<br /><var>requried</var> | <i class="item-label">string</i> | Role of the user. Possible values: (<b>1</b>, <b>2</b>,<b>3</b>,<b>4</b>).<br />See [Role](#role-object) Object
status | <i class="item-label">string</i>| Status of the user.<br />Possible values: (<b>active</b>, <b>inactive</b>)

### Returns
 Returns an array of a user.

## Retrieve User

> <b>GET /api/v1/users/ <var>id</var></b>

> Example Request

 ```shell
# With shell, you can just pass the correct header with each request
curl "https://dev.qebot.com/api/v1/users/<ID>"
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
    "users": [
        {
            "id": 1,
            "parent_id": 1,
            "first_name": "John",
            "last_name": "Doe",
            "username": "user@example.com",
            "created_date": "2016-10-06T13:28:27+00:00",
            "status": "active",
            "role": {
                "id": 2,
                "name": "Corporate Admin",
            }
        }
    ]
}
```

```php
{
    "users": [
        {
            "id": 1,
            "parent_id": 1,
            "first_name": "John",
            "last_name": "Doe",
            "username": "user@example.com",
            "created_date": "2016-10-06T13:28:27+00:00",
            "status": "active",
            "role": {
                "id": 2,
                "name": "Corporate Admin",
            }
        }
    ]
}
```

```ruby
{
    "users": [
        {
            "id": 1,
            "parent_id": 1,
            "first_name": "John",
            "last_name": "Doe",
            "username": "user@example.com",
            "created_date": "2016-10-06T13:28:27+00:00",
            "status": "active",
            "role": {
                "id": 2,
                "name": "Corporate Admin",
            }
        }
    ]
}
```

```python
{
    "users": [
        {
            "id": 1,
            "parent_id": 1,
            "first_name": "John",
            "last_name": "Doe",
            "username": "user@example.com",
            "created_date": "2016-10-06T13:28:27+00:00",
            "status": "active",
            "role": {
                "id": 2,
                "name": "Corporate Admin",
            }
        }
    ]
}
```

```go
{
    "users": [
        {
            "id": 1,
            "parent_id": 1,
            "first_name": "John",
            "last_name": "Doe",
            "username": "user@example.com",
            "created_date": "2016-10-06T13:28:27+00:00",
            "status": "active",
            "role": {
                "id": 2,
                "name": "Corporate Admin",
            }
        }
    ]
}
```

```javascript
{
    "users": [
        {
            "id": 1,
            "parent_id": 1,
            "first_name": "John",
            "last_name": "Doe",
            "username": "user@example.com",
            "created_date": "2016-10-06T13:28:27+00:00",
            "status": "active",
            "role": {
                "id": 2,
                "name": "Corporate Admin",
            }
        }
    ]
}
```

<span title="get" class="pg-type type-get">get</span>

Retrieves a user from a previously created user object.

To retrieve a user object you must supply the uniqe identifier <var>id</var> to user's resouce link
<i class="item-label">/api/v1/users/ <var>id</var></i> 

### HTTP Request

`GET https://dev.qebot.com/api/v1/users/<ID>`

### Returns
 Returns an array of a user.

## Update User

> <b>PUT /api/v1/users/ <var>id</var></b>

> <b>PATCH /api/v1/users/ <var>id</var></b>

> Example Request

 ```shell
# User id needs to be appended after api uri
curl "https://dev.qebot.com/api/v1/users/<ID>"
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
    "users": [
        {
            "id": 1,
            "parent_id": 1,
            "first_name": "John",
            "last_name": "Doe",
            "username": "user@example.com",
            "created_date": "2016-10-06T13:28:27+00:00",
            "status": "active",
            "role": {
                "id": 2,
                "name": "Corporate Admin",
            }
        }
    ]
}
```

```php
{
    "users": [
        {
            "id": 1,
            "parent_id": 1,
            "first_name": "John",
            "last_name": "Doe",
            "username": "user@example.com",
            "created_date": "2016-10-06T13:28:27+00:00",
            "status": "active",
            "role": {
                "id": 2,
                "name": "Corporate Admin",
            }
        }
    ]
}
```

```ruby
{
    "users": [
        {
            "id": 1,
            "parent_id": 1,
            "first_name": "John",
            "last_name": "Doe",
            "username": "user@example.com",
            "created_date": "2016-10-06T13:28:27+00:00",
            "status": "active",
            "role": {
                "id": 2,
                "name": "Corporate Admin",
            }
        }
    ]
}
```

```python
{
    "users": [
        {
            "id": 1,
            "parent_id": 1,
            "first_name": "John",
            "last_name": "Doe",
            "username": "user@example.com",
            "created_date": "2016-10-06T13:28:27+00:00",
            "status": "active",
            "role": {
                "id": 2,
                "name": "Corporate Admin",
            }
        }
    ]
}
```

```go
{
    "users": [
        {
            "id": 1,
            "parent_id": 1,
            "first_name": "John",
            "last_name": "Doe",
            "username": "user@example.com",
            "created_date": "2016-10-06T13:28:27+00:00",
            "status": "active",
            "role": {
                "id": 2,
                "name": "Corporate Admin",
            }
        }
    ]
}
```

```javascript
{
    "users": [
        {
            "id": 1,
            "parent_id": 1,
            "first_name": "John",
            "last_name": "Doe",
            "username": "user@example.com",
            "created_date": "2016-10-06T13:28:27+00:00",
            "status": "active",
            "role": {
                "id": 2,
                "name": "Corporate Admin",
            }
        }
    ]
}
```

<span title="put" class="pg-type type-put">post</span>
<span title="patch" class="pg-type type-patch">post</span>

Updates a user object.

To update a user object you must supply the uniqe identifier <var>id</var> to user's resouce link
<i class="item-label">/api/v1/users/ <var>id</var></i>

### HTTP Request

`PUT https://dev.qebot.com/api/v1/users/<ID>`

`PATCH https://dev.qebot.com/api/v1/users/<ID>`

<aside class="notice">
Even though all user params are optional.  If an empty request is passed an error will be thrown.
</aside>

<h5 class="sidebar-nav-heading">Request Arguments</h5>
Param |   | Description
----- | - | -----------
first_name | <i class="item-label">string</i> | First name of user.
last_name | <i class="item-label">string</i> | Last name of user.
username | <i class="item-label">string</i> | Username of user, valid email address.
password | <i class="item-label">string</i> | Password of user.
status | <i class="item-label">string</i> | Status of user.<br />Possible values: (<b>active</b>, <b>inactive</b>)


### Returns
 Returns an array of a user.

## Delete User

> <b>DELETE /api/v1/users/ <var>id</var></b>

> Example Request

 ```shell
# User id needs to be appended after api uri
curl "https://dev.qebot.com/api/v1/users/<ID>"
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

Deletes a user object.

To delete a user object you must supply the uniqe identifier <var>id</var> to user's resouce link
<i class="item-label">/api/v1/users/ <var>id</var></i>

### HTTP Request

`DELETE https://dev.qebot.com/api/v1/users/<ID>`

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

