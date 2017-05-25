## TWRP device tree for YU Yunique (jalebi)

Add to `.repo/local_manifests/jalebi.xml`:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
	<project name="TeamWin/android_device_yu_jalebi" path="device/yu/jalebi"  remote="github" revision="android-7.1" />
</manifest>
```

Then run `repo sync` to check it out.

To build:

```sh
. build/envsetup.sh
lunch omni_jalebi-eng
mka recoveryimage
```

Kernel sources are available at: https://github.com/LineageOS/android_kernel_cyanogen_msm8916
