angular-loading-bar
===================

This project is a fork from: [chieffancypants/angular-loading-bar](https://github.com/chieffancypants/angular-loading-bar)

## Usage:

1. include the loading bar as a dependency for your app.  If you want animations, include `ngAnimate` as well. *note: ngAnimate is optional*

    ```js
    angular.module('myApp', ['angular-loading-bar', 'ngAnimate'])
    ```
    
2. include the supplied JS and CSS file (or create your own CSS to override defaults).

    ```html
    <link rel='stylesheet' href='build/loading-bar.min.css' type='text/css' media='all' />
    <script type='text/javascript' src='build/loading-bar.min.js'></script>
    ```

3. That's it -- you're done!


## Configuration

This fork has only one additional feature: select the parent element where the loading bar will be placed.
Note: this selector will be used on jqlite find method, but additionally it can accept ids.

```js
angular.module('myApp', ['angular-loading-bar'])
  .config(['cfpLoadingBarProvider', function(cfpLoadingBarProvider) {
    cfpLoadingBarProvider.parentSelector = '#myloadingbarcontainer'; // Default: 'body'
  }])
```

## Other modifications

This fork does not have the spinner, only the loading-bar.

## License:
Licensed under the MIT license
