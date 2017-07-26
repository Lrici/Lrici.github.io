#使用Github和Jekyll搭建自己的博客
本博客是按照新手搭建博客来写的

##本教程将使用到的工具：
* Github:用于
* Git：用于本地编辑的静态博客上传到Github上
* Jekyll:用于生成静态博客
* ruby：用于安装jekyll
* MarkdownPad：用于博客界面的编辑

##一、创建仓库以及Git的本地操作
###1、在Github上创建一个仓库
* 在Github上创建一个仓库、仓库名称为username.github.io，username就是你在Github上的用户名
* 在仓库中新建一个index.html文件，创建完成后别忘记Commit new file
* 现在访问username.github.io 就可以看到你创建的博客的一个页面啦，噔、噔、噔
* 博客中目前一个
###2、Git的本地操作
* 首先需要在本地建立一个存放博客的仓库
* 将在Github上创建的仓库clone下来，最好单独建立一个文件夹来保存与博客相关的内容文件；README.md文件的图标是MarkdownPad，在第五步中会介绍安装MarkdownPad。


##二、搭建本地环境

###1、安装ruby
* 安装Ruby的目的是通过RubyGem安装Jekyll；
* Ruby的下载地址 [http://railsinstaller.org/en](http://railsinstaller.org/en)，railsinstaller安装包包括的内容如下
* 在安装过程中选择默认就可以；安装完成后会默认产生一个sites的文件夹
###2、安装Bundler
* 打开Command Prompt with Ruby and Rails命令窗口执行  
  gem install bundler；
###3、安装jekyll
* 在Command Prompt with Ruby and Rails命令窗口执行
  gem install jekyll bundler

##三、Jekyll的使用
* 创建一个新的博客，
      进入在第一步中在本地建立的Blog目录，执行jekyll new Myblog   建立的时间可能会有一点久，请耐心等待，我用了大概8分钟左右
* build博客
      进入MyBlog目录，执行bundle install
      然后执行  bundle exec jekyll build
	   
* 启动、并访问博客，
      执行 bundle exec jekyll serve，在浏览器中访问 http://localhost:4000  会显示默认生成的网站
* 将博客上传到Github中，并访问浏览
*     将MyBlog文件夹中的文件，复制到 Lrici.github.io 文件夹中，提交到Github，现在访问Lrici.github.io显示的还是

需要我们把index.html删掉，就出现我们默认生成的模板了
##四、博客模板的使用
* 默认生成的网站当然不符合我们的需要；如果你想要手动DIY自己的博客、可以参考[http://jekyllrb.com/docs/structure/](http://jekyllrb.com/docs/structure/)
* 如果不想这么麻烦，可以从网上下载一些博客的模板然后改成自己的风格就可以；
* 模板的选择  
* [https://jekyll-themes.com/](https://jekyll-themes.com/)
* [http://jekyllthemes.org/](http://jekyllthemes.org/)

##五、使用Markdown编辑博客，并将其发布到自己的网站上
###1、安装MarkDownPad
* 下载地址[http://markdownpad.com/download.html](http://markdownpad.com/download.html)
###2、编辑博客
   在MarkDown中编辑博客，博客文件的命名方式 YEAR-MONTH-DAY-title.MARKUP
###3、发布博客
   将编辑好的博客存放到_post文件夹中，并上传到Github中
