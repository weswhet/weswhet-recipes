Recipe for Kolide Launcher - https://github.com/kolide/launcher

### Notes:

This recipe will download from the latest full release from github (NOT PRE-RELEASES).

It currently takes the darwin binaries in the release tarball and makes a pkg to deploy them to `/usr/local/launcher/bin/*`.

The munki recipe will include an installs array for the included binaries, as well as including the github release notes for the latest version in the description.