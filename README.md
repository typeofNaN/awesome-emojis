# Awesome Emojis 😄

一款基于Unicode的emoji表情包库，使用方便，提供三种不同格式的数据。

## Installation

``` sh
# using npm
npm install awesome-emojis --save

# using yarn
yarn add awesome-emojis

# using pnpm
pnpm add awesome-emojis
```

## Usage

本表情包库提供三种不同格式的数据：

* 分组数组数据

``` js
// ESM
import { EmojiGroup } from 'awesome-emojis'

// commonjs
const { EmojiGroup } = require('awesome-emojis')

console.log(EmojiGroup)
// [
//   {
//     "name": "Smileys & Emotion",
//     "slug": "smileys_emotion",
//     "emojis": [
//       {
//         "emoji": "😀",
//         "skin_tone_support": false,
//         "name": "grinning face",
//         "slug": "grinning_face",
//         "unicode_version": "1.0",
//         "emoji_version": "1.0"
//       },
//       ...
//     ]
//   },
//   ...
// ]
```

* 数组数据

``` js
import { EmojiList } from 'awesome-emojis'

console.log(EmojiList)
// [
//   {
//     "codes": "1F600",
//     "char": "😀",
//     "name": "grinning face",
//     "category": "Smileys & Emotion (face-smiling)",
//     "group": "Smileys & Emotion",
//     "subgroup": "face-smiling"
//   },
//   ...
// ]
```

* 对象键值对数据

``` js
import { Emojis } from 'awesome-emojis'

console.log(Emojis)
// {
//   "😀": {
//     "name": "grinning face",
//     "slug": "grinning_face",
//     "group": "Smileys & Emotion",
//     "emoji_version": "1.0",
//     "unicode_version": "1.0",
//     "skin_tone_support": false
//   },
//   ...
// }
```
