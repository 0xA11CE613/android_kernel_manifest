
## Repo Init ##
```bash
repo init -u https://github.com/prabhatKrMishra/android_kernel_manifest.git -b msm-6.1-blair
```
## Sync Source ##
```bash
repo sync --force-sync --no-clone-bundle --current-branch --no-tags -j$(nproc --all)
```
## Build ##
For Clang builds
```bash
BUILD_CONFIG=kernel/msm-5.4/build.config.msm.holi VARIANT=qgki LTO=thin TARGET_PRODUCT=fogos BUILD_KERNEL=1 TARGET_BUILD_VARIANT=user build/build.sh
```
