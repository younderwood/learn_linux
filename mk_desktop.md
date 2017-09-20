#gnome3增加自定义程序快捷方式

 

手动增加快捷方式配置文件

在/usr/share/application目录中存放着所有程序的快捷方式的配置文件，全部都采用.desktop结尾 

我们可以在这个目录添加一个新的配置文件来实现添加快捷方式 

配置文件的参数如下： 

Name: 程序快捷方式的名称

Comment: 程序快捷方式的描述

Exec: 程序可执行文件的路径

Terminal: 程序执行的方式，true为执行在命令行中，falase则相反

Type:  程序类型，默认为Application

Categories: 程序在Application面板中所属的分类，

StartupNotify: 设置是否现实程序启动和关闭的提示，默认为true

Icon: 程序图标的路径，如果只填写名字，那么gnome会在 /usr/share/icons 里面寻找这个图片

下面我举一个简单的例子，我创建了一个Komodo Edit的快捷方式，文件命名为komodo.desktop,内容如下 

[Desktop Entry]

Name=Komodo Edit

Comment=MyDevelopment

Icon=/home/App/Komodo-edit/share/icons/komodo256.png

Exec=/home/App/Komodo-edit/bin/komodo

Terminal=false

Type=Application

Categories=Development;

StartupNotify=true

保存后，我们就能在程序列表中看到它了