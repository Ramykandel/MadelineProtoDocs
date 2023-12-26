---
title: "account.updateColor"
description: "account.updateColor parameters, return type and example"
grand_parent: "Telegram RPC API"
parent: "Methods"
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
redirect_from: /API_docs/methods/account_updateColor.html
---
# Method: account.updateColor
[Back to methods index](index.html)



### Parameters:

| Name     |    Type       | Required |
|----------|---------------|----------|
|for\_profile|[Bool](/API_docs/types/Bool.html) | Optional|
|color|[int](/API_docs/types/int.html) | Optional|
|background\_emoji\_id|[long](/API_docs/types/long.html) | Optional|


### Return type: [Bool](/API_docs/types/Bool.html)

### Can bots use this method: **NO**


### MadelineProto Example ([now async for huge speed and parallelism!](https://docs.madelineproto.xyz/docs/ASYNC.html)):


```php
if (!file_exists('madeline.php')) {
    copy('https://phar.madelineproto.xyz/madeline.php', 'madeline.php');
}
include 'madeline.php';

$MadelineProto = new \danog\MadelineProto\API('session.madeline');
$MadelineProto->start();

$Bool = $MadelineProto->account->updateColor(for_profile: $Bool, color: $int, background_emoji_id: $long, );
```

