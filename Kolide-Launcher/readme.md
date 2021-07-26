Recipe for Kolide Launcher - https://github.com/kolide/launcher

### Notes:

Now uses the universal build of launcher for Silicon support.

This recipe will download from the latest full release from github (NOT PRE-RELEASES).

It currently takes the darwin binaries in the release tarball and makes a pkg to deploy them to `/usr/local/launcher/bin/*`.

The munki recipe will include an installs array for the included binaries, as well as including the github release notes for the latest version in the description.

As of launcher version 0.11.16 it no longer includes osqueryd. Would suggest `osquery.*.recipe`'s

The pkg recipe here removes the newly included `package-builder` binary.
