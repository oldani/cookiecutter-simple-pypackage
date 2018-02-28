{% set is_open_source = cookiecutter.open_source_license != 'Not open source' -%}
{% for _ in cookiecutter.project_name %}={% endfor %}
{{ cookiecutter.project_name }}
{% for _ in cookiecutter.project_name %}={% endfor %}

{% if is_open_source %}
[![Pypi link](https://img.shields.io/pypi/v/{{ cookiecutter.project_slug }}.svg)](https://pypi.python.org/pypi/{{ cookiecutter.project_slug }})
[![Travis job](https://img.shields.io/travis/{{ cookiecutter.github_username }}/{{ cookiecutter.project_slug }}.svg)](https://travis-ci.org/{{ cookiecutter.github_username }}/{{ cookiecutter.project_slug }})

{%- endif %}

{% if cookiecutter.add_pyup_badge == 'y' %}
[![Pyup](https://pyup.io/repos/github/{{ cookiecutter.github_username }}/{{ cookiecutter.project_slug }}/shield.svg)](https://pyup.io/repos/github/{{ cookiecutter.github_username }}/{{ cookiecutter.project_slug }}/)
{% endif %}


{{ cookiecutter.project_short_description }}

## Table of Content:

- [Intallation](#installation)
- [Usage](#usage)
- [TODO](#todo)
- [Contributing](#contributing)
- [Credits](#credits)

## Installation


```batch

    $ pip install {{ cookiecutter.project_slug }}
```

This is the preferred method to install {{ cookiecutter.project_name }}, as it will always
install the most recent stable release.

If you don't have [pip](https://pip.pypa.io) installed, this 
[Python installation guide](http://docs.python-guide.org/en/latest/starting/installation/) 
can guide you through the process.

## Usage

--


## TODO

- [ ] Add Test


## Contributing

Contributions are welcome, and they are greatly appreciated! Every
little bit helps, and credit will always be given.

For more info please click [here](./CONTRIBUTING.md)


## Credits

This package was created with Cookiecutter and the `oldani/cookiecutter-simple-pypackage` project template.

- [Cookiecutter](https://github.com/audreyr/cookiecutter)
- [oldani/cookiecutter-simple-pypackage](https://github.com/oldani/cookiecutter-simple-pypackage)
