# TWPUB墨屉
收录TiddlyWiki的电子书（TWPUB），墨屉格式电子书




## 电子书转换（epub 到 twpub）

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
