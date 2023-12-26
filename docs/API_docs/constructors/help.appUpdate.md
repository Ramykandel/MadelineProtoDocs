---
title: "help.appUpdate"
description: "An update is available for the application."
nav_exclude: true
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
redirect_from: /API_docs/constructors/help_appUpdate.html
---
# Constructor: help.appUpdate  
[Back to constructors index](/API_docs/constructors/index.html)



An update is available for the application.

### Attributes:

| Name     |    Type       | Required | Description |
|----------|---------------|----------|-------------|
|can\_not\_skip|[Bool](/API_docs/types/Bool.html) | Optional|Unskippable, the new info must be shown to the user (with a popup or something else)|
|id|[int](/API_docs/types/int.html) | Yes|Update ID|
|version|[string](/API_docs/types/string.html) | Yes|New version name|
|text|[string](/API_docs/types/string.html) | Yes|Text description of the update|
|entities|Array of [MessageEntity](/API_docs/types/MessageEntity.html) | Yes|[Message entities for styled text](https://core.telegram.org/api/entities)|
|parse\_mode| [string](/API_docs/types/string.html) | Whether to parse HTML or Markdown markup in the message| Optional |
|document|[Document](/API_docs/types/Document.html) | Optional|Application binary|
|url|[string](/API_docs/types/string.html) | Optional|Application download URL|
|sticker|[Document](/API_docs/types/Document.html) | Optional|Associated sticker|



### Type: [help.AppUpdate](/API_docs/types/help.AppUpdate.html)



## Usage of parse_mode:

Set parse_mode to html to enable HTML parsing of the message.  

Set parse_mode to Markdown to enable markdown parsing of the message.  

The following tags are currently supported:

```html
<br>a newline
<b><i>bold works ok, internal tags are stripped</i> </b>
<strong>bold</strong>
<em>italic</em>
<i>italic</i>
<u>underline</u>
<s>strikethrough</s>
<del>strikethrough</del>
<strike>strikethrough</strike>
<code>inline fixed-width code</code>
<pre>pre-formatted fixed-width code block</pre>
<blockquote>pre-formatted fixed-width code block</blockquote>
<a href="https://github.com">URL</a>
<a href="mention:@danogentili">Mention by username</a>
<a href="mention:186785362">Mention by user id</a>
<a href="tg://user?id=186785362">Mention by user id</a>
Custom emoji: <emoji id="5368324170671202286">👍</emoji>
Custom emoji: <tg-emoji emoji-id="5368324170671202286">👍</tg-emoji>
<pre language="json">Pre tags can have a language attribute</pre>
<spoiler>Spoiler</spoiler>
<tg-spoiler>Spoiler</tg-spoiler>
```

You can also use normal markdown ([bot API MarkdownV2 syntax](https://core.telegram.org/bots/api#markdownv2-style)), note that to create mentions you can also use the `mention:` syntax like in html:  

```markdown
*bold \*text*
_italic \*text_
__underline__
~strikethrough~
||spoiler||
*bold _italic bold ~italic bold strikethrough ||italic bold strikethrough spoiler||~ __underline italic bold___ bold*
[inline URL](http://www.example.com/)
[inline mention of a user](tg://user?id=123456789)
![👍](tg://emoji?id=5368324170671202286)
\`inline fixed-width code\`
\`\`\`
pre-formatted fixed-width code block
\`\`\`
\`\`\`php
pre-formatted fixed-width code block written in the PHP programming language
\`\`\`

[Mention by username](mention:@danogentili)
[Mention by user id](mention:186785362)
[Mention by user id](tg://user?id=186785362)
[👍](emoji:5368324170671202286)
[👍](tg://emoji?id=5368324170671202286)
```

### Example:

```
$help_appUpdate = ['_' => 'help.appUpdate', 'can_not_skip' => Bool, 'id' => int, 'version' => 'string', 'text' => 'string', 'entities' => [MessageEntity, MessageEntity]parse_mode: 'string', , 'document' => Document, 'url' => 'string', 'sticker' => Document];
```  
