---
title: Setting the HTTP request type in your player
description: 
uuid: b8fa7233-e654-4acf-a9d7-14158cded13e

---

# Setting the HTTP request type {#setting-the-http-request-type}

The request body for all Media Collection API requests must be in JSON format, so you should set the content request type in your player. For example, in JavaScript you would set the `Content-Type` request header as follows: 

```
httpRequest.setRequestHeader('Content-Type', 'application/json'); 
```

