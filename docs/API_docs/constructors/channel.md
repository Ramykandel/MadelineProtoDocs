---
title: "channel"
description: "Channel/supergroup info"
nav_exclude: true
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Constructor: channel  
[Back to constructors index](/API_docs/constructors/index.html)



Channel/supergroup info

### Attributes:

| Name     |    Type       | Required | Description |
|----------|---------------|----------|-------------|
|creator|[Bool](/API_docs/types/Bool.html) | Optional|Whether the current user is the creator of this channel|
|left|[Bool](/API_docs/types/Bool.html) | Optional|Whether the current user has left this channel|
|broadcast|[Bool](/API_docs/types/Bool.html) | Optional|Is this a channel?|
|verified|[Bool](/API_docs/types/Bool.html) | Optional|Is this channel verified by telegram?|
|megagroup|[Bool](/API_docs/types/Bool.html) | Optional|Is this a supergroup?|
|restricted|[Bool](/API_docs/types/Bool.html) | Optional|Whether viewing/writing in this channel for a reason (see `restriction_reason`|
|signatures|[Bool](/API_docs/types/Bool.html) | Optional|Whether signatures are enabled (channels)|
|min|[Bool](/API_docs/types/Bool.html) | Optional|See [min](https://core.telegram.org/api/min)|
|scam|[Bool](/API_docs/types/Bool.html) | Optional|This channel/supergroup is probably a scam|
|has\_link|[Bool](/API_docs/types/Bool.html) | Optional|Whether this channel has a private join link|
|has\_geo|[Bool](/API_docs/types/Bool.html) | Optional|Whether this chanel has a geoposition|
|slowmode\_enabled|[Bool](/API_docs/types/Bool.html) | Optional|Whether slow mode is enabled for groups to prevent flood in chat|
|call\_active|[Bool](/API_docs/types/Bool.html) | Optional|Whether a group call or livestream is currently active|
|call\_not\_empty|[Bool](/API_docs/types/Bool.html) | Optional|Whether there's anyone in the group call or livestream|
|fake|[Bool](/API_docs/types/Bool.html) | Optional|If set, this [supergroup/channel](https://core.telegram.org/api/channel) was reported by many users as a fake or scam: be careful when interacting with it.|
|gigagroup|[Bool](/API_docs/types/Bool.html) | Optional|Whether this [supergroup](https://core.telegram.org/api/channel) is a gigagroup|
|noforwards|[Bool](/API_docs/types/Bool.html) | Optional|Whether this channel or group is [protected](https://telegram.org/blog/protected-content-delete-by-date-and-more), thus does not allow forwarding messages from it|
|join\_to\_send|[Bool](/API_docs/types/Bool.html) | Optional|Whether a user needs to join the supergroup before they can send messages: can be false only for [discussion groups »](https://core.telegram.org/api/discussion), toggle using [channels.toggleJoinToSend](../methods/channels.toggleJoinToSend.html)|
|join\_request|[Bool](/API_docs/types/Bool.html) | Optional|Whether a user's join request will have to be [approved by administrators](https://core.telegram.org/api/invites#join-requests), toggle using [channels.toggleJoinToSend](../methods/channels.toggleJoinRequest.html)|
|forum|[Bool](/API_docs/types/Bool.html) | Optional|Whether this supergroup is a [forum](https://core.telegram.org/api/forum)|
|stories\_hidden|[Bool](/API_docs/types/Bool.html) | Optional|
|stories\_hidden\_min|[Bool](/API_docs/types/Bool.html) | Optional|
|stories\_unavailable|[Bool](/API_docs/types/Bool.html) | Optional|
|id|[long](/API_docs/types/long.html) | Yes|ID of the channel|
|access\_hash|[long](/API_docs/types/long.html) | Optional|Access hash|
|title|[string](/API_docs/types/string.html) | Yes|Title|
|username|[string](/API_docs/types/string.html) | Optional|Username|
|photo|[ChatPhoto](/API_docs/types/ChatPhoto.html) | Optional|Profile photo|
|date|[int](/API_docs/types/int.html) | Yes|Date when the user joined the supergroup/channel, or if the user isn't a member, its creation date|
|restriction\_reason|Array of [RestrictionReason](/API_docs/types/RestrictionReason.html) | Optional|Contains the reason why access to this channel must be restricted.|
|admin\_rights|[ChatAdminRights](/API_docs/types/ChatAdminRights.html) | Optional|Admin rights of the user in this channel (see [rights](https://core.telegram.org/api/rights))|
|banned\_rights|[ChatBannedRights](/API_docs/types/ChatBannedRights.html) | Optional|Banned rights of the user in this channel (see [rights](https://core.telegram.org/api/rights))|
|default\_banned\_rights|[ChatBannedRights](/API_docs/types/ChatBannedRights.html) | Optional|Default chat rights (see [rights](https://core.telegram.org/api/rights))|
|participants\_count|[int](/API_docs/types/int.html) | Optional|Participant count|
|usernames|Array of [Username](/API_docs/types/Username.html) | Optional|
|stories\_max\_id|[int](/API_docs/types/int.html) | Optional|
|color|[PeerColor](/API_docs/types/PeerColor.html) | Optional|
|profile\_color|[PeerColor](/API_docs/types/PeerColor.html) | Optional|
|emoji\_status|[EmojiStatus](/API_docs/types/EmojiStatus.html) | Optional|
|level|[int](/API_docs/types/int.html) | Optional|



### Type: [Chat](/API_docs/types/Chat.html)


### Example:

```
$channel = ['_' => 'channel', 'creator' => Bool, 'left' => Bool, 'broadcast' => Bool, 'verified' => Bool, 'megagroup' => Bool, 'restricted' => Bool, 'signatures' => Bool, 'min' => Bool, 'scam' => Bool, 'has_link' => Bool, 'has_geo' => Bool, 'slowmode_enabled' => Bool, 'call_active' => Bool, 'call_not_empty' => Bool, 'fake' => Bool, 'gigagroup' => Bool, 'noforwards' => Bool, 'join_to_send' => Bool, 'join_request' => Bool, 'forum' => Bool, 'stories_hidden' => Bool, 'stories_hidden_min' => Bool, 'stories_unavailable' => Bool, 'id' => long, 'access_hash' => long, 'title' => 'string', 'username' => 'string', 'photo' => ChatPhoto, 'date' => int, 'restriction_reason' => [RestrictionReason, RestrictionReason], 'admin_rights' => ChatAdminRights, 'banned_rights' => ChatBannedRights, 'default_banned_rights' => ChatBannedRights, 'participants_count' => int, 'usernames' => [Username, Username], 'stories_max_id' => int, 'color' => PeerColor, 'profile_color' => PeerColor, 'emoji_status' => EmojiStatus, 'level' => int];
```  
