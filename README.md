# [首页查询更多项目](https://github.com/GraduationProject-springboot) 包安装运行


# 0712springboot校园志愿者管理系统--论文

![picture](https://raw.githubusercontent.com/GraduationProject-springboot/.github/main/img/wx.png)

### 点击播放视频 ▼
[![Watch the video](https://i.sstatic.net/Vp2cE.png)](https://www.bilibili.com/video/BV14HerezEwW?p=65)


# 第一章 绪论
## 1.1  研究背景
科学技术日新月异的如今，计算机在生活各个领域都占有重要的作用，尤其在信息管理方面，在这样的大背景下，学习计算机信息不仅仅是为了掌握一种技能，更重要的是能够让它真正地使用到实践中去，以创新的视角去不断方便人们的生活，推动对新知识的学习，培养自学能力，锻炼动手实践的本领。现代的校园志愿者管理系统，也应该摆脱人工管理的模式，使用计算机技术来进行信息管理工作。所以本次系统设计的校园志愿者管理结合了文字、图像，并能实现校园志愿者管理的功能，这也是一般校园志愿者系统的重要的要素。校园志愿者管理系统经过几年的实践和总结正在往更深入的方向发展。由此，人们要改善系统功能迫在眉睫。随着线上管理系统的飞速发展，校园志愿者管理系统不断完善其工作流程的繁杂性、多样化、管理复杂、收缴费用与设备维护繁琐等存在的问题。所以要通过计算机胜任校园志愿者管理的工作，使校园志愿者系统更加准确、方便及快捷。

因此，开发出一套高效率、低差错的校园志愿者信息管理系统是十分必要。本系统主要目的是全面实现校园志愿者管理系统数字化，管理员对于用户的所有信息能够全部掌握，而用户能够对自己的校园志愿者信息能够有一个直观的了解。
## 1.2  系统研究现状
现如今，校园志愿者的服务并不很完善，尽管实行了校园志愿者管理，但传统的管理方式远远不够，传统的管理方式只停留在传统的状态。同时，因资金有限再加上也缺少专业水平的工作人员，所以校园志愿者的管理手段较为落后，也就很难提高校园志愿者的管理效率，同时也就不能很好的为用户提供更为完善的服务。传统的管理方式都是通过手动来进行管理记录及操作，不但麻烦琐碎，还经常出现错误，给广大用户带来很不便，同时也需要大量的人力、物力和财力，极大的浪费了校园志愿者的资源。校园志愿者管理系统是校园志愿者信息管理的一个重要组成部分，随着线上管理系统的快速发展，人们慢慢地来希望校园志愿者管理系统能够提供更为合理及完善的校园志愿者服务。现在，好的校园志愿者管理也成为广大用户们的关键。
## 1.3  系统实现的功能
本次设计任务是要设计一个校园志愿者管理系统，通过这个系统能够满足管理员和志愿者的校园志愿者信息管理功能。系统的主要功能包括首页、个人中心、志愿者管理、活动类型管理、活动信息管理、活动报名管理、活动通知管理、活动心得管理、交流反馈、系统管理等功能。

管理员可以根据系统给定的账号进行登录，登录后可以进入校园志愿者管理系统对校园志愿者所有模块进行管理。包括查看和修改自己的个人信息以及登录密码。

该系统为每一个用户都分配了一个用户账号，用户通过账号的登录可以在系统中查看校园志愿者信息及对个人信息进行修改等功能。
## 1.4系统实现的特点
本系统提供给管理员对首页、个人中心、志愿者管理、活动类型管理、活动信息管理、活动报名管理、活动通知管理、活动心得管理、交流反馈、系统管理等诸多功能进行管理。本系统对于用户输入的任何信息都进行了一定的验证，为管理员操作提高了效率，也使其数据安全性得到了保障。
## 1.5  本文的组织结构
本文的组织结构如下：

1、绪论。综述了本文的研究背景，分析了校园志愿者管理系统的结构；更好的从用户的角度出发，发现当今校园志愿者系统中的不足，同时要指出本次系统中的特色。

` `2、对系统主要的使用技术，开发环境、环境配置的介绍。介绍了本次开发所用的系统开发环境MyEclipse，还介绍了Tomcat环境配置、springboot框架和MySql环境配置。

3、系统的设计与实现。介绍了开发校园志愿者管理信息系统的思路并进行了需求分析，在需求分析的基础上进行了总体设计、详细设计以及数据库等相关方面介绍；该部分是全文的主旨。

4、系统功能模块具体实现。对开发中一些主要具体功能的实现进行描述。涉及到数据库、页面参数传递等相关知识。

5、对系统进行测试；

6、总结与展望。对整个论文及设计过程进行总结，指出系统设计过程的心得以及设计中存在的不足；后期还有待完善的地方等;包括致谢。
# 第二章开发技术与环境配置
以Java语言为开发工具，利用了当前先进的springboot框架，以MyEclipse10为系统开发工具，MySQL为后台数据库，开发的一个校园志愿者管理系统。
## 2.1  SpringBoot框架
SpringBoot是一个全新开源的轻量级框架。基于Spring4.0设计，其不仅继承了Spring框架原来有的优秀特性，而且还通过简化配置文件来进一步简化了Spring应用的整个搭建以及开发过程。另外在原本的Spring中由于随着项目的扩大导入的jar包数量越来越大，随之出现了jar包版本之间的兼容性问题，而此时SpringBoot通过集成大量的框架使得依赖包的版本冲突，以及引用的不稳定性问题得到了很好的解决。

SpringBoot可以看做是Spring的加强版本，但实质上都是Spring的相关技术，有了这些优秀的开源框架，程序员在开发过程中将事半功倍。
## ` `2.2Java语言简介
Java是由SUN公司推出，该公司于2010年被oracle公司收购。Java本是印度尼西亚的一个叫做爪洼岛的英文名称，也因此得来java是一杯正冒着热气咖啡的标识。Java语言在移动互联网的大背景下具备了显著的优势和广阔的前景，它是面向对象的，分布式的，动态的，具有平台无关性、安全性、健壮性。Java语言的基本语句语法和C++一样，但是它面向对象的技术更加彻底，因为Java要求将所有的内容都必须封装成类，把类作为程序的基本单位。由于不允许类外有变量、方法。 Java语言的分布式体现在数据分布和操作分布，它是面向网络的语言，可以处理TCP/IP协议，它也支持客户机/服务器的计算模式。Java语言的动态性是指类在运行时是动态安装的，使得Java可以动态的维护程序。Java不支持指针，对内存访问的所有操作都是通过对象实例化实现的，这样就避免了指针操作中易产生的错误，同时也预防了病毒对系统的破坏和威胁。

Java语言的编程风格与C语言非常接近，它继承了C++面向对象技术的核心，它面世之后发展迅速，非常流行，对高级C语言形成了很大的冲击。业内人士称之为“一次编译、到处执行”。当然java也有缺点，在每次执行编译后，字节码都需要消耗一定的时间，在某些程度上降低了性能。但是这并不影响java成为此次设计语言的选择。Java语言简单易学，使用它的编程时间短，功能性强，开发者学习起来更简便、更快。Java的主要特性有以下几个：

1.面向对象

面向对象有四个特点：封装、继承、多态、抽象。抽象是指忽略一个问题中的次要部分，关注主要部分。多态是指对同一种消息做出的不同反应。继承是指在原有的父类方法基础上增加自己独有的方法，而不改变原来父类。

2.平台无关性、

Java编译出来的是字节码，直接由虚拟机执行。在任何平台上，只要有Java虚拟机，Java代码都能运行。

3.可靠性和安全性

Java对内存的访问都必须通过对象的实例变量来实现，避免了指针中出现的错误。

\4. 多线程	

Java提供了多线程功能，利用编程实现同一时间同时工作的功能。
## 2.3  MySQL环境配置
（1）本系统的数据使用的是MySQL,所以要将MySQL安装到指定目录，如果下载的是非安装的MySQL压缩包，直接解压到指定目录就可以了。然后点击C:\Program Files\MySQL\bin\winMySQLadmin.exe这个文件其中C:\Program Files\MySQL是MySQL安装目录。输入winMySQLadmin的初始用户、密码（注：这不是MySQL里的用户、密码）随便填不必在意，确定之后右下角任务的启动栏会出现一个红绿灯的图标，红灯亮代表服务停止，绿灯亮代表服务正常，左击这个图标->winnt->install the service 安装此服务，再左击这个图标->winnt->start the service 启动MySQL服务。

（2）修改MySQL数据库的root密码。用cmd进入命令行模式输入如下命令:

cd C:\Program Files\MySQL\bin

MySQLadmin -u root -p password 123

回车出现Enter password: ，这是要输入原密码. 刚安装时密码为空,所以直接回车，此时MySQL 中账号 root 的密码被改为 123 安装完毕。
## 2.4  MyEclipse环境配置
安装完MyEclipse后选择myeclipse“Window->Preferences”

（1）配置myeclipse的jre为sun的jdk，不要用myeclipse的默认jdk：

选择“java->Installed JREs”,勾中里面的“jdk1.7”.

（2）配置编译的级别为6.0：

选择“Compiler->Compiler compliance level”的值为“6.0”。

（3）配置myeclipse的默认的文件编码格式为“UTF-8”：

`   `选择“General->Workspace”，选中“Text file encod”下面的“Other”，设置里面的值为“UTF-8”。

（4）去掉myeclipse的JSP的验证：

选择“MyEclipse->Validation”,将“Build”列的所有勾都给去掉,这样在编译时因为避免了jsp的验证，所以编译的速度会快很多.
## 2.5  mysql数据库介绍
利用MYSQL的数据独立性、安全性等特点，在软件项目中对数据进行操作，可以保证数据准确无误，并降低了程序员的应用开发时间。

MYSQL的特点是支持多线程，能方便的对系统资源充分利用，有效提高速度，还提供多种方式途径来对数据库进行连接；MYSQL的功能相对弱小、规模也小，但本系统要求不高，MYSQL完全可以满足本系统使用。

利用MYSQL建立系统数据库，不仅有利于数据处理业务的早期整合，还能利于发展后两种数据扩展的操作。

## 2.6  B/S架构
B/S结构是目前使用最多的结构模式，它可以使得系统的开发更加的简单，好操作，而且还可以对其进行维护。使用该结构时只需要在计算机中安装数据库，和一些很常用的浏览器就可以了。浏览器就会与数据库进行信息的连接，可以实现很多的功能，B/S结构是可以直接进行使用的，而且B/S结构在使用中极大的减少了工作的维护。基于B/S的软件，所有的数据库之间都是相互独立的，因此是非常安全的。因为基于B/S结构可以清楚的看到系统正在处理的业务，并且能够及时的让管理人员做出决策，这样就可以避免企业的损失。B/S结构的基本特点是集中式的管理模式，用户使用系统生成数据后，这些数据就可以存储到系统的数据库中，方便日后能够用到，这样就可以满足人们的所有的需求。

![](/md/blog.007.png)

图2-1  B/S模式三层结构图
# 第三章系统分析与设计
## 3.1 可行性分析
一个完整的系统，可行性分析是必须要有的，因为他关系到系统生存问题，对开发的意义进行分析，能否通过本系统来补充线下校园志愿者管理模式中的缺限，去解决其中的不足等，通过对本系统，不仅能使工作量不断地减少，还能使工作和管理的效率更加高。所以开发该系统能实现更大的意义和价值，系统完成后，能否达到预期效果就要通过可行性分析，分析之后，决定此系统是否开发。该校园志愿者管理系统的开发设计中，对技术、经济、操作方面进行了可行性分析；
### 3.1.1 技术可行性
本系统开发选择java语言，它被研究的目的就是在于能够为网页创建等可以看到的信息。随着移动互联网技术的不断发展和创新，java俨然已成为下一代互联网的Web标准。所以后台设计选择使用mysql数据库主要用来的建立和维护信息。对于前台开发要求应具备功能完善、易于操作等优点，后台数据库的要求则是能够建立和维护数据信息的统一性和完整性。
### 3.1.2 操作可行性
现在随着科技的飞速发展，计算机早已经进入了人们的日常生活中，人们的工作环境也不像以前有那么多的要求，需要工作人员一定要到公司办公，有的工作在家也可以完成。这使得人们的工作效益有了很大的提高。操作的多样性也变高了。因此，管理的计算机化，智能化是社会发展而带来的必然趋势，各种智能的软件层出不穷，不同的软件能完成用户不同的需求，这不仅提高了工作效率还能完成一些用户特定的一些需求。本系统不仅界面简洁明了还采用可视化界面，用户只要用鼠标和键盘就可以完成对相关信息的修改，删除，添加等操作。因为这个系统的操作十分简单，方便上手，对于第一次使用系统的人，只需要很少的时间就可以上手操作。由此可见，本系统在操作上是可行的。
### 3.1.3经济可行性
基于springboot的校园志愿者管理系统，该系统软件开发仅需要一台普通的计算机便可完成实现开发，其成本很低。另外，作为毕业设计作品来讲，开发成本基本上可以忽略不计，且该系统软件的投入使用，可以实现更加快速高效的校园志愿者管理，同时还能实现对人力资源和管理资源的有效节约，该校园志愿者管理系统在经济上完全可行。
## 3.2  需求分析
利用springboot、Java、MyEclipse和mysql数据库等知识点，结合相关设计模式、以及软件工程的相关知识，设计一个校园志愿者管理系统，来进行记录用户的信息，以及系统信息的增删改查的功能，根据实现需求，系统需完成这些基本功能：

（1）系统合理显示系统首页界面，管理员界面和志愿者界面等功能界面。

（2）所有用户的信息都保存与数据库中。 

（3）对校园志愿者信息能够进行查询、修改、删除、添加等操作。
## 3.3  总体设计
根据校园志愿者管理系统的功能需求，进行系统设计。

前台功能：用户进入系统可以实现首页、活动信息、活动心得、公告信息、交流反馈、个人中心、后台管理等功能进行操作；

后台由管理员和志愿者，主要功能包括首页、个人中心、志愿者管理、活动类型管理、活动信息管理、活动报名管理、活动通知管理、活动心得管理、交流反馈、系统管理等功能；

系统对这些功能进行整合，产生的功能结构图如下：

![](/md/blog.008.png)

图3-1 系统总体结构图

## 3.4  数据库设计与实现
在每一个系统中数据库有着非常重要的作用，数据库的设计得好将会增加系统的效率以及系统各逻辑功能的实现。所以数据库的设计我们要从系统的实际需要出发，才能使其更为完美的符合系统功能的实现。
### 3.4.1  数据库概念结构设计
数据库的E-R图反映了实体、实体的属性和实体之间的联系。下面是各个实体以及实体的属性。

活动信息实体属性图如下所示：

![](/md/blog.009.png)

图3-2活动信息实体属性图

活动心得实体属性图如下所示：

![](/md/blog.010.png)

图3-3活动心得实体属性图

活动报名实体属性图如下所示：

![](/md/blog.011.png)

图3-4活动报名实体属性图
### 3.4.2数据库具体设计
根据E-R图，设计每张表的变量名，变量的类型及主键等如下。

表4-1：配置文件

|字段名称|类型|长度|字段说明|主键|默认值|
| :-: | :-: | :-: | :-: | :-: | :-: |
|id|bigint||主键|主键||
|name|varchar|100|配置参数名称|||
|value|varchar|100|配置参数值|||
表4-2：token表

|字段名称|类型|长度|字段说明|主键|默认值|
| :-: | :-: | :-: | :-: | :-: | :-: |
|id|bigint||主键|主键||
|userid|bigint||用户id|||
|username|varchar|100|用户名|||
|tablename|varchar|100|表名|||
|role|varchar|100|角色|||
|token|varchar|200|密码|||
|addtime|timestamp||新增时间||CURRENT\_TIMESTAMP|
|expiratedtime|timestamp||过期时间||CURRENT\_TIMESTAMP|
表4-3：收藏表

|字段名称|类型|长度|字段说明|主键|默认值|
| :-: | :-: | :-: | :-: | :-: | :-: |
|id|bigint||主键|主键||
|addtime|timestamp||创建时间||CURRENT\_TIMESTAMP|
|userid|bigint||用户id|||
|refid|bigint||收藏id|||
|tablename|varchar|200|表名|||
|name|varchar|200|收藏名称|||
|picture|varchar|200|收藏图片|||
|type|varchar|200|类型(1:收藏,21:赞,22:踩)||1|
|inteltype|varchar|200|推荐类型|||



表4-4：公告信息

|字段名称|类型|长度|字段说明|主键|默认值|
| :-: | :-: | :-: | :-: | :-: | :-: |
|id|bigint||主键|主键||
|addtime|timestamp||创建时间||CURRENT\_TIMESTAMP|
|title|varchar|200|标题|||
|introduction|longtext|4294967295|简介|||
|picture|varchar|200|图片|||
|content|longtext|4294967295|内容|||
表4-5：交流反馈

|字段名称|类型|长度|字段说明|主键|默认值|
| :-: | :-: | :-: | :-: | :-: | :-: |
|id|bigint||主键|主键||
|addtime|timestamp||创建时间||CURRENT\_TIMESTAMP|
|userid|bigint||留言人id|||
|username|varchar|200|用户名|||
|content|longtext|4294967295|留言内容|||
|cpicture|varchar|200|留言图片|||
|reply|longtext|4294967295|回复内容|||
|rpicture|varchar|200|回复图片|||
表4-6：活动信息

|字段名称|类型|长度|字段说明|主键|默认值|
| :-: | :-: | :-: | :-: | :-: | :-: |
|id|bigint||主键|主键||
|addtime|timestamp||创建时间||CURRENT\_TIMESTAMP|
|huodongmingcheng|varchar|200|活动名称|||
|huodongleixing|varchar|200|活动类型|||
|tupian|varchar|200|图片|||
|huodongshijian|date||活动时间|||
|renshu|int||人数|||
|huodongchangdi|varchar|200|活动场地|||
|huodongjieshao|longtext|4294967295|活动介绍|||
|sfsh|varchar|200|是否审核||否|
|shhf|longtext|4294967295|审核回复|||
表4-7：活动心得

|字段名称|类型|长度|字段说明|主键|默认值|
| :-: | :-: | :-: | :-: | :-: | :-: |
|id|bigint||主键|主键||
|addtime|timestamp||创建时间||CURRENT\_TIMESTAMP|
|huodongmingcheng|varchar|200|活动名称|||
|huodongleixing|varchar|200|活动类型|||
|tupian|varchar|200|图片|||
|xindefenxiang|longtext|4294967295|心得分享|||
|fabushijian|datetime||发布时间|||
|userid|bigint||用户id|||
表4-8：活动通知

|字段名称|类型|长度|字段说明|主键|默认值|
| :-: | :-: | :-: | :-: | :-: | :-: |
|id|bigint||主键|主键||
|addtime|timestamp||创建时间||CURRENT\_TIMESTAMP|
|biaoti|varchar|200|标题|||
|xuehao|varchar|200|学号|||
|xingming|varchar|200|姓名|||
|shouji|varchar|200|手机|||
|tongzhineirong|longtext|4294967295|通知内容|||
|tongzhishijian|datetime||通知时间|||
表4-9：活动类型

|字段名称|类型|长度|字段说明|主键|默认值|
| :-: | :-: | :-: | :-: | :-: | :-: |
|id|bigint||主键|主键||
|addtime|timestamp||创建时间||CURRENT\_TIMESTAMP|
|huodongleixing|varchar|200|活动类型|||
表4-10：活动报名

|字段名称|类型|长度|字段说明|主键|默认值|
| :-: | :-: | :-: | :-: | :-: | :-: |
|id|bigint||主键|主键||
|addtime|timestamp||创建时间||CURRENT\_TIMESTAMP|
|huodongmingcheng|varchar|200|活动名称|||
|huodongleixing|varchar|200|活动类型|||
|renshu|int||人数|||
|baomingshuoming|varchar|200|报名说明|||
|baomingshijian|datetime||报名时间|||
|xuehao|varchar|200|学号|||
|xingming|varchar|200|姓名|||
|shouji|varchar|200|手机|||
|sfsh|varchar|200|是否审核||否|
|shhf|longtext|4294967295|审核回复|||
表4-11：志愿者

|字段名称|类型|长度|字段说明|主键|默认值|
| :-: | :-: | :-: | :-: | :-: | :-: |
|id|bigint||主键|主键||
|addtime|timestamp||创建时间||CURRENT\_TIMESTAMP|
|xuehao|varchar|200|学号|||
|mima|varchar|200|密码|||
|xingming|varchar|200|姓名|||
|xingbie|varchar|200|性别|||
|touxiang|varchar|200|头像|||
|nianling|varchar|200|年龄|||
|banji|varchar|200|班级|||
|youxiang|varchar|200|邮箱|||
|shouji|varchar|200|手机|||
|sfsh|varchar|200|是否审核||否|
|shhf|longtext|4294967295|审核回复|||
表4-12：活动心得评论表

|字段名称|类型|长度|字段说明|主键|默认值|
| :-: | :-: | :-: | :-: | :-: | :-: |
|id|bigint||主键|主键||
|addtime|timestamp||创建时间||CURRENT\_TIMESTAMP|
|refid|bigint||关联表id|||
|userid|bigint||用户id|||
|nickname|varchar|200|用户名|||
|content|longtext|4294967295|评论内容|||
|reply|longtext|4294967295|回复内容|||
表4-13：用户表

|字段名称|类型|长度|字段说明|主键|默认值|
| :-: | :-: | :-: | :-: | :-: | :-: |
|id|bigint||主键|主键||
|username|varchar|100|用户名|||
|password|varchar|100|密码|||
|role|varchar|100|角色||管理员|
|addtime|timestamp||新增时间||CURRENT\_TIMESTAMP|


# 第四章  系统功能的具体实现
## 4.1 系统功能模块
校园志愿者管理系统，用户进入到系统首页，可以查看首页、活动信息、活动心得、公告信息、交流反馈、个人中心、后台管理等内容进行操作，如图4-1所示。

![](/md/blog.012.jpeg)

图4-1系统首页界面图

志愿者注册；在志愿者注册页面中输入用户名、密码、确认密码、姓名、年龄、邮箱、手机等内容完成注册操作；如图4-2所示。

![](/md/blog.013.jpeg)

图4-2志愿者注册界面图

活动信息；在活动信息页面中可以查看活动名称、活动类型、活动时间、人数、活动场地、活动介绍、图片等内容；并进行报名操作；如图4-3所示。

![](/md/blog.014.png)

图4-3活动信息界面图

活动心得；在活动心得页面中可以查看活动名称、图片、活动类型、发布时间、心得分享等内容，并进行评论或收藏操作；如图4-4所示。

![](/md/blog.015.png)

图4-4活动心得界面图

个人中心；在个人中心页面中输入用户名、密码、姓名、性别、上传图片、年龄、邮箱、手机等内容进行更新信息，并根据需要对我的收藏进行详细的操作管理，如图4-5所示。

![](/md/blog.016.png)

图4-5个人中心界面图

## 4.2管理员功能
管理员登录，通过填写注册时输入的用户名、密码、选择角色等信息进行登录操作，如图4-6所示。

![](/md/blog.017.jpeg)

图4-6管理员登录界面图

管理员登录进入校园志愿者管理系统可以查看首页、个人中心、志愿者管理、活动类型管理、活动信息管理、活动报名管理、活动通知管理、活动心得管理、交流反馈、系统管理等功能进行详细操作，如图4-7所示。

![](/md/blog.018.png)

图4-7管理员功能界面图

志愿者管理；在志愿者管理页面中可以查看索引、用户名、姓名、性别、头像、年龄、邮箱、手机等内容，并进行详情，修改和删除等操作；如图4-8所示。

![](/md/blog.019.png)

图4-8志愿者管理界面图

活动类型管理；在活动类型管理页面中可以查看索引、活动类型等内容，并进行修改、删除等操作；如图4-9所示。

![](/md/blog.020.png)

图4-9活动类型管理界面图

活动信息管理；在活动信息管理页面中可以查看索引、活动名称、活动类型、图片、活动时间、人数、活动场地等内容，并进行详情、修改或删除等操作；如图4-10所示。

![](/md/blog.021.png)

图4-10活动信息管理界面图

活动报名管理；在活动报名管理页面中可以查看索引、活动名称、活动类型、人数、报名说明、报名时间、用户名、姓名、手机、审核回复、审核状态、审核等内容，并进行详情、修改、通知和删除等操作；如图4-11所示。

![](/md/blog.022.png)

图4-11活动报名管理界面图

活动通知管理；在活动通知管理页面中可以查看索引、标题、用户名、姓名、手机、通知时间等内容，并进行详情、修改和删除等操作；如图4-12所示。

![](/md/blog.023.png)

图4-12活动通知管理界面图

活动心得管理；在活动心得管理页面中可以查看索引、活动名称、活动类型、图片、发布时间等内容，并进行详情、修改、查看评论和删除等操作；如图4-13所示。

![](/md/blog.014.png)

图4-13活动心得管理界面图

交流反馈；在交流反馈页面中可以查看索引、用户名、留言内容、留言图片、回复内容、回复图片等内容，并进行详情、修改和删除等操作；如图4-14所示。

![](/md/blog.024.png)

图4-14交流反馈界面图

系统管理；在公告信息页面中可以查看索引、标题、图片等内容，并进行详情，修改和删除等操作；还可以对轮播图管理进行详细操作；如图4-15所示。

![](/md/blog.025.png)

图4-15系统管理界面图

## 4.3志愿者功能
志愿者登录进入校园志愿者管理系统可以查看首页、个人中心、活动报名管理、活动通知管理、活动心得管理、我的收藏管理、交流反馈等功能进行详细操作，如图4-16所示。

![](/md/blog.026.png)

图4-16志愿者功能界面图

个人中心；在个人中心页面通过填写用户名、性别、头像、年龄、手机、姓名、邮箱等内容进行个人信息修改；如图4-17所示。

![](/md/blog.027.png)

图4-17个人中心界面图

活动报名管理；在活动报名管理页面中可以查看索引、活动名称、活动类型、人数、报名说明、报名时间、用户名、姓名、手机、审核回复、审核状态等内容，并进行详情、或删除等操作；如图4-18所示。

![](/md/blog.028.png)

图4-18活动报名管理界面图

活动通知管理；在活动通知管理页面中可以查看索引、标题、用户名、姓名、手机、通知时间等内容，并进行详情等操作；如图4-19所示。

![](/md/blog.029.png)

图4-19活动通知管理界面图

活动心得管理；在活动心得管理页面中可以查看索引、活动名称、活动类型、图片、发布时间等内容，并进行详情，修改，查看评论或删除等操作；如图4-20所示。

![](/md/blog.030.png)

图4-20活动心得管理界面图












