# Developer notes

## Making a release

This requires the following tools:

  - [vmanage (by Gerph)](https://github.com/gerph/riscos-vmanage)

The procedure is:

  - Make sure the module builds correctly using the Github CI pipeline and RISC OS Build Service (preferred) or the `!!Release` script under RISC OS.
  - Bump the version number in VersionNum: `vmanage inc`
  - Update `!ReadMe` to include the new version number
  - Commit the new `VersionNum` and `!ReadMe` files: `git commit VersionNum \!ReadMe`
  - Tag the new release: `git tag v1.23`  (**remember to specify the correct version number!**)
  - Push to Github: `git push --tags`


