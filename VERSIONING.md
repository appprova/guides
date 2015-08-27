# AppProva - Git and Versioning

Our workflow is based on `git-flow`, also we use SEMVER to our code versioning.

### Git flow

[git-flow](https://github.com/nvie/gitflow) are a set of git extensions to provide high-level repository operations for [Vincent Driessen's branching model](http://nvie.com/posts/a-successful-git-branching-model/).

[This](http://danielkummer.github.io/git-flow-cheatsheet/index.html) cheatsheet shows the basic usage and effect of git-flow operations.

We use the following configuration:

```
$ git flow init
```

- Branch name for production releases: `master`
- Branch name for "next release" development: `develop`
- Feature branches? `feature/`
- Release branches? `release/`
- Hotfix branches? `hotfix/`
- Support branches? `support/`
- Version tag prefix? `v`

### Versioning

We use [Semantic Versioning](http://semver.org/) to manage our releases. Given a version number MAJOR.MINOR.PATCH, increment the:

1. MAJOR version when you make incompatible API changes,
1. MINOR version when you add functionality in a backwards-compatible manner, and
1. PATCH version when you make backwards-compatible bug fixes.
1. Additional labels for pre-release and build metadata are available as extensions to the MAJOR.MINOR.PATCH format.

### Releases

Always when creating a new release, please add a descritive tag message to make easy to understand and track what is being delivered. Remember to always be very clear and assertive on that, please don't just copy commit messages.

```
Changelog v0.0.0

- Features
  - Here comes every feature added to this release
- Fixes
  - Here comes every bug fix;
- Others
  - Here comes code enhancement and other stuff like configurations, etc...
```
