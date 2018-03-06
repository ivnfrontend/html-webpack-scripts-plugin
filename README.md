# HTMLWebpackScripts
`HTMLWebpackScripts` is a plugin for [Webpack](https://webpack.js.org/).

### Why
By default Webpack will generate plain scripts with like `/bundles/vendor.0a78e31b5c440.js`. In order to serve these script assets and  other generated assets by Webpack (like stylesheets) you should have index.html file and include those assets manually or a plugin that generates HTML and includes those assets automatically, like [`HTML Webpack Plugin`](https://www.npmjs.com/package/html-webpack-plugin).
More likely you'll use the second option and generate HTML automatically.

However [`HTML Webpack Plugin`](https://www.npmjs.com/package/html-webpack-plugin) will add plain scripts into generated HTML like `<script type="text/javascript" src="/bundles/vendor.0a78e31b5c440.js"></script>`. It won't give you additional control over those scripts.


But if you want to enhance the control of those scripts and additional attributes like `defer` or `async` or `crossorigin` or even custom attributes like `data-script-inlined`, `HTMLWebpackScripts` plugin for you!
