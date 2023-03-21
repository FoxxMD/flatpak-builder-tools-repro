Using [flatpak-node-generator](https://github.com/flatpak/flatpak-builder-tools/tree/master/node)

`yarn.lock` and `package-lock.json` have been build from the same `package.json`

# NPM

When using `flatpak-node-generator npm package-lock.json` `generated-sources.json` only has 4 sources written:

```console
$ flatpak-node-generator npm package-lock.json
Reading packages from lockfiles...
421 packages read.
Generating packages [421/421] duplexer3 @ 0.1.5                                                                                                                                                                                         
Wrote 4 source(s).
```

# Yarn

When using `flatpak-node-generator yarn yarn.lock` `generated-sources.json` has 4 sources written:

```console
$ flatpak-node-generator yarn yarn.lock
Reading packages from lockfiles...
405 packages read.
Generating packages [405/405] make-error @ 1.3.6                                                                                                                                                                                        
Wrote 407 source(s).
```
