{% set is_open_source = cookiecutter.open_source_license != 'Not open source' -%}
{% for _ in cookiecutter.project_name %}={% endfor %}
{{ cookiecutter.project_name }}
{% for _ in cookiecutter.project_name %}={% endfor %}

.. image:: https://img.shields.io/pypi/v/{{ cookiecutter.project_name }}.svg
        :target: https://pypi.org/project/{{ cookiecutter.project_name }}
.. image:: https://github.com/{{ cookiecutter.github_username }}/{{ cookiecutter.project_name }}/actions/workflows/tests.yml/badge.svg
        :target: https://github.com/{{ cookiecutter.github_username }}/{{ cookiecutter.project_name }}/actions
.. image:: https://github.com/{{ cookiecutter.github_username }}/{{ cookiecutter.project_name }}/actions/workflows/docs.yml/badge.svg
        :target: https://{{ cookiecutter.github_username }}.github.io/{{ cookiecutter.project_name }}
{% if cookiecutter.add_pyup_badge == 'y' %}
.. image:: https://pyup.io/repos/github/{{ cookiecutter.github_username }}/{{ cookiecutter.project_name }}/shield.svg
        :target: https://pyup.io/repos/github/{{ cookiecutter.github_username }}/{{ cookiecutter.project_name }}/
{% endif %}


{{ cookiecutter.project_short_description }}

{% if is_open_source %}
Documentation: https://{{ cookiecutter.github_username }}.github.io/{{ cookiecutter.project_name }}.
{% endif %}

Features
--------

* TODO

