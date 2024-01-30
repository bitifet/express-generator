# ExpressGen TO-DO List


## Improvements

### New Name

Even my original goal was just adding support for
[esmrouter](https://www.npmjs.com/package/esmrouter) I finally expanded my
goals to make a wider upgrade to this wonderful (but highly outdated) tool.

Since express-generator2 and 3 are already taken, adding an
"express-generator4" to the list wouldn't make much sense.

So I finally decided to call it 'expressgen' which will also be more handy for
using through npx so that instead of `npm install -g expressgen && expressgen`
we could just execute `npx expressgen`.

This change involves:

  * Updating package.json changing the package name and updating the *bin*
    section.

  * Update README.md to document usage through npx.

### Incorporate nodemon

  * (Idea borrowed from [TheOfficialDev-ops'
    fork](https://github.com/TheOfficialDev-ops/express-generator3) of
    express-generator).


## Upgrades

### Move to Pug

  * Make pug its default template engine.

  * Definitely deprecate Jade.
    - Since its only the precursor of pug there is no reason to use it in new
      projects.

### Upgrade coding styles

  * Begin migration to modern variable declarations (const, let...) where
    applicable.

### Upgrade other optional libs

  * Just to provide newer versions (I'll only check existing tests keep
    passing).

