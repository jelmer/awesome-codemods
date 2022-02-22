# Awesome Code Fixers

A curated list of tools that don't just point out what needs to be done
(like static code analyzers or linters) but actually fix your code. This means
they can e.g. be used in pre-commit scripts or with tools like
[silver-platter](https://github.com/jelmer/silver-platter).

Code formatters are intentionally excluded here but can be found in
https://github.com/rishirdua/awesome-code-formatters.

## By Environment

[**Python**](#python)
[**C++**](#c++)
[**Go**](#go)
[**Debian**](#debian)

### Python

1. [**yesqa**](https://github.com/asottile/yesqa) - Remove unnecessary ``#noqa`` comments
2. [**pyupgrade**](https://github.com/asottile/pyupgrade) - upgrade syntax for newer versions of the language
3. [**reorder_python_imports**](https://github.com/asottile/reorder_python_imports) - automatically reorder imports
4. [**teyit**](https://github.com/isidentical/teyit) - use recommended style for assert statements
5. [**blacken-docs**](https://github.com/asottile/blacken-docs) - run black on code fragements in documentation
6. [**setup-py-upgrade**](https://github.com/asottile/setup-py-upgrade) - upgrade setup.py to new metadata syntax

### C++

### Go

### Debian

1. [**lintian-brush**](https://salsa.debian.org/jelmer/lintian-brush) - Fix issues reported by lintian
2. [**deb-scrub-obsolete**](https://salsa.debian.org/jelmer/lintian-brush) - Remove obsolete maintainer script / control file entries
3. [**apply-multiarch-hints**](https://salsa.debian.org/jelmer/lintian-brush) - Apply multi-arch fixes from https://multiarch.debian.net/
4. [**deb-new-upstream**](https://github.com/breezy-team/breezy) - Import new upstream releases or snapshots
5. [**cme**](https://packages.debian.org/cme) - Fix various common issues in Debian packages

## Libraries/Tools for refactoring

1. [**Bowler**](https://github.com/facebookincubator/Bowler) - modern Python
2. [**rerast**](https://github.com/google/rerast) - transform Rust code using rules

## Tools for invoking code fixers

1. [**pre-commit**](https://www.pre-commit.com/) - Run formatters during git pre-commit
2. [**silver-platter**](https://github.com/jelmer/silver-platter) - Run codefixers against remote repositories and publish changes (creating PRs/pushing)
3. [**all-repos**](https://github.com/asottile/all-repos) - Run fixers across a set of local repositories

## Fix aggregators

1. [**routine-update**](https://salsa.debian.org/science-team/routine-update) - run various code fixers for Debian packages

## Commercial Platforms

1. [**CodeFix**](https://www.devgraph.com/codefix/)

## Meta

See also the list of [awesome code formatters](https://github.com/rishirdua/awesome-code-formatters).

**License**

This awesome list is licensed under the CC-0 license.
