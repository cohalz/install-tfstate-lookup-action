# install-tfstate-lookup-action

Composite run steps action for installing [fujiwara/tfstate-lookup](https://github.com/fujiwara/tfstate-lookup).

## Usage

Action cohalz/install-tfstate-lookup-action@v1 installs tfstate-lookup binary for Linux into /usr/local/bin. This action runs install only.

Pass the parameter "latest" to use the latest version of tfstate-lookup.



```yml
jobs:
  deploy:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v2
      - uses: cohalz/install-tfstate-lookup-action@v1
        with:
          version: v0.3.0 # or latest
```
