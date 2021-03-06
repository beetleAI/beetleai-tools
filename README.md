# BeetlAI Softwares

## Project pre-requisites

The prerequisite for running our software is to have NodeJS and Git, Chrome and Mozilla browsers installed on your machine.

### Hardware Requirements:
```
Operating System : Windows/Mac/Linux
The application development requires at least 4GB of RAM to run efficiently in any the above OS.
```
### Tools Requirements

1. Install [Visual Studio Code](https://code.visualstudio.com/Download) (VS code) IDE to develop the code
2. Install [Atom](https://atom.io/) tool
3. Install [GIT client](https://git-scm.com/download/gui/windows)
4. Install [Draw.io ](https://app.diagrams.net/) to design tool for sfotware architecture diagrams.
5. Install [notepad ++](https://notepad-plus-plus.org/downloads/v7.8.1/), a light weight editor

### Install nodeJS and NPM latest stable versions  

Install [NodeJS](https://nodejs.org/en/) which install npm too.


### Install VueJS node module using npm tool.

```bash
C:\Users\cpm\AI>npm install --global vue-cli
npm WARN deprecated vue-cli@2.9.6: This package has been deprecated in favour of @vue/cli
npm WARN deprecated coffee-script@1.12.7: CoffeeScript on NPM has moved to "coffeescript" (no hyphen)
C:\Users\cpm\AppData\Roaming\npm\vue-list -> C:\Users\cpm\AppData\Roaming\npm\node_modules\vue-cli\bin\vue-list
C:\Users\cpm\AppData\Roaming\npm\vue -> C:\Users\cpm\AppData\Roaming\npm\node_modules\vue-cli\bin\vue
C:\Users\cpm\AppData\Roaming\npm\vue-init -> C:\Users\cpm\AppData\Roaming\npm\node_modules\vue-cli\bin\vue-init
+ vue-cli@2.9.6
updated 1 package in 246.719s
```

### Now, How to create vuejs project using VUE CLI

```bash
vue init webpack AI-LAB

? Project name ailab
? Project description A Vue.js project
? Author PurushothamCheekuru <cheekuru.cvshp@gmail.com>
? Vue build standalone
? Install vue-router? Yes
? Use ESLint to lint your code? Yes
? Pick an ESLint preset Standard
? Set up unit tests No
? Setup e2e tests with Nightwatch? Yes
? Should we run `npm install` for you after the project has been created? (recommended) npm

   vue-cli · Generated "AILAB".
```

### How to run VUE application

```bash
C:\Users\cpm\AI>cd AILAB
C:\Users\cpm\AI\AILAB>npm run dev
```

----------------------
## How to Document your software faster?

Markdown is a utility tool to [Make a README](https://www.makeareadme.com/) for building software documentation easy.

### Prerequisite

Browse nodeJS installation [instructions](https://nodejs.org/en/download/) for your specific OS.

```bash
$ npm install --save-dev marked
```

### Steps to build project

To compile the markdown to HTML and write it to a new README.html file. Create a README.md with sample markdown content and  JS script file ```generateReadMe.js```.

```javascript
var marked = require('marked');
var fs = require('fs');

var readMe = fs.readFileSync('README.md', 'utf-8');
var markdownReadMe = marked(readMe);

fs.writeFileSync('./site/README.html', markdownReadMe);
```

### Edit index.html
Create a index.html and add the following HTML object where the README.md content should be displayed
```html
<object data="README.html" type="text/html"></object>
```

### Generate md files
Then run this on the command line to make it happen:
```bash
$ node path/to/generateReadMe.js
```

----------------------------------------------------------


## AI LAB

> A Vue.js project

### Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report

# run e2e tests
npm run e2e

# run all tests
npm test
```
### How to debug VueJS apps

Install and enable [VueJS Devtools](https://flaviocopes.com/vue-devtools/)  Chrome extension.

For a detailed explanation on how things work, check out the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).
