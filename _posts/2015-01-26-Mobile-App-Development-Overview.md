<style>
body{
	font: 13px/21px "Microsoft YaHei","宋体","Myriad Pro","Lato","Helvetica Neue",Helvetica,Arial,sans-serif;
	font-weight: 400;
	line-height: 21px;
	font-size: 14px;
}
h2,h3,h4 {
	font-weight: bold;
}
</style>
# 移动应用开发的三种模式
(本文档可以任意转载引用，文中图片可能不是原创，如果图片版权所有者反对使用，请及时与我联系)

<br />

## 移动操作系统的历史
--------

* 上世纪90年代，是PalmOS一统江湖的局面（超过90%的市场），拥有数十万的开发者队伍，并有数万款应用软件，采用其作为操作系统的PDA一度总销量达到数千万。
* 微软在1996年推出了嵌入式操作系统Windows CE，而PDA则是其重点发展方向。但和Windows的发展历程一样，一直到2000年推出Windows CE 3.0，微软才算初步取得成功。
* 在1996年推出了嵌入式操作系统Windows CE，而PDA则是其重点发展方向。但和Windows的发展历程一样，一直到2000年推出Windows CE 3.0，微软才算初步取得成功。2002年10月，将面向手机的Windows CE改名为Windows Mobile。
* Symbian的前身是EPOC，早在上世纪80年代就开始了，后来则被Nokia全额收购。Symbian提供了灵活的用户界面，来适应不同的用户需求。目前基于Symbian的用户界面有很多，主要是Series 60/80/90以及UIQ，而其中以Series 60所占的市场份额最大。本世纪出，Symbian一度占领了半壁江山。
* RIM的Blackberry，则是具有典型的企业应用特点，其最早于1999年开始提供服务，凭借其独步天下的Push Mail的概念，获得了欧美大量商务人士的厚爱。
* 2007年6月29日，是移动应用开发者应该记住的一个日子，Apple的iPhone在美国上市。2010年1月初，苹果公司宣布App Store应用程序下载量突破30亿。换句话说就是，仅在2009年一年，iPhone用户就从苹果的App Store上购买下载了25亿个应用程序。同时，苹果在2009年的全球市场份额已占到99.4%，这让苹果当仁不让地“稳坐”手机应用的“霸主”宝座。
* Google于2007年11月宣布推出基于Linux的开源操作系统：Android。
* 当然，在中国还有个不得不提到的MTK。

iOS之前那些陈芝麻烂谷子可能都没人想去关心了，下面是一副2005年~2013年，真正的智能移动操作系统的发展历史。

<p style="font-size:10px; color:#336699;">from http://infogr8.com/infographics/app-developers-alliance-mobile-os-history/</p>
![0](http://infogr8.com/wp-content/uploads/2014/04/AppAlliance_Mobile-OS-History-02.jpg)
<br />

## 目前的市场占有率
--------

　　调研机构Strategy Analytics最新的第三季度(2014年）报告中显示，Android以83.6%的市场占有率稳居移动操作系统市场之首。出货量为2.68亿，去年同期为2.06亿，市场份额由81.4%上升至83.6%。

　　苹果出货量虽然从上年同期的3380万上升到3930万，但是它的市场份额却由13.4%降到12.3%。Strategy Analytics认为下滑的原因是苹果没有占据低端手机市场，机型单一的苹果的确在占有率上无法与Android匹敌。

　　余下的市场则由Windows Phone和黑莓为主导。其中Windows Phone为3.3%，出货量为1050万部，略高于去年同期的1030万部，但份额却从4.1%跌至3.3%。

　　黑莓占0.7%，出货量从250万降至230万，份额也从1%滑落到0.7%。而剩下一些冷门的操作系统仅在最后的0.1%市场份额中挣扎。

![0](http://connectwww.com/wp-content/uploads/2014/11/Mobile-Operating-System-Market-share-October-2014.jpg)
<br />

### 2015年m-commerce market趋势

下面这个图有点意思，贴一下：
![1](https://tctechcrunch2011.files.wordpress.com/2015/01/mcommerce-market-map-2-02.png?w=1024&h=606)
<br />

## 开发平台
--------

* 在iOS和Android之前，以原生开发为主
* 跨平台的Java和QT也比较活跃
* 而iOS和Android出现后，伴随着软硬件的巨大进步，智能手机的上的应用功能甚至比PC上的还要复杂和强大，渐渐演化出三种开发模式

<br />

## 移动应用（Mobile APP）的三种开发模式
--------

* Native apps – the “real apps” with full access
  
	<p style="color: green;">Native apps live on the device。 They are developed specifically for one platform, and can take full advantage of all the device features。<p>

* Mobile Web Apps

	<p style="color: green;">Web apps are not real applications; they are really websites that, in many ways, look and feel like native applications, but are not implemented as such. They are run by a browser and typically written in HTML5. </p>

* Hybrid Apps

	<p style="color: green;">Hybrid apps are part native apps, part web apps. Like native apps, they live in an app store and can take advantage of the many device features available. Like web apps, they rely on HTML being rendered in a browser, with the caveat that the browser is embedded within the app.</p>

下图很清楚地解释了三种开发模式：
![2](http://img.brightcove.com/app-cloud-infographic.jpg)

**下面，我们先展示一份结论性的数据，介绍三种开发模式的差异，然后分别对三种开发模式做一些较为详细的说明。**

<br />

# 三种开发模式对比
--------

以下是一份来自dzone的表格，对三种模式的差异以及优劣解释的很清楚：

![3](http://java.dzone.com/sites/all/files/Screen%20Shot%202014-06-13%20at%205.05.49%20PM.png)

另一幅图：

![4](http://img.blog.csdn.net/20140107174159000)

还有个简单的：

![5](http://cms.csdnimg.cn/article/201303/18/514720de7c050.jpg)

HTML5跨平台，但用户体验不好；
Native用户体验好，但无法直接实现跨平台，升级运维工作量大；
Hybrid（混合模式），可以实现跨平台，用户体验也可以做的不错；

规律是，兼容性越强的技术，成本越低，性能越差；兼容性越差的技术，成本越高，性能越好。

# Mobile Web App 开发

这种模式比较简单，主要是HTML5/CSS3+Javascript开发，以网站的形式发布，可以是One-Page-Application，也可以由多个页面组成。
手机端则通过浏览器访问，和访问一般的网站没有区别。

使用HTML5和CSS3，可以绘制和展现较为丰富的UI元素，配合一些图片或者Icon字体，其视觉感受可以接近Native App，以HTML5/CSS3模拟原生UI的框架比比皆是（可以搜索 mobile HTML5 widgets)。而Javascript的大量使用，可以实现复杂的逻辑，也可以极大增强交互性，提升用户体验。

其局限性已经在上面大体说明，本文中也不再展开，需要强调以下三点：

1. Javascript在浏览器中运行，被限制在sandbox中，只有某些默许的系统功能可以调用
2. 移动浏览器环境有其特殊性，例如touch事件、像素，和PC端的开发还是有较大的区别
3. 不同平台浏览器兼容性问题仍然大量存在

<br />

## 参考文档
--------
以下列举一些文档供参考：

1. [It’s not a web app. It’s an app you install from the web](http://blog.forecast.io/its-not-a-web-app-its-an-app-you-install-from-the-web/ "It’s not a web app. It’s an app you install from the web")
2. [当前 WEB APP 开发的最佳实践](http://lyric.im/best-practice-for-web-app-development/)
3. [移动Web单页应用开发实践——页面结构化](https://github.com/maxzhang/maxzhang.github.com/issues/8)
4. [此像素非彼像素](http://www.w3cplus.com/css/A-pixel-is-not-a-pixel-is-not-a-pixel.html)
5. [Mobile Web 开发之百味良药](http://segmentfault.com/a/1190000000339907)

还有下面这个系列：

1. [Part 1: The viewport metatag](http://davidbcalhoun.com/2010/viewport-metatag)
2. [Part 2: The mobile developer’s toolkit](http://davidbcalhoun.com/2010/the-mobile-developers-toolkit-mobile-web-part-2)
3. [Part 3: Designing buttons that don’t suck](http://davidbcalhoun.com/2010/designing-buttons-that-dont-suck)
4. [Part 4: On designing a mobile webpage](http://davidbcalhoun.com/2010/on-designing-a-mobile-webpage)
5. [Part 5: Using mobile-specific HTML, CSS, and JavaScript](http://davidbcalhoun.com/2010/using-mobile-specific-html-css-javascript)
6. [Part 6: Dealing with device orientation](http://davidbcalhoun.com/2010/dealing-with-device-orientation)
7. [Part 7: Mobile JavaScript libraries and frameworks](http://davidbcalhoun.com/2010/mobile-javascript-libraries-and-frameworks)

# Native App 开发
\* 注意： 本文只是overview，每个主题都不会深入介绍。

<br />

## iOS
--------
iOS由于其封闭性，各版本之间的兼容性非常之好。而Apple的API做得也很好，尤其是官方文档，阅读的时候真是一种享受。网站是这个：
[iOS Dev Center](https://developer.apple.com/devcenter/ios/index.action)

初学者可以从这一篇开始了解：[Start Developing iOS Apps Today](https://developer.apple.com/library/ios/documentation/iPhone/Conceptual/iPhone101)，当然，你也可以任意选择一篇“快速入门”，比如这个[60分钟入门](http://blog.csdn.net/a451493485/article/details/9364867)，开发一个Hello World，iOS的神秘感立刻消失，接下来就可以慢慢研究了。

在程序猿的世界里，学习一门新技术都是差不多的套路，除了Hello World，欲对iOS开发有全局的认识，首先需要了解以下3个主题：

* 系统架构
* 开发语言和环境
* 如何测试和发布

<br />

### iOS系统架构
不多说，上几幅图：

![6](http://hi.csdn.net/attachment/201008/7/0_1281189503BwBH.gif)
![7](http://hi.csdn.net/attachment/201008/7/0_1281189549tYRd.gif)

<br />

### iOS开发语言和环境
据我了解，目前至少有6类语言能够开发iOS native app，相应地，它们都有不同的开发环境。

1. Objective-C + Xcode
2. Swift +　Xcode
3. C# + Xamarin
4. Java + ROBOVM, [网站请看这里](http://www.robovm.com/)
5. Python + kivy, [网站请看这里](http://kivy.org/#home)
6. Pascal + Delphi, [网站请看这里](http://www.embarcadero.com/products/rad-studio/android-ios-code-samples-xe7)

以下会对前三种做简要介绍。后三种鄙人实在没有时间去研究了。

<br />

#### Objective-C + Xcode
这就是官方最早的开发模式了，目前来看，也是使iOS App最优的开发模式（根据成本和输出成正比的关系，这种开发模式应该是最耗时的）。Objective-C就是我们经常说的OC，它扩展了ANSI C，是C的超集。OC和Xcode都是apple官方出品，专属MacOS的财产。是的，你给了自己一个购买Mac笔记本的理由，不过别得意，下面还有穷孩子的解决方案。

**有钱人方案：**

1. 购买一台Mac电脑，什么都OK，Mini，Book，Book Pro，iMac...，等我擦一下口水再接着写...
2. 购买iOS设备，各版本iPhone，各版本iPad，哦，对了，还可以准备买iWatch
3. 在mac电脑上下周Xcode
4. 安装iOS SDK和模拟器
5. 哦，对，也许还需要安装Interface Builder，是用来设计界面的
6. 可以开发了

**穷孩子方案**

1. 购买二手Mac电脑
2. 或者，用黑苹果，这个请到网上自行补课

还有个教程可参考[ios开发从入门到精通](http://wenku.baidu.com/course/view/1ce3571252d380eb62946d8c)。

<br />

####  Swift + Xcode
Swift，一种支持多编程范式，编译式编程语言，由苹果公司在2014年推出，用来撰写OS X和iOS应用程序[3]。2014年，在AppleWWDC所发布。苹果宣称Swift的特点是：快速、现代、安全、互动，而且明显优于Objective-C语言。Swift以LLVM编译，可以使用现有的Cocoa和Cocoa Touch框架。Xcode Playgrounds功能是Swift为苹果开发工具带来的最大创新，该功能提供强大的互动效果，能让Swift源代码在撰写过程中能实时显示出其运行结果。Swift在 Mac OS 和 iOS 平台可以和Object-C使用相同的运行时期(runtime)。这意味着Swift 程序可以运行于目前已存在的平台之上，包含 iOS 6 和 OS X 10.8 都可以运行Swift的程序.[7] 更重要的, Swift 和 Obj-C 的代码可并存于单一程序内, 这种延伸就如同C 和 C++ 的关系一样。

Swift is an innovative new programming language for Cocoa and Cocoa Touch. Writing code is interactive and fun, the syntax is concise yet expressive, and apps run lightning-fast. Swift is ready for your next iOS and OS X project — or for addition into your current app — because Swift code works side-by-side with Objective-C. 参考[这里](https://developer.apple.com/swift/)。
![8](https://devimages.apple.com.edgekey.net/swift/images/swift-screenshot.jpg)

<br />

#### C# + Xamarin
Xamarin 是由早期的Mono项目（这个请自行补课，简单来说.NET虚拟机在Linux上的开源实现）演变而来，原本是在Linux上执行C#程序的一个开放原始码项目。后来陆续发表支持iOS的Mono Touch framework以及Mono For Android Framework。因此它在市场上并不是一个新的产品。2011年，原本在Novell的Mono项目团队独立成立一家公司，正式将名称改为Xamarin。 

不看不知道，一看吓一跳，Xamarin老强大了，帮众有四大天王：

![9](images/xamarinproducts.png)

两个图，供参考：

- 跨平台

![跨平台](https://i-msdn.sec.s-msft.com/dn394307.img_32(zh-tw,MSDN.10).jpg)

- 系统架构示意图

![系统架构示意图](https://i-msdn.sec.s-msft.com/dn394307.img_33(zh-tw,MSDN.10).jpg)

Xamarin Studio可以安装在Windows 7或者Mac上，它能做这些事情：

![10](images/xamarincando.png)

不幸的是，Xamarin在Windows下开发需要商业版或者更高版本。不多说了，参考以下几个网站：

1. [Xamarin官网](http://xamarin.com/)

	页面视觉设计方面不错，感觉挺高大上的。是的，你没看错，我还是骑着那台烂车。。。哦，不是唱歌，我想说的是，你没看错，还是响应式的布局。Banner上那个build、test、monitor的文字变化还挺好玩。

2. [跨平台实战](https://msdn.microsoft.com/zh-tw/vstudio/dn394307.aspx)

	MSDN tw 文档。

3. [Hello Mamarin](http://blogs.msdn.com/b/msdntaiwan/archive/2013/09/11/visual-studio-app-hello-xamarin.aspx)

	还是MSDN。

### 测试和发布

iOS应用可以通过虚拟机测试，这一点在上面的文章中都有讲解，不再赘述。

在真机测试，则有以下几种选择（摘抄自[这里](http://blog.csdn.net/a451493485/article/details/9364867))：

-  加入苹果的Developer Program，成为付费会员，有了这个付费会员资格，就可以直接在Xcode中点击”Run”将刚刚改过的代码编译打包安装到开发测试用的iOS设备上。在iOS真机上操作被测试的程序能激活Xcode中设置的断点。
- 越狱iOS设备。将iPhone和iPad越狱后，可以通过SSH直接上传Xcode编译好的ipa包（一个iOS App本质上就是一个ipa包）。
- 越狱的iOS设备，配合破解过的Xcode，甚至可以实现和付费开发者计划一样的功能：在Xcode上点击”Run”，就自动编译安装到iOS设备上去运行了企业部署方案。

关于申请账号、安装证书，同样可以参考相关文章。

<br />

## Android
--------

Android分支版本太多了，很多厂商都做了扩展。我们这里只简要说明官方版本的android开发。

<br />

### Android系统架构

**TODO:解释体系架构**

官方提供的图，颜色很重：

![11](http://img.blog.csdn.net/20130524105706838)

<br />

### 开发语言和环境

至少有3个：

1. Java + Android Strudio（or ADT）
2. C++ + NDK
3. C# + Xamarin

前两个都是官方提供的，下面简要介绍一下第一个。

<br />

#### Java + Android Studio
首先还是不能错过的[官方网站](http://developer.android.com/index.html)。 现在打头的是“Lollipop”版本。
新的IDE，即Android Strudio是基于IntelliJ平台做的，体验不错：

![12](images/studio-hero.png)

如果某些情况还需要ADT，可参考这个：[Android ADT开发环境搭建](https://software.intel.com/zh-cn/blogs/2014/02/27/android)

Android是大众消费，对平台没什么挑剔的，Windows下跑的欢着呢，随便找个Step By Step就能做个Hello World。不过，对我天朝子民，Android开发最麻烦的地方就是官网上不去啊，因此，有大神给出了方案：[收集整理Android开发所需的方方面面](https://github.com/inferjay/AndroidDevTools)，类似的网站应该还有，一个断了还可以试试其他。

下面就推荐一些文档：

1. Java的沾边的东西，IBM怎么会错过

	[Android 开发从入门到精通(比较老,不过还是有参考价值）](http://www.ibm.com/developerworks/cn/opensource/theme/android/)
2. 有人整理了一堆资料，我就贴个链接好了

	[Android开发之旅：书籍、教程、工具和各种干货](http://blog.jobbole.com/73026/)。
	<p>顺便说一句，这个伯乐在线是个不错的网站，有事没事扫三眼。</p>

3. 优酷上的视频，没看过

	[Android开发视频教程（重制版）](http://www.youku.com/playlist_show/id_19518970.html?sf=40600)


### 测试和发布

同iOS一样，测试也有模拟器，在使用IDE的时候，自然会用到。

在手机上测试也非常简单：

1. 首先要安装驱动。我是在电脑上安装了豌豆荚，手机连接到电脑上就提示安装驱动，豌豆荚会自动寻找与手机对应的驱动，很简单的。
2. 手机的USB调试模式打开（例如小米：设置->开发人员选项->USB调试）。
3. 在eclipse中，选择window -> show view -> other->Android->device， 在device界面中选择你手机的名字就行了。
4. 直接run程序就可以在手机上看到效果了。

<TODO:发布到商城>

# Hybrid App 开发
<TODO：脖子疼了，改天继续>
