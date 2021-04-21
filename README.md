# wiki-docs-submodule

Example repository setup where the Github wiki is included as a git submodule, and any changes to the repo will update the wiki, and and wiki edits are automatically updated in the repo and attributed appropriately with a Github Action.

To develop:

```
git clone https://github.com/igorbrigadir/wiki-docs-submodule.git
git submodule update --init
```

`cd` into `docs` folder, push and commit docs changes to the submodule to update the wiki.

Some caveats: using submodules means you may have to add some additional configurations and steps for things like readthedocs for example.

For reference, making a new submodule:

```
git submodule add git@github.com:igorbrigadir/wiki-docs-submodule.wiki.git docs
```

Removing a submodule:

```
git submodule deinit docs
```
