# TWRP Recovery Project

### How to build ###

```bash
# Create dirs
$ mkdir twrp ; cd twrp

# Init repo
$ repo init --depth=1 -u git://github.com/minimal-manifest-twrp/platform_manifest_twrp_omni.git -b twrp-9.0

# Clone my local repo
$ git clone https://github.com/tnakamur/android_manifest_sony_houou.git -b twrp .repo/local_manifests

# Sync
$ repo sync --no-repo-verify -c --force-sync --no-clone-bundle --no-tags --optimized-fetch --prune -j`nproc`

# Build
$ . build/envsetup.sh
$ lunch omni_houou-eng
$ mka bootimage
```

## Credits
2020 @tnakamur
