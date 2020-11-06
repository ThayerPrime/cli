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
