# Presentations

This repository hosts presentations made using the [reveal-js] framework. [Presentations]
stores other kinds of presentations, plus images and videos since I don't want them here.
This is really just markdown files rendered in a nice way.

## Usage

### Fork

It should be quite straight forward to use this for your own presentations. Just fork the
repo and make some new markdown files, preferably on the format `YYYY-MM-DD-title.md`.

### Run locally

Run it locally with

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

This will put the static page in the `docs` directory.

## Plugins

In addition to the default plugins provided by [reveal-md], the following plugins are
included in this project:

- [spotlight]

  Turned off atm. Include by adding `"plugin/spotlight/spotlight.js",` to the file
  `reveal-md.json`.

- [elapsed-time-bar]

  The timer is triggered by setting

  ```yml
  revealOptions:
    allottedTime: 900000
  ```

  in the YAML front matter, where time is in seconds.

- [revealjs-animated]


[presentations]: https://github.com/engeir/presentations
[spotlight]: https://github.com/denniskniep/reveal.js-plugin-spotlight
[elapsed-time-bar]: https://github.com/tkrkt/reveal.js-elapsed-time-bar
[revealjs-animated]: https://github.com/rogeralmeida/revealjs-animated
[reveal-js]: https://revealjs.com
[reveal-md]: https://github.com/webpro/reveal-md
