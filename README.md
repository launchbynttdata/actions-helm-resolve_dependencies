# Github Action to Recursively Resolve Chart Dependencies

## About

This action is designed to simplify the process of resolving chart dependencies in Helm. It will download, unpack, examine, and recursively resolve chart dependencies for the specified chart.

## Usage

```workflow
...
  steps:
  - name: Resolve Chart Dependencies
    uses: launchbynttdata/actions-helm-resolve_dependencies@v0
    with:
      chart_path: path/to/top/Chart.yaml
...
```

To use this action, you need to provide the following input:

* `chart_path`: The path to the top-level chart from where the dependency resolution should start.
