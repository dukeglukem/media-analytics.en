---
description: Actions are the events that occur in your app that you want to measure.
seo-description: Actions are the events that occur in your app that you want to measure.
seo-title: Track App Actions
title: Track App Actions
uuid: 188be0a6-271c-4a6b-806d-02abe7240f47
index: y
internal: n
snippet: y
translate: y
---

# Track App Actions

Each action has one or more corresponding metrics that are incremented each time the event occurs. For example, you might send a ` trackAction` call for each new subscription, each time a content is rated, or each time a level is completed. Actions are not tracked automatically, so call ` trackAction` when an event that you want to track occurs, and map the action to a custom event. 

>1. When an event you want to track occurs, call ` trackAction`.
>
>   ```
>   ADBMobile().trackAction("myapp.ActionName",&amp;nbsp;{})
>   ```
>
>1. Map the action to a custom event.
>   You can also send additional context data with each track action call. 
>
>   ```
>   dictionary = {} 
>   dictionary["myapp.social.SocialSource"] = "Twitter"  
>   ADBMobile().trackAction("myapp.SocialShare", dictionary)
>   ```
>