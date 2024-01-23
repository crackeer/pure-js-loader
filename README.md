
## import pure-js-loader.js

```js
<script src="https://cdn.jsdelivr.net/npm/pure-js-loader/loader.js" defer></script>
```

## write your js code
```js

// register css files
window.registerCssLibrary({
    'bootstrap5' : 'https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css',
})

// register js files
window.registerJSLibrary({
    'jquery': 'https://cdn.jsdelivr.net/npm/jquery@3.7.1/dist/jquery.min.js',
    'bootstrap5': 'https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.min.js',
    'vue' : 'https://cdn.jsdelivr.net/npm/vue@3.4.15/dist/vue.global.min.js',
    'bootbox': 'https://cdn.jsdelivr.net/npm/bootbox@6.0.0/dist/bootbox.min.js',
    'axios': 'https://cdn.jsdelivr.net/npm/axios@1.6.5/dist/axios.min.js',
    'dayjs' : 'https://cdn.jsdelivr.net/npm/dayjs@1.11.10/dayjs.min.js'
})

// choose load files
window.quickStart(['bootstrap5'], {
    'vue' : 1,
    'jquery' : 2,
    'bootstrap5' : 3,
    'bootbox' : 3,
    'axios' : 4,
    "dayjs" : 5,
}, async () => {
    // callback do something
})
```
