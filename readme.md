# PWA notes

## On 3G
* aim for <=1 second load 
* 900Kb/s, 40ms latency
* App Shell HTML+CSS+JS <= 50kb


Web fonts are slow  -   Use system/device fonts
```css
html {
    font-family: system-ui, -apple-system, BlinkMacSystemFont, 
                "Segoe UI", Roboto, Oxygen, Ubuntu, Cantarell, 
                "Fira Sans", "Droid Sans", "Helvetica Neue", sans-serif
}
```

## The course misses out a few key things whiole following along:

* in the sw.js demo, the index.js needs refereencing in index.html to get what the demo shows (then removed later for the webpack version)
* it doesn't cover initialising webpack configs, so this is needed in the root of the app:
```sh
npm i -g create-webpack-config
webpack-config init
```
this generates a bunch of webpack template files