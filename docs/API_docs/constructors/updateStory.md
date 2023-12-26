---
title: "updateStory"
description: "updateStory attributes, type and example"
nav_exclude: true
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Constructor: updateStory  
[Back to constructors index](/API_docs/constructors/index.html)



### Attributes:

| Name     |    Type       | Required |
|----------|---------------|----------|
|peer|[long](/API_docs/types/long.html) | Yes|
|story|[StoryItem](/API_docs/types/StoryItem.html) | Yes|



### Type: [Update](/API_docs/types/Update.html)


### Example:

```
$updateStory = ['_' => 'updateStory', 'peer' => long, 'story' => StoryItem];
```  
