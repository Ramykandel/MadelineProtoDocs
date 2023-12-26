---
title: "topPeer"
description: "Top peer"
nav_exclude: true
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Constructor: topPeer  
[Back to constructors index](/API_docs/constructors/index.html)



Top peer

### Attributes:

| Name     |    Type       | Required | Description |
|----------|---------------|----------|-------------|
|peer|[long](/API_docs/types/long.html) | Yes|Peer|
|rating|[double](/API_docs/types/double.html) | Yes|Rating as computed in [top peer rating »](https://core.telegram.org/api/top-rating)|



### Type: [TopPeer](/API_docs/types/TopPeer.html)


### Example:

```
$topPeer = ['_' => 'topPeer', 'peer' => long, 'rating' => double];
```  
