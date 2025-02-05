# netopeer-deb
Repo to automate builds of the netopeer2 stack deb packages.

## Releases
The resulting packages are published in the [project releases](https://github.com/cpascual/netopeer-build/releases)

## apt repo

The deb packages are also published in an apt repo.

You can add the repo with:

```console
wget https://iPronics.github.io/netopeer-build/gpg.key -O- | sudo tee /etc/apt/trusted.gpg.d/netopeer-deb.asc
echo 'deb [arch=amd64] https://iPronics.github.io/netopeer-build/ bookworm main' | sudo tee /etc/apt/sources.list.d/netopeer-deb.list
```

...and then install packages with e.g.:

```console
sudo apt update
sudo apt install sysrepo-tools
sudo apt install netopeer2
```
