---
title: android常用框架
date: 2016-06-15 14:42:18
tags:
---
# 综合框架(orm、ioc、http,图片处理)
##  1、andbase开发框架
* **项目下载地址(1)：**https://github.com/zhaoqp2010/andbase
* **项目下载地址(2)：** http://www.amsoft.cn/article/view-429.html   （带有效果图）
* andbase中包含了大量的开发常用手段。
  如网络下载，多线程与线程池的管理，数据库ORM，图片缓存管理，图片文件下载上传，Http请求工具，SOAP工具类，异步Task，常用工具类（字符串，日期，文件处理，图片处理工具类等），能够使您的应用在团队开发中减少冗余代码，很大的提高了代码的维护性与开发高效性，能很好的规避由于开发疏忽而导致常犯的错误。
* andbase封装了大量的常用控件。
  如list分页，grid分页，下拉刷新，进度框，图片轮播，表格，多线程下载器，侧边栏，图片上传，轮子选择，图表，Tab滑动，日历选择器等。
* 强大的AbActivity，您没有理由不继承它。
  继承它你能够获得一个简单强大可设置的操作栏，以及一系列的简单调用，如弹出框，提示框，进度框，副操作栏等。
* 提供效率较高图片缓存管理策略，使内存大幅度节省，利用率提高，效率提高。
  程序中要管理大量的图片资源，andbase提供简单的方法，几步完成下载与显示，并支持缩放，裁剪，缓存功能，OOM不再有。
* 封装了大量常见工具类。
  包括日期，字符，文件，图片，数学，View万能适配工具类等各种处理函数， 多而全。
* 用andbase大量减少handler的使用，而采用回调函数，代码更整洁。
  handler会产生大量代码，并且不好维护，andbase对handler进行了封装，你会发现用了andbase基本代码中不会再有大量的handler判断语句。
* 简单轻量支持注解自动建表的ORM框架（支持一/多对多的关联操作）。
  写sql，建表，工作量大，andbase提供更傻瓜异步增删改查工具类，数据库在内置卡和外置卡都可以。
* 异步请求http框架，网络请求标准化，支持文件上传下载，get，post，进度显示。
  包含了异步与http请求的工具类，SOAP请求工具类，简单实用。
+ <!-- more -->

## 2、xUtils开发框架
* **xutils地址：**https://github.com/wyouflf/xUtils
* **xutils3地址：**https://github.com/wyouflf/xUtils3
* xutils已更新到xutils3 ，xutils3 重构了xutils很多ＡＰＩ
* xutils3包含了很多实用的android工具.
* xutils3支持超大文件(超过2G)上传，更全面的http请求协议支持(11种谓词)，拥有更加灵活的ORM，更多的事件注解支持且不受混淆影响...
xutils3最低兼容Android 4.0 (api level 14). (Android 2.3?)
xutils3变化较多所以建立了新的项目不在旧版(github.com/wyouflf/xUtils)上继续维护, 相对于旧版本:
HTTP实现替换HttpClient为UrlConnection, 自动解析回调泛型, 更安全的断点续传策略.
支持标准的Cookie策略, 区分domain, path...
事件注解去除不常用的功能, 提高性能.
数据库api简化提高性能, 达到和greenDao一致的性能.
图片绑定支持gif(受系统兼容性影响, 部分gif文件只能静态显示), webp; 支持圆角, 圆形, 方形等裁剪, 支持自动旋转...


## 3、Afinal开发框架
* **Afinal地址：**https://github.com/yangfuhai/afinal
* Afinal 是一个android的sqlite orm 和 ioc 框架。同时封装了android中的http框架，使其更加简单易用；
* 使用finalBitmap，无需考虑bitmap在android中加载的时候oom的问题和快速滑动的时候图片加载位置错位等问题。
* Afinal的宗旨是简洁，快速。约定大于配置的方式。尽量一行代码完成所有事情。
* FinalDB模块：android中的orm框架，一行代码就可以进行增删改查。支持一对多，多对一等查询。
* FinalActivity模块：android中的ioc框架，完全注解方式就可以进行UI绑定和事件绑定。无需findViewById和setClickListener等。
* FinalHttp模块：通过httpclient进行封装http数据请求，支持ajax方式加载。
* FinalBitmap模块：通过FinalBitmap，imageview加载bitmap的时候无需考虑bitmap加载过程中出现的oom和android容器快速滑动时候出现的图片错位等现象。FinalBitmap可以配置线程加载线程数量，缓存大小，缓存路径，加载显示动画等。FinalBitmap的内存管理使用lru算法，没有使用弱引用（android2.3以后google已经不建议使用弱引用，android2.3后强行回收软引用和弱引用，详情查看android官方文档），更好的管理bitmap内存。FinalBitmap可以自定义下载器，用来扩展其他协议显示网络图片，比如ftp等。同时可以自定义bitmap显示器，在imageview显示图片的时候播放动画等（默认是渐变动画显示）。

## 4、LoonAndroid 
* **项目地址：**https://github.com/gdpancheng/LoonAndroid
*   (1)  自动注入框架（只需要继承框架内的application既可）
*   (2)  图片加载框架（多重缓存，自动回收，最大限度保证内存的安全性）
*   (3)  网络请求模块（继承了基本上现在所有的http请求）
*   (4)  eventbus（集成一个开源的框架）
*   (5)  验证框架（集成开源框架）
*   (6)  json解析（支持解析成集合或者对象）
*   (7)  数据库（不知道是哪位写的 忘记了）
*   (8)  多线程断点下载（自动判断是否支持多线程，判断是否是重定向）
*   (9)  自动更新模块
*   (10) 一系列工具类



# 数据库
##  1、DBFlow
* **项目地址：**https://github.com/Raizlabs/DBFlow
* **中文文档：** https://github.com/VankaIn/DBFlow_CN
* **Demo**    https://github.com/taoweiji/DBFlowExample
* DBFlow目的是把其他ORM的数据库最好的优点集合在一起，而且将它们进一步优化。DBFlow不只是让你知道如何解决你的功能上的问题，而且它使你容易处理Android上的数据库。让我们好好利用DBFlow，使我们尽可能的把程序写的最好。
* **可扩展性：**Model 是一个接口，无需子类，但为了方便起见，我们建议使用 BaseModel。你可以不继承任何Model类在不同的包中的类，并把它们作为你的数据库表。你也可以继承其他Model然后同时加入@Column，他们又可以在不同的packages中。此外，在该库的子类对象，能满足您的需求。（翻译不好）
* **速度:**这个库内置Java的注释处理代码生成，有几乎为零的运行时性能（反射是主要的，生成的数据库模块的构造方法）。该库通过生成的代码，你可以节省样板代码和维护时间。凭借强大的模式高速缓存（多主键Model 也行），你可以通过重复使用，在这里可能超过SQLite的速度。我们支持延迟加载，如支持@ForeignKey或@OneToMany，使查询发生的速度超快。
* **SQLite流式查询:**此库中的查询尽可能坚持SQLite的原生查询， select(name, screenSize).from(Android.class).where(name.is("Nexus 5x")).and(version.is(6.0)).querySingle()
开源:该库是完全开源，不仅欢迎贡献，而且鼓励。
* **强大: **我们支持触发器，模型视图，索引，迁移，在同一个线程中，内置的数据库请求队列执行操作，还有更多的功能。。。
* 多个数据库，多个模块:我们无缝支持多个数据库文件，数据库模块，在同一时间。
* 基于SQLite:SQLite是世界上最广泛使用的数据库引擎。。。。。
* SQLCipher【本地数据库加密】支持
* 支持Kotlin 扩展

## 2、OrmLite
* **官网地址：** http://ormlite.com/
* **github地址：** https://github.com/j256/ormlite-android
* **Getting started:**http://ormlite.com/javadoc/ormlite-core/doc-files/ormlite_1.html#Getting-Started
* OrmLite 不是 Android 平台专用的ORM框架，它是Java ORM。支持JDBC连接，Spring以及Android平台。语法中广泛使用了注解（Annotation）。
*  **支持SQLCipher【本地数据库加密】**
*  **github地址** https://github.com/wobuaihuangjun/ormlite-sqlcipher
*  **项目DEMO** https://github.com/sierpito/demo-ormlite-with-sqlcipher


## 3、LitePal
*  **github地址:** https://github.com/wobuaihuangjun/ormlite-sqlcipher
*  **DEMO:** https://github.com/LitePalFramework/LitePalTest
*  **详细教程博客：**http://blog.csdn.net/sinyu890807/article/category/2522725
*  litepalAndroid是一个开源库，允许开发者使用SQLite数据库变得极其简单。你可以在线完成大部分的数据库操作甚至无需编写SQL语句，包括创建或升级表、CRUD操作，聚合函数等。
* 使用对象关系映射(ORM)图案。
* 几乎“零配置”(只有一个配置文件很少的性质)。
* 用于维护所有表自动地(例如创建、改变或删除表)。
* 封装的API用于避免书写SQL语句。
* Awesome流利的查询API。
* 可替换的选择，仍然使用SQL，但是更容易和比原件更好的API。
* 更引人注目。


## 4、greenDAO 
* **gitHub地址：**https://github.com/greenrobot/greenDAO
* **官网地址:**http://greendao-orm.com/
* greendao是一个开源的类库(Android)提供一个易于使用的接口到SQLite数据库的数据以帮助开发人员处理有效地减轻了开发人员从数据库处理低级别要求，同时节省了开发时间。SQLite是一个不错的嵌入式数据库。尽管如此，编写SQL语句和查询的解析结果是相当繁重且耗时的任务。您省去这些greendao通过Java对象映射到数据库表(通常称为ORM)。用这种方法你可以存储、更新、删除和查询用于Java对象的使用一个简单的面向对象的API。
* 最大性能最快的orm(Android)；我们的基准都是开放源码的太
* 易于使用强大的API的覆盖关系和加入
* 最小内存消耗
* 小库大小(<100KB),以保持您的构建时间且避免在65K限制方法
* 数据库加密支持：greendaosqlcipher保持用户数据的安全
* 强大的社区：超过4.000GitHub五角星表示强烈和活跃的社区


## 6、activeandroid
* **gitHub地址：**https://github.com/pardom/ActiveAndroid
* **官网地址:**http://www.activeandroid.com/
* Active Record（活动目录）是Yii、Rails等框架中对ORM实现的典型命名方式。Active Android 帮助你以面向对象的方式来操作SQLite。。

## 7、sugar ORM 
* **gitHub地址：**https://github.com/satyan/sugar
* **官网地址:**http://satyan.github.io/sugar/index.html
* 用超级简单的方法处理Android数据库
* 数据库的创建
* 简单的API来操纵你的业务对象

## 8、android-lite-orm 
* **gitHub地址：**https://github.com/litesuits/android-lite-orm
* **官网地址:** http://litesuits.com/?form=gorm
* LiteOrm是一个小巧、强大、比系统自带数据库操作性能快1倍的 android ORM 框架类库，开发者一行代码实现数据库的增删改查操作，以及实体关系的持久化和自动映射。

## 9、realm
* **官网地址** https://realm.io/cn/
* 移动数据库：一个SQLite和ORM的替换品
* 支持 （Java、Objective—C、swift、React Native 、Xamarin ）


#  网络请求

##  1、volley
 * **官网地址**https://github.com/smanikandan14/Volley-demo
 * Google推出了官方的针对Android平台上的网络通信库，能使网络通信更快，更简单，更健壮
 * Volley在提供了高性能网络通讯功能的同时，对网络图片加载也提供了良好的支持
 * 1、封装了的异步的RESTful 请求API；
 * 2、一个优雅和稳健的请求队列；
 * 3、一个可扩展的架构，它使开发人员能够实现自定义的请求和响应处理机制；
 * 4、能够使用外部HTTP Client库；
 * 5、缓存策略；
 * 6、自定义的网络图像加载视图（NetworkImageView，ImageLoader等);

## 2、android-async-http  
* **项目地址：**https://github.com/loopj/android-async-http
* **文档介绍：**http://loopj.com/android-async-http/ 
*  (1) 在匿名回调中处理请求结果
*  (2) 在UI线程外进行http请求
*  (3) 文件断点上传
*  (4) 智能重试
*  (5) 默认gzip压缩
*  (6) 支持解析成Json格式
*  (7) 可将Cookies持久化到SharedPreferences

## 3、okhttp
* **官方地址：**http://square.github.io/okhttp/
* ** gitHub ** https://github.com/square/okhttp
* HTTP是应用现代网络。它告诉我们如何与媒体交换数据。做HTTP负载使助力你的东西快和节省带宽。
* okhttp是HTTP客户端，通过有效的默认值：
* HTTP/2支持允许所有的请求到相同主机共享一个插座。
* 连接池减少等待时间请求（如HTTP/2没有可用的)。
* 透明gzip下载尺寸收缩。
* 响应高速缓存避免了将网络完全用于重传请求。
* okhttp坚守当网络是麻烦：它会悄然恢复从常见的连接问题。如果你的服务有多个IP地址okhttp试图替换地址，如果第一次连接失败。这是对于IPv4+IPv6服务，已在中心托管的冗余数据。okhttp发起新的TLS连接与现代特征(SNI，alpn)，并且落回到TLS1.0如果握手失败。
* 使用okhttp是容易的。其请求/响应API设计流畅和永恒性的建设者。它同时支持同步阻塞调用和异步调用的回调。
* okhttp支持安卓2.3及以上。对于Java，最低要求是1.7。

## 4、android-lite-http
* **gitHub地址：**https://github.com/litesuits/android-lite-http
* **官网地址:** http://litesuits.com/?form=gorm
* litehttp是一种简单、灵活和智能的AndroidHTTP框架。你可以用litehttphttp请求只写一行代码！它可以转换一个Java模型参数和兰德作为一个JSON响应Java模式的智能化水平




#   图片加载及处理
##  1、Android-Universal-Image-Loader
* **项目地址：** https://github.com/nostra13/Android-Universal-Image-Loader
*  Android-Universal-Image-Loader是一个开源的UI组件程序，该项目的目的是提供一个可重复使用的仪器为异步图像加载，缓存和显示
* 多线程的图片加载(Async或Sync)
* imageloader定制的配置(线程执行下载器、解码器、存储器和磁盘缓存，显示图像的选项，等等。）
* 定制选项的每一个显示呼叫图像(短轴图像缓存，解码选项、位图的处理和显示等。)
* 图像缓存存储器中和/或磁盘上的文件的系统(设备或SD卡)
* 装载过程（包括监听下载进度）
*  **效果图** ![enter image description here](https://raw.githubusercontent.com/nostra13/Android-Universal-Image-Loader/master/UniversalImageLoader.png)
## 2、 picasso
* **项目地址：** https://github.com/square/picasso 或 http://square.github.io/picasso/
* picasso是Square公司开源的一个Android图形缓存库；可以实现图片下载和缓存功能。仅仅只需要一行代码就能完全实现图片的异步加载：
	
## 3、Glide
* **项目地址：** https://github.com/bumptech/glide
* Glide 是一个 Android 上的图片加载和缓存库，其目的是实现平滑的图片列表滚动效果。


## 4、Fresco 
* **项目地址：** http://www.fresco-cn.org/或https://github.com/facebook/fresco
* Fresco 是一个强大的图片加载组件。
* Fresco 中设计有一个叫做 image pipeline 的模块。它负责从网络，从本地文件系统，本地资源加载图片。为了最大限度节省空间和CPU时间，它含有3级缓存设计（2级内存，1级文件）。
* Fresco 中设计有一个叫做 Drawees 模块，方便地显示loading图，当图片不再显示在屏幕上时，及时地释放内存和空间占用。
* Fresco 支持 Android2.3(API level 9) 及其以上系统。

## 5、picasso-transformations
* **项目地址：** https://github.com/wasabeef/picasso-transformations
* picasso-transformations是一个图像转换类库，为Picasso（强大的图片下载和缓存开源软件）提供各种各样的图像转换。
* **效果图**
*   ![enter image description here](https://github.com/wasabeef/picasso-transformations/blob/master/art/demo.gif?raw=true)


## 6、glide-transformations
* **项目地址：** https://github.com/wasabeef/glide-transformations
* 一个基于Glide的transformation库，拥有裁剪，着色，模糊，滤镜等多种转换效果
* **效果图**
*  ![enter image description here](https://github.com/wasabeef/glide-transformations/blob/master/art/demo.gif?raw=true)

## 7、GlidePalette
* **项目地址：** https://github.com/florent37/GlidePalette
* 一个可以在Glide加载时很方便使用Palette的库
* **效果图**
* ![enter image description here](https://raw.githubusercontent.com/florent37/GlidePalette/master/screenshot/night_small_2.png)


## 8、android-gpuimage
* **项目地址：** https://github.com/CyberAgent/android-gpuimage
* 实现各种各样图像滤镜（图像处理）效果，多达50多种效果，基本囊括了最常见的图像处理效果。包括：contrast，hue，gamma，brightness，sharpness，emboss，saturation，exposure，shadow，blend等等。 由于需要用到OpenGL ES 2.0，所以，仅能在真机中测试。可以载入本地相册的照片或者直接拍照后进行照片处理。

## 9、基于android-gpuimage 开发项目
* **android-instagram-filter **
* 基于gpuimage的android图片滤镜，实现instagram效果。
* **项目地址：** https://github.com/sangmingming/android-instagram-filter
* **android-instagram-image-filter**
* 模仿instagram的滤镜（和in的滤镜类似
* **项目地址：**https://github.com/imrunning/android-instagram-image-filter
* **效果图** 
* ![enter image description here](https://raw.githubusercontent.com/imrunning/android-instagram-filter/master/Screenshot/Screenshot_2015-03-13-09-13-15.png)
