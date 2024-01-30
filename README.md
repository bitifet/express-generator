[![Express Logo](https://i.cloudup.com/zfY6lL7eFa-3000x3000.png)gen](http://expressjs.com/)

[Express'](https://www.npmjs.com/package/express) application generator.

[![NPM Version][npm-image]][npm-url]
[![NPM Downloads][downloads-image]][downloads-url]
[![Linux Build][github-actions-ci-image]][github-actions-ci-url]
[![Windows Build][appveyor-image]][appveyor-url]

<!-- (Syntax highlighting issue breaker (Sorry)) []() -->

## Dev Note

This is a modified version of [Express
Generator](https://github.com/express/generator) which is nowadays highly
outdated.

There are already several forks of it out there.

The aim (or one of its) of this new fork is to catch the attention of the other
forks authors in order to join our efforts in a single package.

> 📌 **If you are the author of one of these forks (or plan to create a new one),
> PLEASE contact me and I'll give you access to this repository.**
> 
> I'm not an experienced maintainer neither have a lot of time to invest in it.
> But hopefully we could keep this useful tool more updated.

### Name change

To break the "express-generatorX" sequence, I renamed it 'expressgen' which, in
turn, will be more handy to be used as 'npx expressgen'.

### Goals

You can find my inital goals in the [TO-DO List](./TODO.md) I added to the project.

Please feel free to suggest/add your own ones.


## Installation

```sh
$ npm install -g express-generator
```

## Quick Start

The quickest way to get started with express is to utilize the executable `express(1)` to generate an application as shown below:

Create the app:

```bash
$ express --view=hbs /tmp/foo && cd /tmp/foo
```

Install dependencies:

```bash
$ npm install
```

Start your Express.js app at `http://localhost:3000/`:

```bash
$ npm start
```

## Command Line Options

This generator can also be further configured with the following command line flags.

        --version        output the version number
    -e, --ejs            add ejs engine support
        --pug            add pug engine support
        --hbs            add handlebars engine support
    -H, --hogan          add hogan.js engine support
    -v, --view <engine>  add view <engine> support (dust|ejs|hbs|hjs|jade|pug|twig|vash) (defaults to jade)
        --no-view        use static html instead of view engine
    -c, --css <engine>   add stylesheet <engine> support (less|stylus|compass|sass) (defaults to plain css)
        --esmr           add esmrouter (make browser-enabled npm packages available client side)
        --git            add .gitignore
    -f, --force          force on non-empty directory
    -h, --help           output usage information

## License

[MIT](LICENSE)

[npm-image]: https://img.shields.io/npm/v/express-generator.svg
[npm-url]: https://npmjs.org/package/express-generator
[appveyor-image]: https://img.shields.io/appveyor/ci/dougwilson/generator/master.svg?label=windows
[appveyor-url]: https://ci.appveyor.com/project/dougwilson/generator
[downloads-image]: https://img.shields.io/npm/dm/express-generator.svg
[downloads-url]: https://npmjs.org/package/express-generator
[github-actions-ci-image]: https://img.shields.io/github/workflow/status/expressjs/generator/ci/master?label=linux
[github-actions-ci-url]: https://github.com/expressjs/generator/actions/workflows/ci.yml
