---
description: null
seo-description: null
seo-title: Retrieving Stored Identifiers
title: Retrieving Stored Identifiers
uuid: c20474fc-8361-4a60-b2f0-631fb3a23120
index: y
internal: n
snippet: y
translate: y
---

# Retrieving Stored Identifiers

This information helps you retrieve locally stored user identities from your Roku app.


>[!IMPORTANT]
>
>The ` getAllIdentifiers()` method retrieves all user identities known and persisted by the Roku SDK. You must call this method **before** a user opts-out. 



The locally stored identities are returned in a JSON string, which might contain: 

* Company Context - IMS Org IDs
* User IDs
* Experience Cloud ID (MCID)
* Data Source IDs (DPID, DPUUID)
* Analytics IDs (AVID, AID, VID, and associated RSIDs)
* Audience Manager ID (UUID)
For example: 
```
vids&amp;nbsp;=&amp;nbsp;ADBMobile().getAllIdentifiers()
```
