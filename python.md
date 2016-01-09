# Python

Default to Python 3.


## Logging

Use the standard library [logging][logging] module. In each module, initialize
a module-level logger like this:

    import logging
    log = logging.getLogger(__name__)
    log.addHandler(logging.NullHandler())

In the main program, configure logging like this:

    logging.basicConfig(level=logging.INFO)

[logging]: https://docs.python.org/2/library/logging.html


## Style and linting

Follow [PEP8][pep8]. Use [autopep8][autopep8] to automatically format it.
Always use [flake8][flake8], but feel free to ignore the McCabe checks.

[pep8]: https://www.python.org/dev/peps/pep-0008/
[flake8]: https://pypi.python.org/pypi/flake8
[autopep8]: https://pypi.python.org/pypi/autopep8
