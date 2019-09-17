## ZenOS CAF Android 10 ##

## Repo Init ##
```bash
repo init -u https://github.com/ZenOS-CAF-Q/manifest.git -b ten-caf
```
## Sync Source ##
```bash
repo sync -c -f --force-sync --no-tag --no-clone-bundle -j$(nproc --all)
```
## Build Time (Linux x86_64 ONLY) ##
```bash
. build/envsetup.sh
brunch zen_<DEVICE>-userdebug (or zen_<DEVICE>-user)
