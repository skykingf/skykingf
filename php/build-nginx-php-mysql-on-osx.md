# 在OS X 11.1上搭建Nginx＋PHP＋MySQL的Web开发环境
***

## 1.安装homebrew
1. 打开终端Terminal。
2. 在命令行中输入如下命令安装homebrew  
  `ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"`  
  根据提示和向导，按Enter键和输入管理密码，homebrew官方提供的脚本会自动将homebrew安装到系统中。  
  如果出现`curl: (35) Server aborted the SSL handshake`错误提示，那么很可能是安装源的网站被墙了。
3. 如果中途失败，再次运行2中的命令，出现如下错误
  `It appears Homebrew is already installed. If your intent is to reinstall you
should do the following before running this installer again:
    ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/uninstall)"`  
    运行`rm -fr /usr/local/.git`，删掉缓存即可重新安装。
4. 安装完成后，运行`brew update`，更新安装包的最新信息。
5. 到此，homebrew就安装成功了。


## 2.安装Nginx
