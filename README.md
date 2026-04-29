openapi-generator-cli mirror
============================

Mirror of openapi-generator-cli for pre-commit. Created with [pre-commit-mirror-maker](https://github.com/pre-commit/pre-commit-mirror-maker).

For pre-commit: see https://github.com/pre-commit/pre-commit

For openapi-generator-cli: see https://pypi.org/project/openapi-generator-cli/

### Using openapi-generator-cli with pre-commit

Add this to your `.pre-commit-config.yaml`:

```yaml
-   repo: https://github.com/mxr/mirrors-openapi-generator-cli
    rev: ''  # Use the sha / tag you want to point at
    hooks:
    -   id: openapi-generator-cli
        # specify validate, generate, etc. each command requires another 'hooks' block
        args: []
        # default shown here; override based on your project setup
        files: '(^|/)(openapi|.*[.](json|ya?ml))$'
```

Note: This uses `openapi-generator-cli[jdk4py]` so openapi commands are supported out of the box.
