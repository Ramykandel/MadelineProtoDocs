---
title: "updatePeerHistoryTTL"
description: "The Time-To-Live for messages sent by the current user in a specific chat has changed"
nav_exclude: true
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Constructor: updatePeerHistoryTTL  
[Back to constructors index](/API_docs/constructors/index.html)



The Time-To-Live for messages sent by the current user in a specific chat has changed

### Attributes:

| Name     |    Type       | Required | Description |
|----------|---------------|----------|-------------|
|peer|[long](/API_docs/types/long.html) | Yes|The chat|
|ttl\_period|[int](/API_docs/types/int.html) | Optional|The new Time-To-Live|



### Type: [Update](/API_docs/types/Update.html)


### Example:

```
$updatePeerHistoryTTL = ['_' => 'updatePeerHistoryTTL', 'peer' => long, 'ttl_period' => int];
```  
