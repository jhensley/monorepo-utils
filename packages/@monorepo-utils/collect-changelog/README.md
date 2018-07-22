# collect-changelog-from-tag

Collect CHANGELOG from tags.

## Feature

- Support independent mode
    - Currently it support [Independent mode](https://github.com/lerna/lerna#independent-mode---independent) only
- Get CHANGELOG from each package's `CHANGELOG.md`

## Install

Install with [npm](https://www.npmjs.com/):

    npm install @monorepo-utils/collect-changelog

## Usage

    Usage
      $ monorepo-utils-collect-changelog [option] "tag@version"

    Options
      --directory the root directory of monorepo

    Examples
      $ monorepo-utils-collect-changelog --directory /path/to/monorepo-project/ "tag@version"
      # current directory is project root
      $ monorepo-utils-collect-changelog "tag@version"

## Example

    $ monorepo-utils-collect-changelog "textlint@8.0.0"
    
    ## textlint@8.0.0
    
    ### fixes
    
    - **babel:** ignore lib directory ([12e581d](https://github.com/textlint/textlint/commit/12e581d))
    - **fixer:** fix thrown error when empty result. (#274) ([7013cee](https://github.com/textlint/textlint/commit/7013cee)), closes [#274](https://github.com/textlint/textlint/issues/274)
    - **textilnt:** fix JSDoc ([8a417e0](https://github.com/textlint/textlint/commit/8a417e0))
    
    ### features
    
    - **packages:** import textlint-plugin-text ([1b7a571](https://github.com/textlint/textlint/commit/1b7a571))
    - **textlint:** update built-in textlint-plugin-markdown@^2 (#282) ([448fef9](https://github.com/textlint/textlint/commit/448fef9))
    
    ### breakingChanges
    
    - **textlint:** markdown-to-ast@4 includes some breaking change


## Author

- [github/azu](https://github.com/azu)
- [twitter/azu_re](https://twitter.com/azu_re)

## License

MIT © azu