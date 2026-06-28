## Repo Init ##
```bash
repo init -u https://github.com/V1NAY007/kernel_manifest.git -b bka
```
## Sync Source ##
```bash
repo sync --force-sync --no-clone-bundle --current-branch --no-tags -j$(nproc --all)
```
## Start building ##
```bash
LTO=thin build/build.sh -j$(nproc --all)
```
