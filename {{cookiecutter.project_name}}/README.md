{{cookiecutter.readable_name}}
{% for _ in cookiecutter.readable_name %}={% endfor %}

[![Build Status](../../actions/workflows/tests.yml/badge.svg)](../../actions/workflows/tests.yml)
[![Build Status](../../actions/workflows/lint.yml/badge.svg)](../../actions/workflows/lint.yml)

[![Supported Versions](https://img.shields.io/pypi/pyversions/{{cookiecutter.project_name}}.svg)](https://pypi.org/project/{{cookiecutter.project_name}})
[![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)

```
SCRIPT GOES HERE
```


Installation
------------
    pip install {{cookiecutter.project_name}}{% if cookiecutter.is_sub_package %}

or

    pip install screenpy[{{cookiecutter.project_name | replace("screenpy_", "")}}]{%- endif %}


Documentation
-------------
Please check out the [Read The Docs documentation](https://{{cookiecutter.project_name | replace("_", "-")}}-docs.readthedocs.io/en/latest/) for the latest information about this module!{% if cookiecutter.is_sub_package %}

You can also read the [ScreenPy Docs](https://screenpy-docs.readthedocs.io/en/latest/) for more information about ScreenPy in general.{%- endif %}


Contributing
------------
You want to contribute? Great! Here are the things you should do before submitting your PR:

1. Fork the repo and git clone your fork.
1. `dev` install the project package:
    1. `pip install -e .[dev]`
    1. Optional (poetry users):
        1. `poetry install --extras dev`
1. Run `tox` to perform tests frequently.
1. Create pull-request from your branch.

That's it! :)
