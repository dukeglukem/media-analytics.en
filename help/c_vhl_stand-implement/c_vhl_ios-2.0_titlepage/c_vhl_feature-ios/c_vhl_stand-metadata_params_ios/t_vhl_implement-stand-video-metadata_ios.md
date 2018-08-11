---
description: null
seo-description: null
seo-title: Implementation for standard video metadata
title: Implementation for standard video metadata
uuid: cfbc8804-baf2-4fb2-a3a3-664b057ace04
index: y
internal: n
snippet: y
translate: y
---

# Implementation for standard video metadata

Here is the Standard Metadata Constants reference: 



|  Constant name  | Description  |
|---|---|
|  ` ADBMediaObjectKeyStandardVideoMetadata`  | Constant for attaching standard video metadata on ` MediaInfo ADBMediaObject`  |
|  ` ADBMediaObjectKeyStandardAdMetadata`  | Constant for attaching standard ad metadata on ` AdInfo ADBMediaObject`  |


>1. Create a dictionary of standard Video metadata key value pairs using the ` ADBStandardMetadataKeys` specified above.
>1. Set the standard video metadata dictionary on ` MediaInfo` ` ADBMediaObject` instance using the Standard Metadata constant for video metadata.
>1. Provide this ` MediaInfo` object while invoking the ` trackSessionStart` API.