repo init -u https://github.com/getitnowmarketing/android_x86_manifest.git -b AsusT102HA

repo sync --no-tags --no-clone-bundle

~/android_x86/pie/vendor/opengapps/sources/x86$ git lfs pull (for all source types)

source build/envsetup.sh

lunch android_x86_64-userdebug

export USE_SQUASHFS=0

m -j4 iso_img

Read more: https://www.android-x86.org/source.html
