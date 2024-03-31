# nixos-configs

## usage

```sh
git submodule init
git submodule update
```

## adding more

given a directory of configs, print the command to add these like:

```sh
for d in */ ; do
  cd $d
  echo "git submodule add $(git config --get remote.origin.url) $d"
  cd ..
done
```
