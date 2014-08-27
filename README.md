eslint mirror
================

Mirror of eslint package for pre-commit.

For pre-commit: see https://github.com/pre-commit/pre-commit
For eslint: see https://github.com/eslint/eslint


### Using eslint with pre-commit

Add this to your `.pre-commit-config.yaml`:

    -   repo: git://github.com/pre-commit/mirrors-eslint
        sha: ''  # Use the sha you want to point at
        hooks:
        -   id: eslint
