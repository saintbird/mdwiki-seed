#Use Mac

##Tools

终端：iTerm2, http://iterm2.com

Shell:  ZSH

文本编辑之Sublime Text2: [Sublime Tips & Tricks](http://code.tutsplus.com/tutorials/sublime-text-2-tips-and-tricks--net-21519)

文本编辑之Mou

Afred

Dash

安装包管理：Homebrew
brew install & brew cask install

版本管理：Git

Automater Workflow

##设置Mac环境
Mac系统的环境变量，加载顺序为：
/etc/profile 
/etc/paths 
~/.bash_profile 
~/.bash_login 
~/.profile 
~/.bashrc
/etc/profile和/etc/paths是系统级别的，系统启动就会加载，后面几个是当前用户级的环境变量。后面3个按照从前往后的顺序读取，如果~/.bash_profile文件存在，则后面的几个文件就会被忽略不读了，如果~/.bash_profile文件不存在，才会以此类推读取后面的文件。~/.bashrc没有上述规则，它是bash shell打开的时候载入的。
设置PATH的语法：
export PATH=$PATH:<PATH 1>:<PATH 2>:<PATH 3>:------:<PATH N>

##实用技巧
快速搭建本地HTTP服务器
- 使用Python: python -m SimpleHTTPServer 8080
- 使用node.js: npm install -g http-server http-server
- 使用Anvil: http://anvilformac.com/
