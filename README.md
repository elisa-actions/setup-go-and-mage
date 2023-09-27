# setup-go-and-mage

Action to setup Go and Mage in your GitHub Actions workflow.

## Usage

### Simple use with defaults

```yaml
# set up go without go.mod caching and mage with the version defined in go.mod

steps:
- uses: actions/setup-go-and-mage@main
```

### Use with caching and custom modfile path

```yaml
steps:
- uses: actions/setup-go-and-mage@main
  with:
    go-cache: true
    modFile: <path-to-modfile>  # defaults to go.mod in repo root
```
