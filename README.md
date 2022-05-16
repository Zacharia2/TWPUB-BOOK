# TWPUB墨屉
收录TiddlyWiki\墨屉格式的电子书（TWPUB）

仅个人学习之用（本仓库不会删除，欢迎大家上传分享twpub图书，提交请求！。🙂，喜欢记得点小星星哦这是对我的鼓励，谢谢。爱你们！）

supermemo导入电子书只适合纯文本书籍，TW有更好的更兼容的方式，所以我的渐进式阅读目标已经达成了，首先是找到自己想要渐进式阅读的电纸书epub，然后用TWPUB-Tools工具转换，然后拖放放进wiki，然后重命名wiki+书目后缀，墨屉wiki的设置中标题选项＋书名后缀，然后放进onedrive。电脑就用TiddlyStow.html打开进行渐进式阅读。反正会同步的，没有电脑时候手机就用tiddloid.apk继续阅读（手机端的onedrive要在后台保持一直运行并且要阅读的书籍要设置允许脱机使用，这样tiddloid的对onedrive的连接才不会断开，第一次阅读时候才不会去先下载然后打开。）。

墨屉wiki导入书籍的流程：拖放书籍.json到墨屉（直接拖入浏览器），在墨屉的![图片](https://user-images.githubusercontent.com/32425955/166909870-f4871de5-c2f3-4c58-b7e4-cec6aeb66b0d.png)点击一下，选择倒三角形状的按钮，选择导入twpub书籍，然后会弹出一个条目，然后你就知道如何做啦。

墨屉是由条目（卡片组成），可以通过筛选器搭配标签使用，实现渐进式阅读。算法是优于sm18的 FSRS 间隔重复算法。



## 一、回写式保存文件

免浏览器下载的保存方法webdav：
1. rclone（单文件软件）：执行 rclone serve webdav <包含wiki的目录>。
2. wsgidav（python软件）:软件官网：https://wsgidav.readthedocs.io/en/latest/index.html


免浏览器下载的保存方法：TiddlyStow.html
1. 打开该页面然后选择墨屉wiki.html，即可
2. 支持保存常用文件列表
3. 刷新返回TiddlyStow页面
4. 来源于https://github.com/btheado/tiddlystow



## 二、电子书转换（epub 到 twpub）

1. 安装nodejs
   nodejs官网下载链接：http://nodejs.cn/download/current/

2. 下载转换工具包
   
   - 克隆转换工具仓库： https://github.com/TWPUB/TWPUB-Tools
   
   git clone https://github.com/TWPUB/TWPUB-Tools.git
   
   - 或者直接打包下载后解压也行

3. 进入到TWPUB-Tools目录，执行npm install
4. 转换书籍：
    - 执行：node epub2twpub --epub <EPUB文件> --output <twpub文件输出路径>
    - 注意：必须得在刚刚下载的...\TWPUB-Tools 目录下执行！否则好像提示没有找到命令。
    - 例如：node epub2twpub --epub C:\月亮与六便士-毛姆.epub --output C:\月亮与六便士-毛姆.json



## 帮助链接

https://github.com/TWPUB/TWPUB-Tools
https://tw-cn.netlify.app/


TiddlyWiki（太微）相关资源：中文教程、插件源、论坛、桌面应用
1. 大家可以一起编辑的中文教程项目： https://tw-cn.netlify.app/
2. 社区插件源： https://tw-cpl.netlify.app
3. TW唯一论坛，问问题、搜方案都来这里，（英文不好的话）开谷歌翻译全网页即可阅读，开 deepl 机翻即可发帖，大家多来交流！ https://talk.tiddlywiki.org/
4. 桌面版应用 TiddlyGit （太记）：https://github.com/tiddly-gittly/TiddlyGit-Desktop

   太记介绍和教程地址： https://zhuanlan.zhihu.com/p/140473235
   
   希望大家都能爱上TiddlyWiki！

QQ群：946052860
