#Use Gollum

源码安装
git clone https://github.com/gollum/gollum
cd gollum
bundle install

安装成功后尝试着在终端输入下面的命令，如果能够正常显示版本号则说明安装成功.
gollum --v

创建自己的wiki系统
接下来我们就可以建立自己的wiki系统了，建立一个名字为”wiki”的目录使用git进行管理。进入到wiki目录，在wiki目录下启动gollum
mkdir wiki
cd wiki
git init
gollum

显示如下：
[2015-01-21 14:03:45] INFO  WEBrick 1.3.1
[2015-01-21 14:03:45] INFO  ruby 2.0.0 (2013-05-14) [x86_64-darwin12.4.1]
== Sinatra/1.4.5 has taken the stage on 4567 for development with backup from WEBrick
[2015-01-21 14:03:45] INFO  WEBrick::HTTPServer#start: pid=17699 port=4567

接下就可以在浏览器中访问了 http://localhost:4567/

创建wiki文档可以选择在全部Web界面进行操作，也可以选择在终端命令行进行提交管理markdown文件，在浏览器中进行查看。