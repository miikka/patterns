# Python

## Project management

Use [uv](https://github.com/astral-sh/uv) unless you need a full-powered build system.

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

Follow [PEP8][pep8]. Use [ruff] to both format and lint.

[pep8]: https://www.python.org/dev/peps/pep-0008/
[ruff]: https://github.com/astral-sh/ruff

## Default library and tool choices

Unless there's a good reason to use something else, I use these:

* Command-line parsing: [argparse](https://docs.python.org/3/library/argparse.html)
* HTTP client: [httpx2](https://github.com/pydantic/httpx2)
* Property-based testing: [Hypothesis](http://hypothesis.readthedocs.org)
* Test runner: [pytest](http://pytest.org/)
