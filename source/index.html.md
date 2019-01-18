---
title: API Reference

language_tabs: # must be one of https://git.io/vQNgJ
  - shell
  - php
  - ruby
  - python
  - go
  - javascript

toc_footers:
  - <a href='#'>Sign Up for a Developer Key</a>
  - <a href='https://github.com/lord/slate'>Documentation Powered by Slate</a>

includes:
  - errors
  - brands
  - businesses
  - users
  - tools
  - billings
  - purchases
  

search: true
---

# Introduction

Welcome to the Qebot API!  The platform API follows a [REST](https://en.wikipedia.org/wiki/Representational_state_transfer)ful architecture that empowers developers to automate, extend and combine Qebot with other services.

We will have language bindings in Shell, PHP, Ruby, Python, Go, and JavaScript!  Please check back to see if the language you use is available. You can view code examples in the dark area to the right, and you can switch the programming language of the examples with the tabs in the top right.

# Authentication

> To authorize, use this code:

```ruby
require 'kittn'

api = Kittn::APIClient.authorize!('meowmeowmeow')
```

```python
import kittn

api = kittn.authorize('meowmeowmeow')
```

```shell
# With shell, you can just pass the correct header with each request
curl "api_endpoint_here"
  -H "Authorization: meowmeowmeow"
```

```javascript
const kittn = require('kittn');

let api = kittn.authorize('meowmeowmeow');
```

> Make sure to replace `meowmeowmeow` with your API key.

Qebot uses an API key to allow access to the API. You can register a new Qebot API key at our [developer portal](http://example.com/developers).

Requests are authenticated using [HTTP Basic Auth](https://en.wikipedia.org/wiki/Basic_access_authentication). Provide your API key as the basic auth username. You do not need to provide a password.

