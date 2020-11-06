# Reliably CLI
Reliability toolbox for developers from the command line.

### Usage

To review your Kubernetes manifests for reliability advice, simply run:

```
$ reliably review
```

It will scan for manifests recursively in your current working directory.

To indicate a specific folder, you can use the `--dir` flag, as follow:

```
$ reliably review --dir ./manifests
```

#### Use as a Github Action

You can use Reliably as part of your Github workflows, by using our [gh-action](https://github.com/reliablyhq/gh-action)

```yaml
- name: Run Reliably
  uses: reliablyhq/gh-action@main
```
