# OrangeFox Recovery Project for the Moto E6s

### How to build ###

```bash
# Create dirs
$ mkdir ofox; cd ofox

# Init repo
$ repo init --depth=1 -u https://gitlab.com/OrangeFox/Manifest.git -b fox_9.0

# Clone pokerp repo
$ git clone https://github.com/motorola-fiji-64/android_device_motorola_fiji_recovery -b fox-9.0 device/motorola/fiji

# Sync
$ repo sync --no-repo-verify -c --force-sync --no-clone-bundle --no-tags --optimized-fetch --prune -j`nproc`

# Build
$ chmod -R +x device/motorola/fiji/build_ofox.sh; mv device/motorola/fiji/build_ofox.sh .
```


