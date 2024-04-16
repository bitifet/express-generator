[![Express Logo](https://i.cloudup.com/zfY6lL7eFa-3000x3000.png)](http://expressjs.com/)

**Updated** [Express'](https://www.npmjs.com/package/express) application generator.

👉 [Up to date](#dev-notes) *express-generator* with [new features](#new-features).

[![NPM Version][npm-image]][npm-url]
[![NPM Downloads][downloads-image]][downloads-url]
[![Linux Build][github-actions-ci-image]][github-actions-ci-url]
[![Windows Build][appveyor-image]][appveyor-url]

<!-- (Syntax highlighting issue breaker (Sorry)) []() -->


> 📌 This is a modified version of [Express
> Generator](https://github.com/expressjs/generator) which is nowadays highly
> outdated.
> 
> For more details see [Dev Notes](#dev-notes) below...

## New features

  * 👉 SaSS css engine works again (even with latest Node.js versions).
  * 👉 Includes nodemon to monitorize changes (`npm run dev`).
  * 👉 Uses [Pug](https://pugjs.org) (instead of legacy Jade) templating engine by default.
  * 👉 Up-to-date versions of all dependencies.
  * 👉 Support for [ESMrouter](https://www.npmjs.com/package/esmrouter)
    (`--esmr` flag) to transparently make available [browser-enabled NPM
    packages](https://docs.npmjs.com/cli/v10/configuring-npm/package-json#browser)
    client side.
  * 👉 Even easier usage: Ex.: `npx xprgen --esmr -c sass myApp` (Create an
    Express App with [Pug](https://pugjs.org), [SaSS](https://sass-lang.com/)
    and [ESMrouter](https://www.npmjs.com/package/esmrouter).
  * 👉 Dependencies preinstallation. Ex: `npx xprgen --esmr -i smarkform myApp`.
    - Even for multiple packages. Ex: `npx xprgen --esmr -i "smarkform sqltt chalk" myApp`.
    - Also possible with devDependencies. Ex: `npx xprgen -i sqltt -d mocha`.
    - Guesses version as current 'latest' tag prefixed whith caret (likewise `npm install`).
    - ...but can be overridden. Ex: `npx xprgen -i "node-sass@^4.1.0"`.



## Quick Start

The quickest way to get started with express is to utilize the executable
`xprgen` through [npx](https://www.npmjs.com/package/npx) to generate an
application as shown below:


> 📌 **Installation**
> 
> If you prefer, you can install it locally using the following command:
> 
> ```sh
> $ npm install -g xprgen
> ```
> 
> To execute it locally, you'll have to omit the initial `npx` command at the
> beginning of the following sentences.


Create the app:

```bash
$ npx xprgen /tmp/foo && cd /tmp/foo
```

Install dependencies:

```bash
$ npm install
```

Start your Express.js app at `http://localhost:3000/`:

```bash
$ npm start
```

Or alternatively, to make it to restart every time a file is changed:

```bash
$ npm run dev
```

## Command Line Options

This generator can also be further configured with the following command line flags.

```
        --version           output the version number
    -e, --ejs               add ejs engine support
        --pug               add pug engine support
        --hbs               add handlebars engine support
    -H, --hogan             add hogan.js engine support
    -v, --view <engine>     add view <engine> support (dust|ejs|hbs|hjs|jade|pug|twig|vash) (defaults to pug)
        --no-view           use static html instead of view engine
    -c, --css <engine>      add stylesheet <engine> support (less|stylus|compass|sass) (defaults to plain css)
        --esmr              add esmrouter (make browser-enabled npm packages available client side)
        --git               add .gitignore
    -i  --install <pkgs>    add specified pkgs as dependencies. Can be specified multiple times or as space-separated string. Accept optional @version spec.
    -d  --devInstall <pkgs> like --install but for devDependencies
    -f, --force             force on non-empty directory
    -h, --help              output usage information
```

## Dev Notes

There are already several forks of it out there.

The aim (or one of its) of this new fork is to catch the attention of the other
forks authors in order to join our efforts in a single package.

> 📌 **If you are the author of one of these forks (or plan to create a new one),
> PLEASE contact me and I'll give you access to this repository.**
> 
> I'm not an experienced maintainer neither have a lot of time to invest in it.
> But hopefully we could keep this useful tool more updated.

### Name change

To break the "express-generatorX" sequence, I renamed it 'xprgen' which, in
turn, will be more handy to be used as 'npx xprgen'.

### Goals

Additionally to those already implemented (see [New features](#new-features)
section), you can find my inital goals in the [TO-DO List](./TODO.md) I added
to the project.

Please feel free to suggest/add your own ones.

### Versioning

Last but not least...

As we've done several breaking changes (and also to avoid confussion with
original express-generator's versions (and possible reviews in case they
happen), I'll start versioning from next major number (5.0.0) and so on...


## License

[MIT](LICENSE)

[npm-image]: https://img.shields.io/npm/v/xprgen.svg
[npm-url]: https://npmjs.org/package/xprgen
[appveyor-image]: https://img.shields.io/appveyor/ci/dougwilson/generator/master.svg?label=windows
[appveyor-url]: https://ci.appveyor.com/project/dougwilson/generator
[downloads-image]: https://img.shields.io/npm/dm/xprgen.svg
[downloads-url]: https://npmjs.org/package/xprgen
[github-actions-ci-image]: https://img.shields.io/github/workflow/status/expressjs/generator/ci/master?label=linux
[github-actions-ci-url]: https://github.com/expressjs/generator/actions/workflows/ci.yml
