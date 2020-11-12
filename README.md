# Reliably CLI
Reliability toolbox for developers from the command line.

### Usage

To review your Kubernetes manifests for reliability advice, simply run:

```
$ reliably discover
```

It will scan for manifests recursively in your current working directory.

To indicate a specific folder, you can use the `--dir` flag, as follow:

```
$ reliably discover --dir ./manifests
```

#### Use as a Github Action

You can use Reliably as part of your Github workflows, by using our [Github Action](https://github.com/reliablyhq/gh-action)

```yaml
- name: Run Reliably
  uses: reliablyhq/gh-action@main
```

#### Use as a docker container

You can run the CLI with our [docker image](https://github.com/orgs/reliablyhq/packages/container/package/cli%2Fcli)

```
$ docker run --rm \
  --volume=</path/to/manifests/folder>:/manifests \
  ghcr.io/reliablyhq/cli/cli \
  review --dir /manifests
```

