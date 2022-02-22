# Presentations

This repository hosts presentations made using the reveal-js framework. [Presentations]
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

[presentations]: https://github.com/engeir/presentations
