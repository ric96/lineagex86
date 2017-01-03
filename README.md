# lineagex86
linage os on android-x86 platform

$ mkdir android-x86
$ cd android-x86
$ repo init -u git://git.osdn.net/gitroot/android-x86/manifest -b $branch
replace cm.xml .repo/manifests
$ repo init -m cm.xml
$ repo sync --no-tags --no-clone-bundle

$ cd packages/services/Telecomm/
$ git revert 1d0ca65e7b41d2728c226ae9284df6ff8e322db3
$ git revert 01882f2df414e2946baf07bef93b3216105a74ec

as of https://github.com/LineageOS/android_build/commit/a0300d400ace78f8045f17c24db33ce6d38dc072
and previous rebase commits
replace Makefile to build/core/
replace dumpvar.mk build/core/
replace envsetup.sh build/
replace folder notfication and notificationlight packages/apps/Settings/src/com/android/settings
