---
description: How to request our API.
---

# Requests

The response that will be obtained varies from the type of endpoint \(`JSON` or `BUFFER`\)

## JavaScript

To obtain the **JSON** response from a request to an API, you must use a package that allows you to do so, such as [axios ](https://npmjs.com/package/axios)or [node-fetch](https://npmjs.com/packages/node-fetch)

**Example:**

```javascript
(async () => {
const fetch = require('node-fetch').default
const url = 'https://api.willz.repl.co/endpoint?key=TOKEN'

const data = await fetch(url)
const res = await data.json()

return res //now res has the JSON response
})
```

## Wrappers

To get the JSON data in discord.js/.go wrappers such as **BDFD** or **AOI.JS** You can use their functions to do it.

**BDFD:**  
Using `$httpGet[url]`& `$httpResult[property;property;...]`

```markup
$nomention
$httpGet[https://api.willz.repl.co/endpoint?key=TOKEN]
$title[Response]
$description[$httpResult[property]]
```

**AOI.JS:**  
Using `$jsonRequest[link;property;error message;Hname:Hvalue;...]`

```javascript
bot.command({
name: "data",
code: `$title[Response]
$description[$jsonRequest[https://api.willz.repl.co/endpoint?key=TOKEN;property;Error!!]]`
})
```

