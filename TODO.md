# xprgen TO-DO List

## Improvements

### New Name

Even my original goal was just adding support for
[esmrouter](https://www.npmjs.com/package/esmrouter) I finally expanded my
goals to make a wider upgrade to this wonderful (but highly outdated) tool.

Since express-generator2 and 3 are already taken, adding an
"express-generator4" to the list wouldn't make much sense.

So I finally decided to call it 'xprgen' which will also be more handy for
using through npx so that instead of `npm install -g xprgen && xprgen`
we could just execute `npx xprgen`.

This change involves:

  * [x] Updating package.json changing the package name and updating the *bin*
    section.

  * [x] Update README.md to document usage through npx.

### Incorporate nodemon

  * [x] (Idea borrowed from [TheOfficialDev-ops'
    fork](https://github.com/TheOfficialDev-ops/express-generator3) of
    express-generator).


## Upgrades

### Move to Pug

  * [x] Make pug its default template engine.

  * [ ] Definitely deprecate Jade.
    - Since its only the precursor of pug there is no reason to use it in new
      projects.

### Upgrade coding styles

  * [ ] Begin migration to modern variable declarations (const, let...) where
    applicable.

### Upgrade other optional libs

  * [ ] Just to provide newer versions (I'll only check existing tests keep
    passing).

