# PWA notes

## Advice on performance budgets (On 3G)
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

## The course misses out a few key things while following along:

`https://app.pluralsight.com/player?course=building-performant-progressive-web-apps-scratch&author=jad-joubran&name=fc68b6d5-7608-46a1-b132-2947f3e67328&clip=5&mode=live`

* in the sw.js demo, the index.js needs refereencing in index.html to get what the demo shows (then removed later for the webpack version)
* it doesn't cover initialising webpack configs, so this is needed in the root of the app:


```sh
npm i -g create-webpack-config
webpack-config init
```
this generates a bunch of webpack template files

Pull in dependancies:
```sh
npm insall 
```

## Links
https://github.com/Polymer/pwa-starter-kit
https://pwa-starter-kit.polymer-project.org/setup
https://pwa-starter-kit.polymer-project.org/
https://www.polymer-project.org/
https://developers.google.com/web/fundamentals/primers/service-workers/

### Webpack
There's a bunch of webpack stuff that's pre-installed and not coverred in tyhe course, so:
* [outdated] https://app.pluralsight.com/library/courses/webpack-fundamentals/exercise-files
    * https://github.com/joeeames/WebpackFundamentalsCourse
* https://app.pluralsight.com/player?course=transpiling-bundling-javascript-webpack&author=wes-mcclure&name=fd890a11-b47f-4aa4-9824-5764b851aebe&clip=1&mode=live
    * https://github.com/g0t4/optimizing-web-apps-webpack

### Vue.js
* https://vuejs.org/v2/guide/installation.html


### Electron
* https://github.com/yoDon/Electron.NET-React-Typescript-MobX
* https://www.nuget.org/packages/ElectronNET.API/
* https://github.com/ElectronNET/Electron.NET



## Working around corporate stuff
https://stackoverflow.com/questions/13913941/how-to-fix-ssl-certificate-error-when-running-npm-on-windows

npm config set cafile "c:/**/[file].pem"
