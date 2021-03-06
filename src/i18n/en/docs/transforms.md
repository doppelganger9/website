# 🐠 Transforms

While many bundlers require you to install and configure plugins to transform assets, Parcel has support for many common transforms and transpilers built in out of the box. You can transform JavaScript using [Babel](https://babeljs.io), CSS using [PostCSS](http://postcss.org), and HTML using [PostHTML](https://github.com/posthtml/posthtml). Parcel automatically runs these transforms when it finds a configuration file (e.g. `.babelrc`, `.postcssrc`) in a module.

This even works in third-party `node_modules`: if a configuration file is published as part of the package, the transform is automatically turned on for that module only. This keeps bundling fast since only modules that need to be transformed are processed. It also means that you don't need to manually configure the transforms to include and exclude certain files, or know how third party code is built in order to use it in your application.
