免费使用华为付费主题教程

首先，你要能下载这个主题，或者你最新版的主题商店支持试用主题。否则就需要root后修改主题商店安装包中带"client_support_tryout_theme"的方法的返回值为1。

下面是主题提取方法。

1.试用或者应用这个主题。

2.打开mt管理器，点击上方地址栏，输入路径“/data/themes/0/”就能找到解压缩后的主题,复制出全部文件（此时wallpaper文件夹为空）。“preview/preview_.*_compress.jpg”不用复制，也无法复制，跳过就行。

3.进入主题商店混搭一个图标，复制出“wallpaper”文件夹。

4.编辑复制出的“description.xml”，删除“<is_tryout_theme>.*</is_vip_no_paid_theme>”这一段，保存。

5.删除“pet”文件夹以及“send_to_report.json”，没有就不用管。

6.把全部文件压缩为zip，后缀名改为“.hwt”。

7.把主题复制到“/storage/emulated/0/Huawei/Themes/”下，就能在“主题商店-我的-主题”永久免费使用。

如果主题商店里没有显示主题，先稍等一会。如果等不及就卸载主题商店的更新：在设置里卸载主题商店，在桌面下拉搜索“主题”，选择“恢复”。

此方法无法提取主题中的全部文件，仅能提取主要文件。如果要提取全部文件，则需要root后在“/data/user/0/com.huawei.android.thememanager/cache/encryptCache/”下提取当前应用的主题。

如果以上方法失效，则可以卸载主题商店更新后，安装版本号低于12.0开头的旧版主题商店。这个版本的主题没有加密，可以在“/storage/emulated/0/Huawei/Themes/”下直接提取。但无法试用付费主题。

如果要提取预置主题和开机动画，则可以在“/hw_product”（新）或者“/data/hw_init”（旧）或者“/version”（RS系列）目录下搜索找到。对应的动态壁纸apk需要单独提取。新版预置主题需要在同目录“theme_standalone_icons”下提取图标后合入。

如果你的主题商店搜不到你要的新版主题，则需要root后将其中一个默认主题用压缩软件打开，将“description.xml”里的“<version>.*</version>”改为“<version>13.0.0</version>”（数字随系统升级增加），然后保存打包替换。默认主题里最高的版本号决定能用主题的最高版本，最低的版本号决定能用主题的最低版本。
