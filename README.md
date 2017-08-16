<p align="center">
    <a href="http://nai8.me" target="_blank">
        <img width="250" height="80" src="http://nai8.me/images/ext-logos/yii2-emoji-logo.png">
    </a>
</p>

# Install
$ composer require abei2017/yii2-emoji
> only used in yii2.
# Usage
```php
use abei2017\emoji\Emoji;
Emoji::shortnameToImage('hello:smile:');// hello <img class="emojione" alt="😄" title=":smile:" src="https://cdn.jsdelivr.net/emojione/assets/3.1/png/32/1f604.png">
Emoji::toShort('😄'); // :smile:
Emoji::unicodeToImage('😄'); // <img class="emojione" alt="😄" title=":smile:" src="https://cdn.jsdelivr.net/emojione/assets/3.1/png/32/1f604.png">
Emoji::toImage(':smile:'); // <img class="emojione" alt="😄" title=":smile:" src="https://cdn.jsdelivr.net/emojione/assets/3.1/png/32/1f604.png">
Emoji::shortnameToUnicode(':smile:'); // 😄
```
# Config
```php
// config/web.php
return [
    ...
    'yii2Emoji'=>[
        'emojiSize'=>'32',//32、64、128
    ]
];
```

# License
MIT