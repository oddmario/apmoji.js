# 🚀 Apmoji.js
## Apple Emojis for the Web ☄️

![GitHub License](https://img.shields.io/github/license/oddmario/apmoji.js)
![GitHub commit activity](https://img.shields.io/github/commit-activity/m/oddmario/apmoji.js)
![GitHub Issues or Pull Requests](https://img.shields.io/github/issues/oddmario/apmoji.js)
![GitHub Issues or Pull Requests](https://img.shields.io/github/issues-pr/oddmario/apmoji.js)

a project inspired by the Twitter/X Twemoji project — https://github.com/twitter/twemoji — **but** for the Apple Emoji set instead

<p align="center">
  <img width="700" height="auto" src="https://i.ibb.co/TKFf8SR/image.png">
</p>

-----

## Usage
You may include Apmoji.js from the [jsDelivr CDN](https://www.jsdelivr.com/), or you may alternatively host it locally by hosting the `dist/apmoji-vX.Y.min.js` file on your server and embedding it onto your application from there.

To include Apmoji.js from jsDelivr, append the following line inside your `<head></head>` tag:
```html
<script src="https://cdn.jsdelivr.net/gh/oddmario/apmoji.js/dist/apmoji-v1.0.min.js"></script>
```

You can then start making your web pages look prettier using the main function of Apmoji.js, `apmoji.parse()`:
```js
apmoji.parse(document.body) // finds any emojis inside the DOM body and converts them to Apple emojis
apmoji.parse(document.querySelector("#mycooldiv")) // finds any emojis inside the #mycooldiv DOM element and converts them to Apple emojis
```

**Or alternatively:**

You can apply the `apmoji` class on any element that contains an emoji. It will use the Apple emojis font as long as Apmoji.js has been initialised using `apmoji.init()` at least once.

```html
<script>
  apmoji.init();
</script>

<span class="apmoji">🥸</span>
```

### Simple is it not?

## License
- Code licensed under the MIT License: http://opensource.org/licenses/MIT
- Emoji CDN provided by https://github.com/benborgers/emojicdn