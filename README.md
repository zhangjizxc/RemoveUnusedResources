# RemoveUnusedResources

迭代删除无用资源的脚本, 适用于跟随android系统编译app. 在运行脚本前需要保证编译出来R文件.
(目前暂时不适用于Android Studio,稍后有时间要改造)
*  直接删除无用资源命令

打开终端,进入代码线的根目录
```shell
cd /media/zhangji/disk2/Code/openCode
....
. build/envsetup.sh
....
lunch aosp_shamu-userdebug
```

*  对于某一工程,例如SoundRecorderSmartisan
```shell
   ./removeunusedresources packages/apps/SoundRecorderSmartisan/
```
*  对于全部APP工程
```shell
   ./development/tools/findunused/removeunusedresources --all
```
