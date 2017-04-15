# @citycide/cz-conventional &middot; [![Version](https://img.shields.io/npm/v/@citycide/cz-conventional.svg?style=flat-square&maxAge=3600)](https://www.npmjs.com/package/@citycide/cz-conventional) [![License](https://img.shields.io/npm/l/@citycide/cz-conventional.svg?style=flat-square&maxAge=3600)](https://www.npmjs.com/package/@citycide/cz-conventional) [![LightScript](https://img.shields.io/badge/written%20in-lightscript-00a99d.svg?flat-square)](http://www.lightscript.org)

> Personalized commitizen adapter based on Angular's conventional standard.

This adapter is basically a rewrite of the official `cz-conventional-changelog`
adapter. The main differences ( and benefits ) are:

- Add `[ci skip]` automatically for `docs` and `chore` types
- Change max line width to the more standard 72 ( from 100 )
- Cut dependencies down from 6 to 2

## installation

```console
npm i -D @citycide/cz-conventional
```

You'll also need commitizen:

```console
npm i -D commitizen

# or, global installation
npm i -g commitzen
```

## usage

See ["Making your repo Commitizen-friendly"][cz-help1] and
["Using the command line tool"][cz-help2] on the commitizen cli repo
for detailed instructions.

To easily set up your own repo with this adapter, you can use:

```console
commitizen init @citycide/cz-conventional --save-dev
```

## see also

- [LightScript][lightscript] - the compile-to-JS language this adapter is written in, leveraging [Babel][babel]
- [babel-plugin-partial-application][babel-plugin] - partial application syntax for JS using `_` like Scala & Kotlin
- [commitizen][commitizen] - the cli utility this adapter is built for

## contributing

Pull requests and any [issues](https://github.com/citycide/cz-conventional/issues)
found are always welcome.

1. Fork the project, and preferably create a branch named something like `feat-make-better`
2. Modify as needed, `src/index.lsc` being the source file
3. Push & pull request! :tada:

## license

MIT © [Bo Lingen / citycide](https://github.com/citycide)

[lightscript]: http://www.lightscript.org
[babel]: https://babeljs.io
[babel-plugin]: https://github.com/citycide/babel-plugin-partial-application
[commitizen]: https://github.com/commitizen/cz-cli
[cz-help1]: https://github.com/commitizen/cz-cli#making-your-repo-commitizen-friendly
[cz-help2]: https://github.com/commitizen/cz-cli#using-the-command-line-tool