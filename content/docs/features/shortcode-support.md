---
title: Shortcode support
---

When your shortcode (youtube.html for example) starts with a comment in which you show how it can be used, the CMS reads that comment. An example is shown below.

```
<!-- 
{{/* 
    
    Usage: 
    {{</* youtube id="qtIqKaDlqXo" image="/uploads/youtubeposter.jpg" */>}} 
    
*/}}
-->
```

If you add something similar to the code above, the CMS will add a button called 'youtube' that will insert this example shortcode.