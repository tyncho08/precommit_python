# The pre-commit Python framework

We can run shell files all we want to dictate how our pre-commit process goes, but this pre-commit framework written in Python got us covered. It even comes with a set of pre-commit hooks out of the box (batteries included!). To adopt pre-commit into our system, we simply perform the following actions:

* Install pre-commit: `pip install pre-commit`
* Add pre-commit to requirements.txt (or requirements-dev.txt)
* Define `.pre-commit-config.yaml` with the hooks you want to include.
* Execute `pre-commit install` to install git hooks in your .git/ directory.

The YAML file configures the sources where the hooks will be taken from. In our case, flake8’s already been included in this framework so we just need to specify its id. On the other hand, we need to define where to source black using few lines of code.