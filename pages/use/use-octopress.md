#Use Octopress

##常用命令
创建新文章：rake new_post

##问题及解决
1 zsh中找不到rake new_post命令
报错：zsh: command not found: new_post["title"]
原因：诸如[]之类的字符不是正确的命令字符
解决：可使用转义符来解决这一问题,但每次都需要敲入转义符，实在是太麻烦了。可通过别名来解决：alias rake="noglob rake"。

2 rake版本错误导致rake new_post执行失败
报错：rake aborted!
Gem::LoadError: You have already activated rake 10.4.2, but your Gemfile requires rake 10.4.1. Prepending `bundle exec` to your command may solve this...
原因：gem更新时将rake版本升级了，但Octopress的Gemfile中要求的rake版本为10.0.
解决：修改Octopress的Gemfile，将gem ‘rake’, ‘~> 10.0’改为gem ‘rake’, ‘~> 10.4.2’，重新执行rake new_post[“title”]就没有问题了。