# Awesome Codemods

A curated list of tools that don't just point out what needs to be done
(like static code analyzers or linters) but actually modify your code. This means
they can e.g. be used in pre-commit scripts or with tools like
[silver-platter](https://github.com/jelmer/silver-platter).

Code formatters are intentionally excluded here but can be found in
https://github.com/rishirdua/awesome-code-formatters.

## By Environment

[**General**](#general)
[**JavaScript/TypeScript**](#javascripttypescript)
[**Python**](#python)
[**PHP**](#php)
[**C/C++**](#cc)
[**C#**](#c)
[**Go**](#go)
[**Ruby**](#ruby)
[**Debian**](#debian)

### General

1. [codespell](https://github.com/codespell-project/codespell) -  check code for common misspellings

### JavaScript/TypeScript

1. [**jscodeshift**](https://github.com/facebook/jscodeshift) - toolkit for running codemods over multiple JavaScript or TypeScript files
2. [**ts-morph**](https://github.com/dsherret/ts-morph) - TypeScript Compiler API wrapper for programmatic code changes
3. [**react-codemod**](https://github.com/reactjs/react-codemod) - codemod scripts to update React APIs
4. [**next-codemod**](https://github.com/vercel/next-codemod) - codemod transformations for upgrading Next.js codebases
5. [**ember-codemods**](https://github.com/ember-codemods) - collection of codemods for Ember.js
6. [**vue-codemods**](https://github.com/SergioCrisostomo/vue-codemods) - codemod scripts to update and refactor Vue files
7. [**angular-codemods**](https://github.com/arthurflachs/angular-codemods) - codemods for refactoring Angular applications
8. [**@mui/codemod**](https://github.com/mui/material-ui/tree/master/packages/mui-codemod) - codemods for upgrading Material UI versions
9. [**eslint-transforms**](https://github.com/eslint/eslint-transforms) - codemods for the ESLint ecosystem
10. [**jest-codemods**](https://github.com/skovhus/jest-codemods) - codemods for migrating test frameworks to Jest
11. [**5to6-codemod**](https://github.com/5to6/5to6-codemod) - transform ES5 code to ES6
12. [**lebab**](https://github.com/lebab/lebab) - transform ES5 code to modern JavaScript
13. [**js-codemod**](https://github.com/cpojer/js-codemod/) - codemod scripts to transform code to next generation JS

### Python

1. [**yesqa**](https://github.com/asottile/yesqa) - Remove unnecessary ``#noqa`` comments
2. [**pyupgrade**](https://github.com/asottile/pyupgrade) - upgrade syntax for newer versions of the language
3. [**reorder_python_imports**](https://github.com/asottile/reorder_python_imports) - automatically reorder imports
4. [**teyit**](https://github.com/isidentical/teyit) - use recommended style for assert statements
5. [**blacken-docs**](https://github.com/asottile/blacken-docs) - run black on code fragements in documentation
6. [**setup-py-upgrade**](https://github.com/asottile/setup-py-upgrade) - upgrade setup.py to new metadata syntax
7.  [**modernize**](https://github.com/pycqa/modernize) - modernize Python code for eventual Python 3 migration
8.  [**autoflake**](https://github.com/pycqa/autoflake) - remove unused imports and unused variables
9. [**ruff**](https://github.com/astral-sh/ruff) - ultra-fast linter that can also fix (some of the) issues it reports
10. [**django-codemod**](https://github.com/browniebroke/django-codemod) - automatically fix Django deprecations

### PHP

1. [**PHP-Codeshift**](https://github.com/Atanamo/PHP-Codeshift) - toolkit for running codemods over multiple PHP files
2. [**rector**](https://github.com/rectorphp/rector) - automated refactoring and upgrading of PHP code

### C/C++

1. [**uncrustify**](https://github.com/uncrustify/uncrustify) - Code formatting along flexible rules

### Go

1. [**golangci-lint**](https://golangci-lint.run/) - linter that can also fix (some of the) issues it reports

### Ruby

1. [**RuboCop**](https://github.com/rubocop/rubocop) - static code analyzer and formatter that can automatically fix many issues
2. [**codeshift**](https://github.com/rajasegar/codeshift) - jscodeshift equivalent for Ruby

### Rust

1. [**clippy**](https://github.com/rust-lang/rust-clippy) - linter that can also fix (some of the) issues it reports

### Debian

1. [**lintian-brush**](https://salsa.debian.org/jelmer/lintian-brush) - Fix issues reported by lintian
2. [**deb-scrub-obsolete**](https://salsa.debian.org/jelmer/lintian-brush) - Remove obsolete maintainer script / control file entries
3. [**apply-multiarch-hints**](https://salsa.debian.org/jelmer/lintian-brush) - Apply multi-arch fixes from https://multiarch.debian.net/
4. [**deb-new-upstream**](https://github.com/breezy-team/breezy) - Import new upstream releases or snapshots
5. [**cme**](https://packages.debian.org/cme) - Fix various common issues in Debian packages
6. [**drop-mia-uploaders**](https://salsa.debian.org/jelmer/debmutate) - Remove Missing-In-Action uploaders from Maintainer/Uploader fields

## Libraries/Tools for refactoring

1. [**Bowler**](https://github.com/facebookincubator/Bowler) - modern Python (deprecated, recommends libcst)
2. [**libcst**](https://github.com/instagram/libcst) - Python
3. [**rerast**](https://github.com/google/rerast) - transform Rust code using rules
4. [**refex**](https://github.com/ssbr/refex) - refactor expressions in Python
5. [**clang-libastmatcher**](https://clang.llvm.org/docs/LibASTMatchersTutorial.html#intermezzo-learn-ast-matcher-basics) - CLang AST Matchers
6. [**asttokens**](https://github.com/gristlabs/asttokens) - token-preserving AST library for Python
7. [**pasta**](https://github.com/google/pasta) - code rewriting for Python using AST mutation instead of string templates
8. [**putout**](https://github.com/coderaiser/putout) - pluggable JavaScript/TypeScript code transformer
9. [**riceburn**](https://github.com/kenotron/riceburn) - TypeScript, JSON, and text file codemod utility

## Tools for invoking codemods

1. [**pre-commit**](https://www.pre-commit.com/) - Run formatters during git pre-commit
2. [**silver-platter**](https://github.com/jelmer/silver-platter) - Run codemods against remote repositories and publish changes (creating PRs/pushing)
3. [**all-repos**](https://github.com/asottile/all-repos) - Run codemods across a set of local repositories
4. [**CodeshiftCommunity**](https://github.com/CodeshiftCommunity/CodeshiftCommunity) - Community-owned global registry for codemods

## Fix aggregators

1. [**routine-update**](https://salsa.debian.org/science-team/routine-update) - run various codemods for Debian packages
2. [**nitpick**](https://github.com/andreoliwa/nitpick) - Apply the same pre-defined settings across all your projects
3. [**mrm**](https://github.com/sapegin/mrm) - codemods for project config files

## Commercial Platforms

1. [**CodeFix**](https://www.devgraph.com/codefix/)

## Meta

See also the lists of:
- [awesome code formatters](https://github.com/rishirdua/awesome-code-formatters)
- [awesome AST](https://github.com/cowchimp/awesome-ast)
- [awesome jscodeshift](https://github.com/sejoker/awesome-jscodeshift)
- [awesome codemods](https://github.com/rajasegar/awesome-codemods) - JS/framework-focused list

**License**

This awesome list is licensed under the CC-0 license.
