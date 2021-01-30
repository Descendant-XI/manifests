To initialize your local repository, use this command:

	repo init -u https://github.com/descendant-xi/manifests.git -b eleven-staging

 Then to sync up:

```bash
repo sync --force-sync --no-tags --no-clone-bundle -j$(nproc --all)
```

Build Descendant
==================

```bash
source build/envsetup.sh

lunch descendant_codename-buildtype

mka descendant
```

Thanks to POSP and specifically Kshitij Gupta for supporting us in using POSP early AOSP bring-up as our "hardware equipped AOSP base".

If you have an issue with syncing or building feel free to reach out at https://t.me/descendant_device_support
