# CI Build Patches

## Purpose

This repo is used for patches to the Brave CI build process. The patches are intended to be temporary,
and we use the scripts here to avoid having to manually update the build job shell script every time we need
to make minor changes to jobs.

This is modeled after the brave-browser and brave-core patch process.

## Producing diffs

To create the patches, use the `--full-index` argument to `git diff`. Our patches are applied after the
brave-core patches so must be created after those have been applied. If you have the same content in these
patches as brave-core, they will fail to apply cleanly.

TODO:

* differentiate patches between platforms (win/osx/linux)
  * maybe this doesn't matter, i.e. chrome/installer/linux/debian/ isn't relevant to Windows
* script will output info like platform, branch, brave-browser version for inline logging of
 what ran during each build (maybe url to branch in github)
