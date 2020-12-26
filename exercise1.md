# Language of choice: python

## CI tools setup for python?

For python, the most commonly used linter is `Flake8` which can also be used with other tools to enforce code style, e.g. `Black`. For testing, the built-in library `unittest` can help with, you guessed it, unit test. A simpler solution would be `pytest`. As development should happen in isolated directories, `tox` can automate the use of `virtualenv` as well as test. As for building, it is usually handled with built-in `setuptools` for distribution, the package of which can only be run by Python interpreter. For platform-specific distribution, one needs to use `py2exe` or `py2app`.

## Alternative CI setup other than Jenkins and Github Actions?

There are many popular CI alternatives, many of which have both local and cloud options. One successful example is `Travis-CI` that also operates in tandem with your existing Github repositories besides the default Github Actions. `Travis-CI` is widely integrated into many popular open-source software. Another option is `Gitlab CI` coming with `Gitlab`. Apart from using their terrific online version, a community version of their platform also exists to be deployed locally as well as the CI/CD system.

## Setup location? Self-hosted or cloud-based environment, reason, and influential factors?

For python applications, it would be reasonable to just use the cloud-based environment for CI and CD as `Python` is an interpreted language like `JavaScript`. The development process should be fast and quick to test and easy to integrate into current code. Another reason for opting in a cloud-based environment is that it may be easier to manage pull requests in a small-to-medium codebase with dozens of contributors. When deciding which one to use, other factors to be taken into consideration may be difficulty in setting up the building environment, potential build time, network and local-machine performances, and more.

