# Contributing


Contributions are welcome, and they are greatly appreciated! Every
little bit helps, and credit will always be given.

You can contribute in many ways:

## Types of Contributions

### Report Bugs

Report bugs at https://github.com/tulsawebdevs/tulsawebdevs.org/issues.

If you are reporting a bug, please include:

* Your operating system name and version.
* Any details about your local setup that might be helpful in troubleshooting.
* Detailed steps to reproduce the bug.

### Fix Bugs

Look through the GitHub issues for bugs. Anything tagged with "[bug](https://github.com/tulsawebdevs/tulsawebdevs.org/labels/bug)"
is open to whoever wants to implement it.

### Implement Features

Look through the GitHub issues for features. Anything tagged with "[feature](https://github.com/tulsawebdevs/tulsawebdevs.org/labels/feature)"
is open to whoever wants to implement it.

### Write Documentation

tulsawebdevs.org could always use more documentation, whether as
part of the official Tulsa Web Devs docs, in docstrings, or
even on the web in blog posts, articles, and such.

### Submit Feedback

The best way to send feedback is to file an issue at
https://github.com/tulsawebdevs/tulsawebdevs.org/issues.

If you are proposing a feature:

* Explain in detail how it would work.
* Keep the scope as narrow as possible, to make it easier to implement.
* Remember that this is a volunteer-driven project, and that contributions
  are welcome :)

## Get Started!

Ready to contribute? Here's how to set up tulsawebdevs.org
for local development.

1. Fork the `tulsawebdevs.org` repo on GitHub.
2. Clone your fork locally:

   ```bash
   $ git clone git@github.com:your_name_here/tulsawebdevs.org.git
   ```

3. Install your local copy into a virtualenv. Assuming you have
   virtualenvwrapper installed, this is how you set up your fork for local
   development:
   
   ```bash
   $ mkvirtualenv tulsawebdevs.org
   $ cd tulsawebdevs.org/
   $ pip install -r requirements.txt -r requirements-dev.txt
   $ ./manage.py syncdb
   ```

4. Create a branch for local development:

   ```bash
   $ git checkout -b name-of-your-bugfix-or-feature
   ```

   Now you can make your changes locally.

5. When you're done making changes, check that your changes pass flake8 and the
   tests, including testing other Python versions with tox::

   ```bash
   $ make qa-all
   ```

   To get flake8 and tox, just pip install them into your virtualenv.

6. Commit your changes and push your branch to GitHub:

   ```bash
   $ git add .
   $ git commit -m "Your detailed description of your changes."
   $ git push origin name-of-your-bugfix-or-feature
   ```

7. Submit a pull request through the GitHub website.

## Pull Request Guidelines

Before you submit a pull request, check that it meets these guidelines:

1. The pull request should include tests.
2. If the pull request adds functionality, the docs should be updated. Put
   your new functionality into a function with a docstring, and add the
   feature to the list in README.rst.
3. The pull request should work for Python 2.7, 3.3, and 3.4, and for PyPy. Check
   https://travis-ci.org/tulsawebdevs/tulsawebdevs.org/pull_requests
   and make sure that the tests pass for all supported Python versions.

## Tips

To run a subset of tests:
```bash
$ ./manage.py test events/tests/test_views.py
```

To mark failed tests:
```bash
$ ./manage.py test --failed
```

To re-run only the failed tests:
```bash
$ ./manage.py test --failed
```