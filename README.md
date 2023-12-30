![Repository Banner](https://banners.beyondco.de/Cookiecutter%20for%20Ansible%20Role.png?theme=light&packageManager=&packageName=cookiecutter+gh%3Ageoffreyvanwyk%2Fcookiecutter-ansible-role&pattern=architect&style=style_1&description=All+you+need+to+start+automating%21&md=1&showWatermark=1&fontSize=125px&images=star) <!-- markdownlint-disable-line first-line-h1 -->

# Cookiecutter for Ansible Role

A [cookiecutter](https://cookiecutter.readthedocs.io/en/stable/) for
[Ansible](https:/docs.ansible.com/ansible/latest) roles with:

* initialized [Molecule](https://ansible.readthedocs.io/projects/molecule)
  directory for testing;
* [GitHub Actions](https://docs.github.com/en/actions) workflow for running
  [YAML Lint](https://yamllint.readthedocs.io/en/stable/),
  [AnsibleLint](https://ansible.readthedocs.io/projects/lint) and Molecule for
  continuous integration;
* GitHub Actions workflow for publishing the role to
  [Ansible Galaxy](https://galaxy.ansible.com);
* a _COPYING_ file containing the copyright license for the role; and
* a license notice at the top of each file.

## Usage

Install the Cookiecutter package.

```shell
pip install -U cookiecutter
```

Create a project skeleton for a new Ansible role.

```shell
cookiecutter gh:geoffreyvanwyk/cookiecutter-ansible-role
```

## How to use Features

### Testing with Molecule

To use Molecule, first install
[Docker](https://docs.docker.com/engine/install/ubuntu/) and run it as a
service.

```shell
sudo service docker start
```

### Publishing to Ansible Galaxy

To publish to Ansible Galaxy, create an account on it, copy your API key from
the _Preferences_ page of your Galaxy profile, then save it in the settings of
your GitHub repository
(_Security > Secrets and variables > Actions > Secrets > Repository secrets_)
as `GALAXY_API_KEY`.

## License

Copyright &copy; 2023 Geoffrey Bernardo van Wyk [(https://geoffreyvanwyk.dev)](https://geoffreyvanwyk.dev)

This file is part of Cookiecutter for Ansible role.

Cookiecutter for Ansible role is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.

Cookiecutter for Ansible role is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.

You should have received a copy of the GNU General Public License along with Cookiecutter for Ansible role. If not, see <https://www.gnu.org/licenses/>.
