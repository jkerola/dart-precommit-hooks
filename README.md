# Pre-Commit hooks for Dart

## Requirements

These hooks use the built in formatting and linting tools provided by the [Dart SDK](https://dart.dev/get-dart).

## Installing

Add the following to your `.pre-commit-config.yaml` file:

```yaml
repos:
  - repo: https://github.com/jkerola/dart-precommit-hooks
    rev: v1.0.0
    hooks:
      - id: dart-analyze
      - id: dart-format
```

Including and excluding files is supported:

```yaml
repos:
  - repo: https://github.com/jkerola/dart-precommit-hooks
    rev: v1.0.0
    hooks:
      - id: dart-analyze
        files: lib/* # defaults to all .dart files
        exclude: bin/* # nothing is excluded by default
```
