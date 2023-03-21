Using [flatpak-node-generator](https://github.com/flatpak/flatpak-builder-tools/tree/master/node)

`yarn.lock` and `package-lock.json` have been built from the same `package.json`. Changing the packages used and the node/npm version does not change the result.

# NPM

When using `flatpak-node-generator npm package-lock.json` `generated-sources.json` only has 4 sources written:

```console
$ flatpak-node-generator npm package-lock.json
Reading packages from lockfiles...
20 packages read.
Generating packages [20/20] jake @ 10.8.5                                                                                                                                                                                               
Wrote 4 source(s).
```

The number of sources is always the same and always is only node-gyp and a script file (seems auto generated).

# Yarn

When using `flatpak-node-generator yarn yarn.lock` `generated-sources.json` has 4 sources written:

```console
$ flatpak-node-generator yarn yarn.lock
Reading packages from lockfiles...
19 packages read.
Generating packages [19/19] brace-expansion @ 1.1.11                                                                                                                                                                                    
Wrote 21 source(s).
```
