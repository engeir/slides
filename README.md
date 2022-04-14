# Presentations

This repository hosts presentations made using the [reveal.js] framework.
[Presentations] stores other kinds of presentations, plus images and videos since
I don't want them here. This is really just markdown files rendered in a nice way.

## Usage

### Fork

It should be quite straight forward to use this for your own presentations. Just [fork
the repo] and make some new markdown files, preferably on the format
`YYYY-MM-DD-title.md`.

### Install

Installing all dependencies is done with

```sh
npm install
```

### Run locally

You can start a locally hosted site that will be available at
[http://localhost:1948](http://localhost:1948) with

```sh
npm run start
```

### Publish

Pushing to GitHub will run a workflow that places the static site in the root of the
`gh-pages` branch.

If you for some reason want to build it manually, you can, with

```sh
npm run build
```

This will put the static site in the `docs` directory.

## Plugins

In addition to the default plugins provided by [reveal-md], the following plugins are
included in this project:

- [reveal.js-elapsed-time-bar]

  The timer is triggered by setting

  ```yaml
  revealOptions:
    allottedTime: 900000
  ```

  in the YAML front matter, where time is in seconds.

- [revealjs-animated]

- [reveal.js-copycode]

- [reveal-drawer]

- [reveal-pointer]

## Project specifics

This project makes a few changes to the original packages [reveal.js] and [reveal-md].
These patches are made using the [patch-package] module:

```sh
npx patch-package reveal-md
npx patch-package reveal.js
```

Thus, if you want further changes from this project or other modules, this is done
simply by changing the source files and running `npx patch-package some-package`.

[fork the repo]: https://github.com/engeir/slides/fork
[patch-package]: https://www.npmjs.com/package/patch-package
[presentations]: https://github.com/engeir/presentations
[reveal-drawer]: https://github.com/burnpiro/reveal-drawer
[reveal-md]: https://github.com/webpro/reveal-md
[reveal-pointer]: https://github.com/burnpiro/reveal-pointer
[reveal.js-copycode]: https://github.com/Martinomagnifico/reveal.js-copycode
[reveal.js-elapsed-time-bar]: https://github.com/tkrkt/reveal.js-elapsed-time-bar
[reveal.js]: https://revealjs.com
[revealjs-animated]: https://github.com/rogeralmeida/revealjs-animated
