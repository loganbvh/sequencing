# Contributing

Contributions are welcome, and they are greatly appreciated!

## Code of Conduct

Everyone interacting in the `sequencing` project's code base,
issue tracker, and any communication channels is expected to follow the
[PyPA Code of Conduct](https://www.pypa.io/en/latest/code-of-conduct/).


## Reporting Bugs

Report bugs [by creating an issue](https://docs.github.com/en/github/managing-your-work-on-github/creating-an-issue).

When reporting a bug, please include:

* Your operating system name and version.
* Any details about your local setup that might be helpful in troubleshooting.
* Detailed steps to reproduce the bug.


## Submitting Feedback

The best way to send feedback is to [create an issue](https://docs.github.com/en/github/managing-your-work-on-github/creating-an-issue).

If you are proposing a feature:

* Explain in detail how it would work and why it is important.
* Keep the scope as narrow as possible, to make it easier to implement.
* Remember that this is a volunteer-driven project, and that contributions
  are welcome.


## Pull Request Guidelines

Pull requests are the best way to propose changes to the `sequencing` codebase, and we actively welcome them.
All pull requests should abide by the following guidelines:

1. All code must be compatible with [Black code style](https://black.readthedocs.io/en/stable/)
(a subset of [PEP 8](https://www.python.org/dev/peps/pep-0008/)).
We recommend using [Black](https://black.readthedocs.io/en/stable/) and [flake8](https://flake8.pycqa.org/en/latest/) locally to ensure compatibility. (See [.flake8](.flake8) for the recommended flake8 configuration.)
2. If you've added code that should be tested, add tests.
3. If you've changed APIs (e.g. function signatures), update the documentation accordingly.
    - If your pull request adds new features, please consider creating an example Jupyter notebook demonstrating the features.
4. Ensure that all tests pass locally before creating the PR.


## Getting Started

Ready to contribute? Follow [GitHub best practices](https://www.asmeurer.com/git-workflow/) - in short:

1. Clone the repository.
2. Fork the repo on GitHub to your personal account.
3. Add your fork as a remote.
4. Pull the latest changes from the `main` branch.
5. Create a topic branch, e.g. `feature/short-description` for a feature or enhancement.
6. Make your changes and commit them (testing locally).
7. Push changes to the topic branch on *your* remote once local tests pass and you are happy with the changes you've made.
8. Create a pull request against the base `main` branch through the Github website.

## Making the Docs

Make an HTML version of the documentation.

> **Note**: This might require installing [Pandoc](https://pandoc.org/installing.html).

```
pip install sphinx sphinx_rtd_theme nbsphinx
cd docs
make html
```

## Unit Tests

Run all of the unit tests from a Python session using

``` python
>>> import sequencing.testing as st
>>> st.run()
```

Or run them from the command line, using

```
pytest --cov
```
