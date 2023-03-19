<div align="center">
<br />

<picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/chatgptjs/chatgpt.js/main/media/images/chatgpt.js-logo-dark-mode-5995x614.png">
    <img width=546 alt="chatgpt.js" src="https://raw.githubusercontent.com/chatgptjs/chatgpt.js/main/media/images/chatgpt.js-logo-light-mode-5995x614.png">
</picture>


### A client-side JavaScript library for ChatGPT 🤖

</div>

## About

**chatgpt.js** is a powerful JavaScript library that allows for super easy interaction w/ the [ChatGPT DOM](https://chat.openai.com).

- Feature-rich
- Object-oriented
- Easy-to-use
- Lightweight (yet optimally performant)

## Importing the library

### ES6:

```js
import chatgpt from 'https://raw.githubusercontent.com/chatgptjs/chatgpt.js/main/chatgpt.js'
```

### ES5:

```js
(function() {
    var xhr = new XMLHttpRequest()
    xhr.open('GET', 'https://raw.githubusercontent.com/chatgptjs/chatgpt.js/main/chatgpt.js')
    xhr.onload = function() {
        if (xhr.status === 200) {
            var chatgptJS = document.createElement('script')
            chatgptJS.textContent = xhr.responseText
            document.head.appendChild(chatgptJS)
        }
    }
    xhr.send()
})()
```

### Greasemonkey:

```js
// @require https://raw.githubusercontent.com/chatgptjs/chatgpt.js/main/chatgpt.js
```

*Optional: To satisfy linting rules in editors like Tampermonkey's, add:*

```js
var chatgpt = window.chatgpt // retrieve chatgpt.js from window object
```

## Usage

**chatgpt.js** was written w/ ultra flexibility in mind.

For example:

```js
chatgpt.getLastResponse()
chatgpt.getLastReply()
chatgpt.get('reply', 'last')
```

Each of these calls successfully fetches the last response.

In other words, if you think it works, it probabily will... so just type it! (Who has time for docs?)

If it didn't, simply submit an [issue](https://github.com/chatgptjs/chatgpt.js/issues) or [PR](https://github.com/chatgptjs/chatgpt.js/pulls) and it will be integrated, ezpz!
