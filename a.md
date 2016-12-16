# [moai-patch 0.5.4](http://git.code.oa.com/moai/patch/tree/0.5.4) Release Notes
### Date: 2016-12-15
### Version: 0.5.4
### Fix:
* patch 的目录 dexopt/dex2oat 之后不允许有任何变动，否则系统会重新 dexopt/dex2oat
### Fix:
* 修改 module 名称
* 整理 sp 存储的变量

# [moai-patch 0.4.9](http://git.code.oa.com/moai/patch/tree/0.4.9) Release Notes
### Date: 2016-12-07
### Version: 0.4.9
### Fix:
* patch 过程中非 patch 进程启动使用了正在 patch 的目录导致 crash bugifx
* 主进程才有权创建首次启动标志文件 bugfix，否则如果其他进程先于主进程启动，导致主进程启动后发现不是第一次启动，不会清除之前旧的 patch
* 安装新版本 app 启动后主进程没有杀死其他进程 bugfix，确保所有进程使用同一份代码
