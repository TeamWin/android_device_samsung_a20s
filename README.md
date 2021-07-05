# Orange Fox Recovery for Samsung Galaxy A20s

### How to build ###

```bash
# Create dirs
$ mkdir of; cd of

# Init repo
$ repo init --depth=1 -u https://gitlab.com/OrangeFox/Manifest.git -b fox_9.0

# Clone a20s repo
$ git clone https://github.com/TeamWin/android_device_samsung_a20s -b fox-9.0 device/samsung/a20s

# Sync
$ repo sync --no-repo-verify -c --force-sync --no-clone-bundle --no-tags --optimized-fetch --prune -j`nproc`

# Build
$ mv device/samsung/a20s/build_ofox.sh .; chmod +x build_ofox.sh; ./build_ofox.sh
```

## Status

**Works**

- Booting
- Zip/img flashing
- ADB/MTP
- Vibration
- Backup/Restore
- Mount

**Don't Work**

- Encryption

## Credits
* mohammad92: For ```a11q``` device/kernel tree.
* firemax13/sunamitheory: Helping me a lot.
* Astrako: For ```build_ofox.sh``` script.
