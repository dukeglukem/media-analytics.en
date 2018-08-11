---
description: null
seo-description: null
seo-title: Tracking errors
title: Tracking errors
uuid: 9edcec54-c9d3-448c-8aea-00f846770a9b
index: y
internal: n
snippet: y
translate: y
---

# Tracking errors

Before you configure error tracking, see [ Implement the Android library ](c_vhl_imp-lib-android.md#concept_A72BFE683F4A4A3397FD0C71E955DF07). 

>1. To track video player errors:
>
>   ```
>   java>   public void onPlayerError(Observable observable, Object data) {  
>       _heartbeat.trackError("videoErrorID"); 
>   }
>   ```

>   >[!NOTE]
>   >
>   >Tracking video player errors will not stop the video tracking session. If the video player error prevents the playback from continuing, make sure that the video tracking session is closed by calling ` trackSessionEnd()` after calling ` trackError()`. 
>