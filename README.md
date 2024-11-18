# netopeer-deb
Repo to automate builds of the netopeer2 stack deb packages.

## Releases
The resulting packages are published in the [project releases](https://github.com/cpascual/netopeer-deb/releases)

## apt repo

The deb packages are also published in an apt repo.

You can add the repo with:

```console
wget https://cpascual.github.io/netopeer-deb/gpg.key -O- > /etc/apt/trusted.gpg.d/netopeer-deb.asc
echo 'deb [arch=amd64] https://cpascual.github.io/netopeer-deb/ bookworm main' > /etc/apt/sources.list.d/netopeer-deb.list
```

...and then install packages with e.g.:

```console
apt update
apt install netopeer2 sysrepo-tools
```
