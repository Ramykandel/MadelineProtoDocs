---
title: "stories.getStoryViewsList"
description: "stories.getStoryViewsList parameters, return type and example"
grand_parent: "Telegram RPC API"
parent: "Methods"
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
redirect_from: /API_docs/methods/stories_getStoryViewsList.html
---
# Method: stories.getStoryViewsList
[Back to methods index](index.html)



### Parameters:

| Name     |    Type       | Required |
|----------|---------------|----------|
|just\_contacts|[Bool](/API_docs/types/Bool.html) | Optional|
|reactions\_first|[Bool](/API_docs/types/Bool.html) | Optional|
|forwards\_first|[Bool](/API_docs/types/Bool.html) | Optional|
|peer|[Username, chat ID, Update, Message or InputPeer](/API_docs/types/InputPeer.html) | Optional|
|q|[string](/API_docs/types/string.html) | Optional|
|id|[int](/API_docs/types/int.html) | Optional|
|offset|[string](/API_docs/types/string.html) | Optional|
|limit|[int](/API_docs/types/int.html) | Optional|


### Return type: [stories.StoryViewsList](/API_docs/types/stories.StoryViewsList.html)

### Can bots use this method: **NO**


### MadelineProto Example ([now async for huge speed and parallelism!](https://docs.madelineproto.xyz/docs/ASYNC.html)):


```php
if (!file_exists('madeline.php')) {
    copy('https://phar.madelineproto.xyz/madeline.php', 'madeline.php');
}
include 'madeline.php';

$MadelineProto = new \danog\MadelineProto\API('session.madeline');
$MadelineProto->start();

$stories_StoryViewsList = $MadelineProto->stories->getStoryViewsList(just_contacts: $Bool, reactions_first: $Bool, forwards_first: $Bool, peer: $InputPeer, q: 'string', id: $int, offset: 'string', limit: $int, );
```

