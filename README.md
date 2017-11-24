# ![](/assets/vue.jpg)Learning Vue.js - 2.x

[Read the book](https://narramadan.gitbooks.io/learning-vue-js/)

This gitbook is for my personal scribble notes that I keep when I learn new technology. I generally use a notebook and bring it along with me for references. I am replacing the way I do with Gitbook as I see this more effective for writing my notes and referring them when needed. Refer to the [Official Guide](https://vuejs.org/v2/guide/index.html) for more details and use this book for quick reference only...

Definition from the official guide for Vue

> Vue\(pronounced /vjuː/, like **view **\) is a **progressive framework **for building user interfaces.

More on [Progressive Framework](/quick-intro.md#progressive-framework)

# **Setting up development environment**

## Install Vue Command Line Interface

We will use [Yarn](https://yarnpkg.com/en/) as our Package Manager and [Webpack](https://webpack.js.org/) as our Module Bundler. We use [vue-cli](https://github.com/vuejs/vue-cli) to scaffold our project.

For all the above tools, we need to ensure that we have Node and NPM installed.

Download and Install Node.

* Verify if Node is working by running `node -v`
* Verify if NPM is working by running `npm -v`

Install Yarn by running `npm install -g yarn`

Install vue-cli by running `npm install --global vue-cli`

Run `vue init webpack sample` to create a sample project which will have a full-featured Webpack + vue-loader setup with hot reload, linting, testing & css extraction.

> vue init &lt;template-name&gt; &lt;project-name&gt; - We use [webpack Template](http://vuejs-templates.github.io/webpack/). Other templates can also be used. Vist vue-cli github page for more information

I choose `standard` ESLint template and `jest` for unit tests.

Below is the structure of the project that is created

```bash
C:\Work\Learning\Vue\sample>dir
 Volume in drive C is Avaya eSOE
 Volume Serial Number is 6CAC-F283

 Directory of C:\Work\Learning\Vue\sample

11/24/2017  10:59 AM    <DIR>          .
11/24/2017  10:59 AM    <DIR>          ..
11/24/2017  10:59 AM               269 .babelrc
11/24/2017  10:59 AM               147 .editorconfig
11/24/2017  10:59 AM                51 .eslintignore
11/24/2017  10:59 AM               627 .eslintrc.js
11/24/2017  10:59 AM               213 .gitignore
11/24/2017  10:59 AM               223 .postcssrc.js
11/24/2017  10:59 AM    <DIR>          build
11/24/2017  10:59 AM    <DIR>          config
11/24/2017  10:59 AM               268 index.html
11/24/2017  10:59 AM             2,561 package.json
11/24/2017  10:59 AM               549 README.md
11/24/2017  10:59 AM    <DIR>          src
11/24/2017  10:59 AM    <DIR>          static
11/24/2017  10:59 AM    <DIR>          test
               9 File(s)          4,908 bytes
               7 Dir(s)  187,680,985,088 bytes free
```

Run `yarn install` to download dependencies and get project ready for development and testing.

Below are commands that are available:

* `yarn dev` or `yarn start` will start vue-loader and can access it using [http://localhost:8080](http://localhost:8080)
* `yarn unit` will run the unit test cases and will display code coverage
* `yarn e2e` will run end-2-end automation test suite - TODO
* `yarn build` will build production deployment project structure

```bash
yarn run v1.1.0
$ node build/build.js
Hash: decafbb41b162d5a062b
Version: webpack 3.8.1
Time: 24297ms
                                                  Asset       Size  Chunks             Chunk Names
               static/js/vendor.7a500e2803f3ee04c53e.js     120 kB       0  [emitted]  vendor
                  static/js/app.936bb6172fb0431042aa.js    11.5 kB       1  [emitted]  app
             static/js/manifest.cd73ec71b99a6df7c14e.js    1.49 kB       2  [emitted]  manifest
    static/css/app.bf9a994c72151daa5e919b0f3ccdc900.css  432 bytes       1  [emitted]  app
static/css/app.bf9a994c72151daa5e919b0f3ccdc900.css.map  828 bytes          [emitted]
           static/js/vendor.7a500e2803f3ee04c53e.js.map     971 kB       0  [emitted]  vendor
              static/js/app.936bb6172fb0431042aa.js.map    37.9 kB       1  [emitted]  app
         static/js/manifest.cd73ec71b99a6df7c14e.js.map    14.2 kB       2  [emitted]  manifest
                                             index.html  508 bytes          [emitted]

  Build complete.

  Tip: built files are meant to be served over an HTTP server.
  Opening index.html over file:// won't work.

Done in 41.93s.
```

## Install Visual Studio Code Extension

Developing UI based projects in Visual Studio Code is fun and easy. Its lightweight and has plugin based architecture build on top of Github's Atom.

Install extension `Vetur` . This provides auto-completion, debugging, error-checking, linting, snipperts, syntax-highlighting and many more.

Run `code .` in the sample folder to open Visual Studio Code and load the project structure by default. Install the extension by clicking `Ctrl+P` on Windows or `Command+P` on Mac and run command `ext install vetur`. Click on `Install` which will start installing the extension. Wait for sometime for it to be downloaded and installed.

## Install Browser Extension



---

**Recommended Readings**

* [https://www.gitbook.com/book/frontendmasters/front-end-handbook](https://www.gitbook.com/book/frontendmasters/front-end-handbook)

---

**Download a .pdf, .epub, or .mobi file from**:

* [https://www.gitbook.com/book/frontendmasters/front-end-handbook/details](https://www.gitbook.com/book/frontendmasters/front-end-handbook/details)

---

[![](https://i.creativecommons.org/l/by-nc-nd/3.0/88x31.png)](http://creativecommons.org/licenses/by-nc-nd/3.0/)  
This work is licensed under a[Creative Commons Attribution-NonCommercial-NoDerivs 3.0 Unported License](http://creativecommons.org/licenses/by-nc-nd/3.0/).

