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

When using plugins with `eslint` you'll need to declare theme under
`additional_dependencies`. For example:

    -   repo: git://github.com/pre-commit/mirrors-eslint
        sha: ''  # Use the sha you want to point at
        hooks:
        -   id: eslint
            additional_dependencies:
            -   eslint-config-google@0.7.1
            -   eslint-loader@1.6.1
            -   eslint-plugin-react@6.10.3
            -   babel-eslint@6.1.2
