

## 1\.  Retrofit　　
In a word: Retrofit is a type-safe network framework based on HTTP protocols that serves Android and java languages

Reason for the list: Retrofit topped the list with 21.8k stars and android sub-titles.

The official address http://square.github.io/retrofit/

github https://github.com/square/retrofit

Author: square team

use:

compile 'com.squareup.retrofit2:retrofit:2.3.0'


## 2\.okhttp

In a word: okhttp is a network framework based on HTTP and HTTP2.0 protocols that serves java and android clients

For reasons of being on the list, okhttp finished second with a 20.4k stars and android subheadings. Large companies such as Taobao also package okhttp. Retrofit 2.0 began to build a built-in okhttp framework, Retrofit focused on packaging interface to complete business requirements, okhttp focused on the security and efficiency of network requests, the author will distinguish between the two, is to let later learners know that this is two sets of frameworks, learning the principles of the framework can be learned separately, so as not to understand confusion.

The official address http://square.github.io/okhttp/

github https://github.com/square/okhttp

Author: square team

use:

compile 'com.squareup.okhttp3:okhttp:3.8.0'

## 3\.Butter Knife

In a word: Butter Butter provides the ability to generate template code using annotations to bind views to methods and parameters.

Reason for listing: 16.5K star on github, along with the Butter Knife plug-in from Android Studio, helps developers save on frequent findviewbyids, and the latest Butter Knife offers onclick bindings and string initialization, and beginners can check out Butter's Ander Knife and Knife Knife plug-ins for further learning!

Official address:http://jakewharton.github.io/butterknife/

github：https://github.com/JakeWharton/butterknife

Author: Jake Wharton is also a member of the Square team

use:

dependencies {
  compile 'com.jakewharton:butterknife:8.6.0' annotationProcessor 'com.jakewharton:butterknife-compiler:8.6.0' }

## 4\.MPAndroidChart

In a word: MPAndroidChart is a chart framework

Reason to be on the list: 16.1K star on github for quick and concise. Powerful and well-known chart frame

The official address https://github.com/PhilJay/MPAndroidChart

github https://github.com/PhilJay/MPAndroidChart

Author: Phil Jay

use:

1. Add Gladle Dependence to AS

Add on the build.gradle of the root:

allprojects {
      repositories {
          maven { url "https://jitpack.io" }
      }
  }
Add on the app's build.gradle:

dependencies {
      compile 'com.github.PhilJay:MPAndroidChart:v3.0.2' }

##5. glide

In a word: glide is a "picture loading and caching framework" focused on providing smooth slicing power

Reason to be on the list: 15.9k star, the number one frame for image loading class frameworks, and google's 2014 developer conference, the camera app was developed based on the gilde framework

github https://github.com/bumptech/glide

Author Bump Technologies team

use:

[! (Copy code) (//common.cnblogs.com/images/copycode.gif)] (javascript:void(0); "Copy Code")
repositories {
  mavenCentral()
}

dependencies {
    compile 'com.github.bumptech.glide:glide:3.8.0' compile 'com.android.support:support-v4:19.1.0' }
[! (Copy code) (//common.cnblogs.com/images/copycode.gif)] (javascript:void(0); "Copy Code")


##6.leakcanary

In a word: a memory detection framework for java and android clients

Reason for listing: Convenience and simplicity are the biggest features of leakcanary, and you can use it directly by simply integrating it in the app's app, and 15.5k stars show how popular it is

github https://github.com/square/leakcanary

Author square team

Use:

 dependencies {
   debugCompile 'com.squareup.leakcanary:leakcanary-android:1.5.1' releaseCompile 'com.squareup.leakcanary:leakcanary-android-no-op:1.5.1' testCompile 'com.squareup.leakcanary:leakcanary-android-no-op:1.5.1' }
Write in Application:

[! (Copy code) (//common.cnblogs.com/images/copycode.gif)] (javascript:void(0); "Copy Code")
public class ExampleApplication extends Application {

  @Override public void onCreate() {
    super.onCreate(); if (LeakCanary.isInAnalyzerProcess(this)) { // This process is dedicated to LeakCanary for heap analysis. // You should not init your app in this process.
      return;
    }
    LeakCanary.install(this); // Normal app init code...
 }
}
[! (Copy code) (//common.cnblogs.com/images/copycode.gif)] (javascript:void(0); "Copy Code")

##7.Android-Universal-Image-Loader

In a word: Once the picture loaded frame king, android development veterans have used it

Reasons to be on the list: Android-side picture loading frame big brother, 15.3k star is enough to prove its popularity, the biggest difference between UIL and gilde is customizable, UIL provides a large number of configuration methods, picture loading status callbacks (success, failure, in progress), loading animation, etc.; But the author still recommends you to use!

github https://github.com/nostra13/Android-Universal-Image-Loader

Author nostra13

use:

Download the address universal-image-loader-1.9.5 .jar


##8.EventBus

In a word: EventBus is a framework for communication between local components

Reason for listing: Intercombusitive communication framework star volume first: 14.8k, in large projects Activities, fragments, Threads, Services can see its use scenario, although EventBus in the delivery of events to uninstaled components is somewhat limited, only suitable for "living" components to pass messages, but still does not prevent it from being active in the various scenarios of large projects.

The official address http://greenrobot.org/eventbus/documentation/how-to-get-started/

github https://github.com/greenrobot/EventBus

Author greenrobot

use:

compile 'org.greenrobot:eventbus:3.0.0'

##9.zxing

In a word: Barcode image processing library

Reason for listing: If you've used QR codes, you've definitely used the famous zxing indirectly. 13.9K of star volume, let it ranked ninth in this list, really, if you have the need to understand the QR code, you may wish to understand, modify its source code to start.

github https://github.com/zxing/zxing

Author Sean Owen


##10.picasso

In a word: powerful picture download, cache framework

Reason for listing: The third picture category framework appears in this list, the difference is that picasso more emphasis on image download, you can integrate picasso into your project, you can also combine gilde and UIL and picicasso, all three packaged into your project, on demand.

The official address http://square.github.io/picasso/

github https://github.com/square/picasso

Author square team

use:

compile 'com.squareup.picasso:picasso:2.5.2'
Or download it

Jar package


##11.lottie-android

In a word: A framework that quickly shows the animation of Adobe Afeter Effect (AE) tools on the Android side

Reason for the list: Animation frame first place, github on 13.3k star proved his superiority, the use of json files to quickly achieve animation effects is its greatest convenience, and this json file is also provided by AdobeAfter Effects (AE) tool, in AE installed a Bodymovin plug-in, using this plug-in to eventually generate animation effects json file, This johnson file can be parsed by LottieAnimationView and generated brilliant animations. And it supports cross-platform yo.

github https://github.com/airbnb/lottie-android

Author: Airbnb Team


##12.fresco

In a word: A framework that manages picture memory

Reason for the list: 12.8k star on the github, fourth in the picture category, Facebook's origin proves that it is not a re-created wheel, in the field of managing image memory has its own world, progressive loading, loading gif is its unique features compared to the top three

Official address: https://www.fresco-cn.org/

github https://github.com/facebook/fresco

Author facebook

use:

dependencies { // 其他依赖
  compile 'com.facebook.fresco:fresco:0.12.0' }
The following dependencies need to be added on demand:

[! (Copy code) (//common.cnblogs.com/images/copycode.gif)] (javascript:void(0); "Copy Code")
dependencies { // 在 API < 14 上的机器支持 WebP 时，需要添加
  compile 'com.facebook.fresco:animated-base-support:0.12.0'

  // 支持 GIF 动图，需要添加
  compile 'com.facebook.fresco:animated-gif:0.12.0'

  // 支持 WebP （静态图+动图），需要添加
  compile 'com.facebook.fresco:animated-webp:0.12.0' compile 'com.facebook.fresco:webpsupport:0.12.0'

  // 仅支持 WebP 静态图，需要添加
  compile 'com.facebook.fresco:webpsupport:0.12.0' }
[! (Copy code) (//common.cnblogs.com/images/copycode.gif)] (javascript:void(0); "Copy Code")


##13.RxAndroid

In a word: A framework for asynchronous communication between Android client components

Reason for listing: 12.7k star on github, second in the component communication framework, only after EventBus, if you want to ask the difference between the two, Eventbus is used to replace the cumbersome Interface between components, RxAndroid is used to replace Ansy Task, not conflict;

github https://github.com/ReactiveX/RxAndroid

By Jake Wharton

use:

compile 'io.reactivex.rxjava2:rxandroid:2.0.1'
compile 'io.reactivex.rxjava2:rxjava:2.1.0'

##14.SlidingMenu

In a word: Side-slip menu bar frame

Reason to be on the list: The Upper Paleo Frame, named after Userval-Image-loader, gives your app the ability to slide the menu bar The github flash has more than 10.5k stars, proving its enduring durability, and even with Google's launch of NavigationDrawer, it hasn't reduced developers' support for Silding Menu, a classic that has not been updated in four years; too many apps have used it, and you can see it on the open source license for the software!

github https://github.com/jfeinstein10/SlidingMenu

By Jeremy Feinstein

use:

Fork source code on gihub, integrated into the project


##15.PhotoView

In a word: An ImageView presentation framework that supports zooming and responding to gestures

Reason for listing: 10.3k star number, located in the picture category frame ranking fifth, PhotoView and the top four are different from this time bring the picture display ability, you must be curious about WeChat's avatar click amplification is how to achieve, many app pictures show how to respond to gesture press, understand PhotosoView, you will be happy! (I won't tell you that ImageView's click-amplification effect is also available on Android's ample)

github https://github.com/chrisbanes/PhotoView

Author: chrisbanes

use:

[! (Copy code) (//common.cnblogs.com/images/copycode.gif)] (javascript:void(0); "Copy Code")
在app根目录的build.gradle中加入：
allprojects {
    repositories {
        maven { url "https://jitpack.io" }
    }
}
在app的module目录的build.gralde中加入：

dependencies {
    compile 'com.github.chrisbanes:PhotoView:latest.release.here' }
[! (Copy code) (//common.cnblogs.com/images/copycode.gif)] (javascript:void(0); "Copy Code")
use

[! (Copy code) (//common.cnblogs.com/images/copycode.gif)] (javascript:void(0); "Copy Code")
<com.github.chrisbanes.photoview.PhotoView
    android:id="@+id/photo_view" android:layout_width="match_parent" android:layout_height="match_parent"/>

 PhotoView photoView = (PhotoView) findViewById(R.id.photo_view);
photoView.setImageResource(R.drawable.image);
[! (Copy code) (//common.cnblogs.com/images/copycode.gif)] (javascript:void(0); "Copy Code")


##16.material-dialogs

In a word: A custom dialog framework

Reason for listing: 9.9k star, the third custom View framework after PhotosoView, SlidingMenu, maybe you're still a new to custom View, and you're a little rusty with Dialog, which you can use to improve your Dellaog usage

github https://github.com/afollestad/material-dialogs

By Aidan Follestad

use:

dependencies { // ... other dependencies here
    compile 'com.afollestad.material-dialogs:core:0.9.4.5'
}


##17.Android-async-http

In a word: A network framework based on asynchronous requests based on http protocols,

Reason to be on the list: While you have countless reasons to use retrofit and okhttp, 9.8k star proves it's still worth learning. It's worth noting that it's also been two years since it's been updated, and you're taking it when you're lazy for a reason!

github https://github.com/loopj/android-async-http

By James Smith

use:

[! (Copy code) (//common.cnblogs.com/images/copycode.gif)] (javascript:void(0); "Copy Code")
repositories {
  maven {
    url 'https://oss.sonatype.org/content/repositories/snapshots/' }
}
dependencies {
  compile 'com.loopj.android:android-async-http:1.5.0-SNAPSHOT' }
[! (Copy code) (//common.cnblogs.com/images/copycode.gif)] (javascript:void(0); "Copy Code")


##18.androidannotations

In a word: A fast development framework based on annotations

Reason for listing: Like Butterknife, annotations are used to quickly complete the initialization of view, except that androids offer more capabilities: simple threading models, etc.;

The official address http://androidannotations.org/

github https://github.com/androidannotations/androidannotations

Author: Wonder Csabo


##19.fastjson

In a word: A framework based on json parsing and generation

Reason for listing: From its name is not difficult to see, fast is its biggest feature, Alibaba's origin to ensure the quality and superiority of the code, 9.4k star number, is also the first chinese open source framework in the list, involving the network of apps will use johnson, fastjson is worthy of your first choice!

github https://github.com/alibaba/fastjson

Author: alibaba

use:

compile 'com.alibaba:fastjson:1.1.58.android'


##20.Material-Animations

In a word: An animated framework that provides the ability to transition scene transformation

Reason for listing: Android Animation Frames came in second place, with 9.3k stars, and unlike lottie-android, which ranks first on the Animation Frames list, Material-Animations offers animated effects for scene switching. Some of Transition's (transition animation) presentations are already available on Android's official website, and as beginners find it difficult to quickly expand into their projects, Material-Animations' examples save developers the hassle of copying them directly into their own apps.

github https://github.com/lgvalle/Material-Animations

Author: Luis G. Valle

use:

Down source code, modify learning


##21.tinker

In a word: It is WeChat's Android hot patch solution

Reason for listing: 9.1k star, WeChat in use of hot patch scheme, heartbeat is not as good as action

The official address http://www.tinkerpatch.com/Docs/intro

github https://github.com/Tencent/tinker

Author: Tencent


##22.ViewPagerIndicator

In a word: An open source framework based on ViewPager's page indicator

Reason for listing: The ancient artifact, although it has not been updated for five years, but you can still see its use in Taobao and other apps, 8.9K of star volume let it stand in the list

The official address http://viewpagerindicator.com/

github https://github.com/JakeWharton/ViewPagerIndicator

By Jake Wharton

use:

Download the address https://github.com/JakeWharton/Android-ViewPagerIndicator/zipball/master


##23.Android-CleanArchitecture
In a word: a demo that explains the design framework

Reason for listing: It's not a framework, you can think of it as a book that will teach you how to design a clean architecture, and there's a sample app in the project that, with graphics explaining, gives you a deeper understanding of the architecture of Android clients. The number of stars of 8.8k proves that it is a "good book".

github https://github.com/android10/Android-CleanArchitecture

Author: Fernando Cejas


##24..Android-PullToRefresh
In a word: A view framework that provides a refresh UI for normal views

Reason for listing: 8.2K's star number makes it the top refresh class UI framework, powerful compatibility capabilities, the framework supports ListView, GrdiView, WebViewScrollView, ViewPager and many other Views to increase refresh capabilities, if you have the need to increase pull-up load, drop-down load, you should consider it!

github https://github.com/chrisbanes/Android-PullToRefresh

Author: Chris Banes

use:

Github fork source code, integrated into the project

##25.flexbox-layout
In a word: an elastic scaling layout

Reasons to go: 8.1k star, front-end H5 developer turn to android development gospel, Flexbox Layout as a replacement for Linear Layout and RelativeLayout, worth a try, along with Constrat Layout.

github https://github.com/google/flexbox-layout

Author: Google

use:

dependencies {
    compile 'com.google.android:flexbox:0.3.0-alpha3' }
##26.AndroidSwipeLayout
In a word: Very powerful sliding layout

Reason for listing: Sliding delete is a common demand for domestic apps, product details of the up and down sliding demand as developers we also often encounter, Android SwitchLayout on the github has 8K star, proving that it has stood the test, you are worth a try

github https://github.com/daimajia/AndroidSwipeLayout

Author: Daimajia

use:

dependencies {
    compile 'com.android.support:recyclerview-v7:21.0.0' compile 'com.android.support:support-v4:20.+' compile "com.daimajia.swipelayout:library:1.2.0@aar" }
or download

AndroidSwipeLayout-v1.1.8.jar

##27.realm-java
In a word: Realm is a mobile database framework

Reason for listing: The core data engine, C, is built much faster than a regular Sqlite database. The author speculates that this is exactly what realm puts before greenDao (7877), the famous database framework, with 7,892 star numbers

Official address:https://realm.io/cn/

github https://github.com/realm/realm-java

Author: Realm Team

Use:https://realm.io/docs/java/latest/

##28.greenDAO
In a word: greenDAO is an efficient and fast SQLIte database

Reason for listing: greenDAO's star quantity and Realm, and EventBus division out of the same door, is also developed and maintained by the greenrobot team, quality assurance, but if the author Realm and GreenDao are both good and bad, can only be specific to the actual use of the use of the simulation line, high-intensity testing can be judged, so we can not say a word, deeply regret

Official address:http://greenrobot.org/greendao/

github https://github.com/greenrobot/greenDAO

use:

[! (Copy code) (//common.cnblogs.com/images/copycode.gif)] (javascript:void(0); "Copy Code")
buildscript {
    repositories {
        jcenter()
        mavenCentral() // add repository
 }
    dependencies {
        classpath 'com.android.tools.build:gradle:2.3.1' classpath 'org.greenrobot:greendao-gradle-plugin:3.2.2' // add plugin
 }
} -----

apply plugin: 'com.android.application' apply plugin: 'org.greenrobot.greendao' // apply plugin
 dependencies {
    compile 'org.greenrobot:greendao:3.2.2' // add library
}
[! (Copy code) (//common.cnblogs.com/images/copycode.gif)] (javascript:void(0); "Copy Code")

##29.stetho
In a word: An open source framework that provides the ability to debug Android apps on Chrome developer tools

Reason for listing: In ancient times, Android programmers to debug the local database, need to go into Android Device Monitor to find /data/data/com.xxx.xxx/databases inside the db file, exported to the PC side, with the PC's data tools to view, now use stetho Save such trouble; today's Android programmers want to debug the network request response process of the message paragraph, need to add Log statement in the request, a message one information printed out, quite cumbersome, now please use stetho, save such trouble put! 7.8K star number, the vast number of Android developers debugging the gospel, you deserve it!

作者：FaceBook

官网地址： http://facebook.github.io/stetho/

github https://github.com/facebook/stetho

使用：

compile 'com.facebook.stetho:stetho:1.5.0'

##30.BaseRecyclerViewAdapterHelper
一句话介绍：强大、流畅的Recyvlerview通用适配器

上榜理由：如果你是RecyclerView的拥簇者，你一定要体验这款专门服务该view的适配器，7.7K个star，让这个家伙位于github上Android 适配器排行榜第一，还有很多惊喜等你去探寻！

官网地址：http://www.recyclerview.org/

作者：陈宇明以及他的小伙伴

使用：

[![复制代码](//common.cnblogs.com/images/copycode.gif)](javascript:void(0); "复制代码")
allprojects {
    repositories {
        ...
        maven { url "https://jitpack.io" }
    }
}

dependencies {
        compile 'com.github.CymChad:BaseRecyclerViewAdapterHelper:VERSION_CODE' }
[![复制代码](//common.cnblogs.com/images/copycode.gif)](javascript:void(0); "复制代码")


##31.AndroidViewAnimations
一句话介绍：一款提供可爱动画集合的框架

上榜理由：正如作者所说，它囊括了开发需求过程中所有的动画效果，集成进了这个简洁可爱的动画框架。7.6K的star数，证明了它在动画框架领域的战斗力，让它仅仅位列lottie-android和Material-Animations两个动画框架霸主之后，屈居第三名

github https://github.com/daimajia/AndroidViewAnimations

作者：daimajia

使用：

dependencies {
        compile 'com.android.support:support-compat:25.1.1' compile 'com.daimajia.easing:library:2.0@aar' compile 'com.daimajia.androidanimations:library:2.2@aar' }
sample：

YoYo.with(Techniques.Tada)
    .duration(700)
    .repeat(5)
    .playOn(findViewById(R.id.edit_area));
	
##32. MaterialDrawer
一句话介绍：强大的塑料风格的抽屉框架

上榜理由：7.6K的star数量，作者的持续更新状态，如果你还在犹豫上手SlidingMenu遇到bug没人管的困境，那么你可以入手它作为你的抽屉布局

github https://github.com/mikepenz/MaterialDrawer

作者：Mike Penz

使用:

compile('com.mikepenz:materialdrawer:5.9.2@aar') {
    transitive = true }
new DrawerBuilder().withActivity(this).build();

##33.Android-ObservableScrollView
一句话介绍：一款让视图滑动更具有视觉效果的滑动式框架

上榜理由：7.5K的star数量，证明了它曾经的价值，github上提供了12种滑动效果，你可以用它弥补其他框架的不足，提升你的App体验！

github https://github.com/ksoichiro/Android-ObservableScrollView

作者：Soichiro Kashima

使用：

compile com.github.ksoichiro:android-observablescrollview

##34.CircleImageView
一句话介绍：圆角ImageView

上榜理由：也许你已经听说过无数种展示圆角图片的方法，但如果你不尝试尝试CircleImageView，那么你的知识库会因为少了它黯然失色，有的时候完成需求是开发者优先考虑的，不同实现方法牵扯到的性能差异更值得让人深思，如果你有心在图片性能上有所涉猎，那么CircleImageView绝对不会让你败兴而归。最后别忘了记得去看Romain Guy的建议哟。

github https://github.com/hdodenhof/CircleImageView

作者：Henning Dodenhof

使用：

dependencies {
    ...
    compile 'de.hdodenhof:circleimageview:2.1.0' }
[![复制代码](//common.cnblogs.com/images/copycode.gif)](javascript:void(0); "复制代码")
<de.hdodenhof.circleimageview.CircleImageView
    xmlns:app="http://schemas.android.com/apk/res-auto" android:id="@+id/profile_image" android:layout_width="96dp" android:layout_height="96dp" android:src="@drawable/profile" app:civ_border_width="2dp" app:civ_border_color="#FF000000"/>
[![复制代码](//common.cnblogs.com/images/copycode.gif)](javascript:void(0); "复制代码")


##35.logger
一句话介绍：一款让log日志优雅显示的框架

上榜理由：logger作为调试框架，并未给出很强大的能力，它最大的亮点是优雅的输出log信息，并且支持多种格式：线程、Json、Xml、List、Map等，如果你整日沉迷于汪洋大海般的log信息不能自拔，logger就是你的指路明灯！6.6k个star让他位列调试框架第二名，屈居facebook的stetho之后

github https://github.com/orhanobut/logger

作者：Orhan Obut

使用：

compile 'com.orhanobut:logger:2.1.1'
Logger.d(MAP);
Logger.d(SET);
Logger.d(LIST);
Logger.d(ARRAY); Logger.json(JSON_CONTENT);
Logger.xml(XML_CONTENT);


##36.agera
一句话介绍:一款服务于Android平台的响应式编程框架

Reason for the list: Google has launched a responsive programming framework for Android developers, which is lighter than RxJava RxAndroid, which topped the list of responsive programming frameworks, and the biggest difference between the two is that the imager is based on push event, pull data (VS Rx series data push).

github https://github.com/google/agera

Author: Google

use:

  compile 'com.google.android.agera:agera:1.3.0'
Expand your capabilities

  compile 'com.google.android.agera:content:1.3.0' compile 'com.google.android.agera:database:1.3.0' compile 'com.google.android.agera:net:1.3.0' compile 'com.google.android.agera:rvadapter:1.3.0' compile 'com.google.android.agera:rvdatabinding:1.3.0'

##37.BottomBar
In a word: A bottom navigation bar view frame

Reason for listing: The king frame in the bottom column, the number of 6.3K star, proves its excellence, fully follows the material design specifications, very convenient to get started. If the shortcomings, can not set the spacing between icon and titile, can not customize the size of the view, etc. , but these can be resolved by modifying the source code, the author also modified a set of domestic developers in line with the bottom navigation framework, will be open source.

github https://github.com/roughike/BottomBar

Author: Iiro Krankka

use:

compile 'com.roughike:bottom-bar:2.3.1'


##38.Calligraphy
In a word: A custom font frame

Reason for listing: If you're still fretting about modifying all font styles in the app with one click, 6.3K star Calligraphy is worth having, it can modify the entire project's Textview font at the same time, or you can set a textview font separately, and wait for something, try it!

github https://github.com/chrisjenx/Calligraphy

Author: Christopher Jenkins

use:

dependencies {
    compile 'uk.co.chrisjenx:calligraphy:2.3.0' }

##39.AndroidSlidingUpPanel
In a word: Draggable slide panel view frame

Reason to be on the list: If your project requires a drag-and-drop sliding panel (showing some details, playing music, map information, etc.), then it's recommended that you use it, 6.3k star, from startup umano, to prove that it's a masterpiece

github https://github.com/umano/AndroidSlidingUpPanel

Author: umano

use:

[! (Copy code) (//common.cnblogs.com/images/copycode.gif)] (javascript:void(0); "Copy Code")
dependencies {
    repositories {
        mavenCentral()
    }
    
    compile 'com.sothree.slidinguppanel:library:3.3.1' }
[! (Copy code) (//common.cnblogs.com/images/copycode.gif)] (javascript:void(0); "Copy Code")

##40.AppIntro
In a word: A framework that provides a quick welcome page

Reason for listing: I never intended to put the welcome page framework into the leaderboard, as a domestic developer, ViewPager development app welcome page is already a hand-in-hand demand, why an open source welcome page framework will have 6.3k star on github? Perhaps you will be dismissive, yes, often in the moment of disdain, the opportunity slipped away.

github https://github.com/apl-devs/AppIntro

Author: Paolo Rotolo

[! (Copy code) (//common.cnblogs.com/images/copycode.gif)] (javascript:void(0); "Copy Code")
 allprojects {
        repositories {
            ...
            maven { url 'https://jitpack.io' }
        }
    }
    
    dependencies {
            compile 'com.github.apl-devs:appintro:v4.2.0' }
[! (Copy code) (//common.cnblogs.com/images/copycode.gif)] (javascript:void(0); "Copy Code")

##41.recyclerview-animators
一句话介绍：一款为Recyclerview提供扩展动画能力的框架

上榜理由：有一句老话：如果有天你失去对新事物的兴趣，那就说明你老了。recyclerview已经推出快三年了，还在用listview的人们，是否已经发掘自己渐渐变老；不要灰心，快为你的项目加入recyclerview-animators框架吧，为“自己”加入新鲜的血液和能量！（笔者备注：6.2K个star）

github https://github.com/wasabeef/recyclerview-animators

作者；https://github.com/wasabeef

使用：

dependencies { // jCenter
  compile 'jp.wasabeef:recyclerview-animators:2.2.6' }


##42.dagger
一句话介绍：一款通过依赖注入降低程序间耦合的开发框架

上榜理由：github 上dagger1版本 有6.2k个star ， dagger2版本有7.3k个；由square完成的dagger1版本，到如今google团队接手的dagger2版本，强力开发团队保证了代码在设计上的优越性；如果你想探究Android 领域的设计模式，这也是不错的选择。

官网地址：https://google.github.io/dagger/

github ：https://github.com/google/dagger

作者：google

使用：

[![复制代码](//common.cnblogs.com/images/copycode.gif)](javascript:void(0); "复制代码")
dependencies {
  compile 'com.google.dagger:dagger:2.x' annotationProcessor 'com.google.dagger:dagger-compiler:2.x' }
If you're using classes in dagger.android you'll also want to include:

compile 'com.google.dagger:dagger-android:2.x' compile 'com.google.dagger:dagger-android-support:2.x'
annotationProcessor 'com.google.dagger:dagger-android-processor:2.x'
[![复制代码](//common.cnblogs.com/images/copycode.gif)](javascript:void(0); "复制代码")


##43.Android-Bootstarp
一句话介绍：一款提供在Android应用上实现Bootstrap（web框架）所作出效果的框架

上榜理由：榜单上第二款响应web技术的Android 端框架，还记得第一名是谁吗——flexbox-layout，作为Android开发者，你有必要去了解Web技术了。5.9k个star，证明它不容小觑

github https://github.com/Bearded-Hen/Android-Bootstrap

作者:Bearded-Hen团队

使用：

dependencies {
   compile 'com.beardedhen:androidbootstrap:{X.X.X}' }
   
   
##44.RxBinding
一句话介绍：一款提供UI组件事件响应能力的框架

上榜理由：如果你还未开始RxAndroid 之旅，RxBinding可以作为你的第一站，通过RXBinding，你将理解响应式编程的快乐，让项目里的事件流程更清晰。5.6K个star，RxAndroid作者亲自操刀，快来试用吧！

github https://github.com/JakeWharton/RxBinding

作者：JakeWharton

[![复制代码](//common.cnblogs.com/images/copycode.gif)](javascript:void(0); "复制代码")
Platform bindings:

compile 'com.jakewharton.rxbinding2:rxbinding:2.0.0'
'support-v4' library bindings:

compile 'com.jakewharton.rxbinding2:rxbinding-support-v4:2.0.0'
'appcompat-v7' library bindings:

compile 'com.jakewharton.rxbinding2:rxbinding-appcompat-v7:2.0.0'
'design' library bindings:

compile 'com.jakewharton.rxbinding2:rxbinding-design:2.0.0'
'recyclerview-v7' library bindings:

compile 'com.jakewharton.rxbinding2:rxbinding-recyclerview-v7:2.0.0'
'leanback-v17' library bindings:

compile 'com.jakewharton.rxbinding2:rxbinding-leanback-v17:2.0.0'
[![复制代码](//common.cnblogs.com/images/copycode.gif)](javascript:void(0); "复制代码")


##45.ListViewAnimations
一句话介绍：一款为ListView提供动展示画效果能力的框架

上榜理由：如果有一天我承认自己老了，我还会排排我的兄弟——ListView，证明我和它一起战斗过。ListViewAnimations的存在就是证明我们这些“老年人”仍有用武之地，也许你有说不出口的难处，无法体会到RecyclerView里动画的快乐，拥有ListViewAnimations，你一样可以骄傲的说，我的孩子（每个item）也有自己的动效啦。（笔者备注 5.6K个star）

github https://github.com/nhaarman/ListViewAnimations

作者：nhaarman

使用：

[![复制代码](//common.cnblogs.com/images/copycode.gif)](javascript:void(0); "复制代码")
repositories {
    mavenCentral()
}

dependencies {
    compile 'com.nhaarman.listviewanimations:lib-core:3.1.0@aar' compile 'com.nhaarman.listviewanimations:lib-manipulation:3.1.0@aar' compile 'com.nhaarman.listviewanimations:lib-core-slh:3.1.0@aar' }
[![复制代码](//common.cnblogs.com/images/copycode.gif)](javascript:void(0); "复制代码")


##46.UItimateRecyclerView
一句话介绍：一款提供刷新、加载更多、动画特效等额外能力的RecyclerView框架

上榜理由：榜单上第三次出现RecyclerView的身影，足以证明RecyclerView的优异性，5.5K个star，框架里所提供众多的能力，如果你是个功利开发者，那么此框架会为你节省很多学习时间，它可以完成多item式布局的大多数需求，值得注意的是，这个项目也是在其他项目的思路上二次开发的。

github https://github.com/cymcsg/UltimateRecyclerView

作者：MarshalChen

使用：

[![复制代码](//common.cnblogs.com/images/copycode.gif)](javascript:void(0); "复制代码")
repositories {
    jcenter()
    }
dependencies {
    ...
    compile 'com.marshalchen.ultimaterecyclerview:library:0.7.2' }
[! (Copy code) (//common.cnblogs.com/images/copycode.gif)] (javascript:void(0); "Copy Code")

##47.uCrop
In a word: an elegant picture crop frame

Reason to be on the list: 5.3K star, picture editing module single out is also an elegant app.

github https://github.com/Yalantis/uCrop

Author: Yalantis

use:

[! (Copy code) (//common.cnblogs.com/images/copycode.gif)] (javascript:void(0); "Copy Code")
allprojects {
   repositories {
      jcenter()
      maven { url "https://jitpack.io" }
   }
}

compile 'com.github.yalantis:ucrop:2.2.1' 
[! (Copy code) (//common.cnblogs.com/images/copycode.gif)] (javascript:void(0); "Copy Code")


##48.RxJava-Android-Samples
In a word: An app that describes the RxJava usage scenario

Reason for listing: The first open source project to appear on the list, "Just to show you how to use another project", can be said to be an use case for RxJava, and the unexpected use of RxJava you can't think of here, which is why it stands on this list with 5.2k star. Regret that you didn't create such a sought-after demo? Get started and write another "XX project use case."

github https://github.com/kaushikgopal/RxJava-Android-Samples

Author: kaushikgopal

use:

Clone explore locally



##49.AndroidAutoLayout
In a word: A framework that provides adaptability

Reason for listing: 5.2K star, Hongyang brother's work, suitable for small project development team, to get the design MM px pixel design is not a headache pinch? This frame has a lot of shortcomings in one-click fixes to your problem, but on the way to perfect fit, you're worth exploring and understanding it! The author does not recommend it to be applied to the project has matured to run, after all, there are too many adaptation solutions on the market, fit problem is like a big mess, want to fry a plate of good dishes, you have to prepare a variety of condiments (fit small program), when you put all kinds of small condiments with the fire pure green, you are not far from the food chef.

github https://github.com/hongyangAndroid/AndroidAutoLayout

Author: Zhang Hongyang

use:

dependencies {
    compile 'com.zhy:autolayout:1.4.5' }
	
	
##50.EffectiveAndroidUI
In a word: a teaching app that explains the efficient display of UI

Reason for listing: Programming novices are difficult to MVC MVP, MVVM and other models have a deep understanding, if there is an example app, it will be of great benefit to beginners, the author encountered it is also met late. 4.8K star, proved that it has been tested and examined by the vast number of developers, of which the Effective UI programming ideas are in line with the official Android course of the Effective UI course, and this project also contains frogment, dagger, theme style, Butterknife and many other small knowledge points, as a programming beginner's learning use case can not be more suitable

github https://github.com/pedrovgs/EffectiveAndroidUI

Author: Pedro Vicente

use:

Clone project to local



##51.Luban
In a word: the closest wechat picture compression framework

Reason for listing: Good ideas always make you shine, Luban only with a single function of picture compression, captured 4.8K star, proved that it is in the picture compression, it may not be the best, but it is to make you and I closest to the great project

github https://github.com/Curzibn/Luban

Author: Curzibn

use:

compile 'top.zibin:Luban:1.1.1'


##52.DroidPlugin
In a word: a popular plug-in development framework

Reason for listing: 4.8K star, plug-in framework list first place, 360 team production, frame quality assurance, success story - 360 mobile phone assistant, and continuous maintenance

github https://github.com/DroidPluginTeam/DroidPlugin/blob/master/readme_cn.md

Author: Andy Zhang

use:

Clone project to local


##53. otto
In a word: an old and powerful event bus framework

Reason for listing: 4.8K star, an event-responsive framework previously introduced by the Square team, and the event-driven framework of Taobao app, which is now recommended for developers to replace Otto with RxJava Rx Android. But Otto still has the value of horizontal comparison with EventBus, and vertically, the differences between otto and square's own Rx series framework are also worth exploring.

github https://github.com/square/otto

Author: square

use:

repositories {
    mavenCentral()
    maven { url "https://oss.sonatype.org/content/repositories/snapshots/" }
}

compile 'com.michaelpardo:activeandroid:3.1.0-SNAPSHOT'


##54.u2020
In a word: an app that provides an advanced teaching example for Dagger (well, the name is a bit around)

Reasons to go on the list: 4.7K star, Jake Wharton-led teaching app that teaches you how to use Dagger in other advanced frameworks, showing Dagger's advanced use with butterKnife, Retrofit, Moshi, Picasso, Okhttp, RxJava, Madge, LeakCanar and many others. You can also learn from your own projects

github https://github.com/JakeWharton/u2020

By Jake Wharton


##55.buck
In a word: Buck is a fast build system

Reason for the list: The author of facebook-google, his excellent understanding of building code, coupled with the maintenance of large teams, and the speed and efficiency of incremental updates make buck the first choice for WeChat Android team building projects, which are faster than gladle when building large projects, but small and medium-sized companies are not suitable for this framework, but as people who aspire to do something in framework design, welcome to explore the matter

Official address:https://buckbuild.com/

github https://github.com/facebook/buck

Author: Facebook

use:

linux or mac system  +docs


##56.PermissionsDispatcher
In a word: An annotation-based framework that provides solutions to runtime hazard rights scenarios

Reason for listing: Since Android 6.0 Google proposed the word dangerous permissions, user security has been mentioned to a certain height, some of the runtime user's more dangerous permissions will no longer be automatically obtained by developers, need to be approved by users, developers can continue to use the right, if you have been subject to permission issues scratching your ears, it is recommended that you try this framework, it is enough to solve your problem

Official address:https://hotchemi.github.io/PermissionsDispatcher/

github https://github.com/hotchemi/PermissionsDispatcher

By Shintaro Katafuchi

use:

[! (Copy code) (//common.cnblogs.com/images/copycode.gif)] (javascript:void(0); "Copy Code")
dependencies {
  compile('com.github.hotchemi:permissionsdispatcher:${latest.version}') {
      exclude module: "support-v13" }
  annotationProcessor 'com.github.hotchemi:permissionsdispatcher-processor:${latest.version}' }  repositories {
  jcenter()
  maven { url 'http://oss.jfrog.org/artifactory/oss-snapshot-local/' }
}
[! (Copy code) (//common.cnblogs.com/images/copycode.gif)] (javascript:void(0); "Copy Code")


##57.android-gif-drawable
In a word: A view frame that provides the ability to display GIF animation

Reason for listing: According to my survey of the famous domestic app - know the use of android-gif-drawable, so proved its value, although in the 11th on the list introduced lottie-android direct application of AE animation examples, but AE designers are not every company equipped with, GIF existence, there must be the need to display GIFs, it is worth your possession!

github https://github.com/koral--/android-gif-drawable

Author: Karol Wrótniak

use:

[! (Copy code) (//common.cnblogs.com/images/copycode.gif)] (javascript:void(0); "Copy Code")
repositories {
    mavenCentral()
    maven { url "https://oss.sonatype.org/content/repositories/snapshots" }
}
dependencies {
    compile 'pl.droidsonroids.gif:android-gif-drawable:1.2.+' }
[! (Copy code) (//common.cnblogs.com/images/copycode.gif)] (javascript:void(0); "Copy Code")


##58.Apktool
In a word: a tool to decompile apk

Reason for listing: Open source anticompiling tool, for each of you who aspire to understand apk reverse cracking, worth having, 4.5k star, reverse crack apk artifact!

github https://github.com/iBotPeaches/Apktool

Official address:https://ibotpeaches.github.io/Apktool/

By Connor Tumbleson


##59.dynamic-load-apk
In a word: plug-in development framework

Reason for listing: 4.5k star, located in the second place in the plug-in development framework (first from the 360 team), comprehensive documentation so that you can quickly start plug-in development, if you like the large text explanation, then this project must be suitable for you

github：https://github.com/singwhatiwanna/dynamic-load-apk

Author: singwhatiwanna

use:

The documentation on github is more coordinated with the author's blog



##60.atlas
In a word: Taobao launched the component development framework

Reason for listing: Taobao team out of the boutique, atlas framework to provide understanding of coupling, components, dynamic development capabilities, 4.5k star let him rank first in the component development framework

github https://github.com/alibaba/atlas

Author: alibaba


##61.volley
In a word: Google recommends using the Android-side web request framework

Reason for listing: 4.4k star, not that he is not good enough, but the use of volley has gradually become the habit of the vast number of developers

github https://github.com/google/volley (new volley address)

Author: google

use:

Clone source to local

##62.androidmvp
In a word: a demo that showcases Android Mvp designs

Reason to be on the list: There are a handful of projects on the list that get 4.2K star simply by showing a design model, and if you're going to try mvp, androidmvp can be your outpost

github https://github.com/antoniolg/androidmvp

Author: Antonio Leiva

use:

clone to local

##63.SwipeBackLayout
In a word: A frame that lets you close a page with a swipe gesture

Reason for listing: imitation WeChat sliding out of the current chat interface effect, providing the ability to slide off the action, through this idea, to achieve the swipe off of fragment easily; The author insists on suggesting that you clone source to explore locally; 4.2k star proves that many people love it

github https://github.com/ikew0ng/SwipeBackLayout

Author: ike_w0ng

use:

compile 'me.imid.swipebacklayout.lib:library:1.0.0'


##64.FlycoTabLayout
In a word: A framework that allows for a wide variety of indicator effects

Reason for listing: Although there is no reason why we should integrate a 2.5M dependency library to add page indicator functionality to an app, as a good framework for understanding the principles of the design of the viewpager or swip views indicator, you are worth opening it to try, and the author suggests splitting the required source code separately and adding it to your project. 4.1K star, secondary development works, still recommended!

github https://github.com/H07000223/FlycoTabLayout

Author: Flyco


##65.android-testing
In a word: a demo that showcases four automated test framework use cases (Espresso, UiAutomator, Android JunitRunner, JUnit4)

Reason for listing: Learners often get caught up in the seemingly unknowable situation, and if you're lucky enough to take a course at Android Testing Support Library Site, you'll be desperate for android's four test frameworks, and this demo is perfect for you

github https://github.com/googlesamples/android-testing

Author: Googlesampes Team


##66.FileDownloader
In a word: an efficient, stable, flexible, easy-to-use file download engine

Reason for listing: 4.1k proves how popular it is, file download seems simple behind how many pit points hidden, I know you have the ability to implement their own file download function, but excellent framework can enhance your design coding ability, this framework can enhance your strength!

github https://github.com/lingochamp/FileDownloader

Author: Lingo Chap team

use:

dependencies {
    compile 'com.liulishuo.filedownloader:library:1.5.5' }

##67.JieCaoVideoPlayer
In a word: A multimedia playback framework based on MediaPlayer api, VideoView

Reason for the list: The third multimedia playback framework in the list, it is in a dexterous posture squeezed into this list, exquisite is its greatest advantage, less than 100k, with it, you can quickly develop video playback like today's headlines, 4k star, prove it is worth a try

github https://github.com/lipangit/JieCaoVideoPlayer

Author: Nathan

use:

compile 'fm.jiecao:jiecaovideoplayer:5.5.4'


##68.glide-transformations
In a word: For many famous picture loading frames to provide the picture shape changeability of the frame

Reason for listing: At the top of the list has introduced glide, Picasso, Fresco and other image loading frameworks, glide-transformations is a framework that provides them with image deformation capabilities, very simple to use, so it is loved by everyone, github has 3.8K star

github https://github.com/wasabeef/glide-transformations

Author: Daichi Furiya

use:

[! (Copy code) (//common.cnblogs.com/images/copycode.gif)] (javascript:void(0); "Copy Code")
repositories {
    jcenter()
}

dependencies {
    compile 'jp.wasabeef:glide-transformations:2.0.2'
    // If you want to use the GPU Filters
    compile 'jp.co.cyberagent.android.gpuimage:gpuimage-library:1.4.1' }
[! (Copy code) (//common.cnblogs.com/images/copycode.gif)] (javascript:void(0); "Copy Code")
Set the variation effect in Glide

Set Glide Transform.

Glide.with(this).load(R.drawable.demo)
        .bitmapTransform(new BlurTransformation(context))
        .into((ImageView) findViewById(R.id.image));


##69.android-gpuimage
In a word: An OpenGL-based image rendering engine

Reason for listing: Put down GpuImage's honor on the IOS platform, Android's android-gpuimage offers more than 70 image rendering effects, and you're wondering how the Meitu show is making picture changes? With it, nothing is a problem. If you're an engineer in the Matte tool class, the idea of building this framework will also be of great benefit to you. The author also imitated the Meitu app through android-gpuimage and captured his girlfriend's heart, once again praised its strength. The ios version of the plus android version, with a total of 19k stars, has proved its strength, what are you waiting for?

github：https://github.com/CyberAgent/android-gpuimage

Author: CyberAgent team

use:

[! (Copy code) (//common.cnblogs.com/images/copycode.gif)] (javascript:void(0); "Copy Code")
repositories {
    jcenter()
}

dependencies {
    compile 'jp.co.cyberagent.android.gpuimage:gpuimage-library:1.4.1' }
[! (Copy code) (//common.cnblogs.com/images/copycode.gif)] (javascript:void(0); "Copy Code")
More retrofits, as well as reading Ios' programming documentation, are highly recommended for small partners with perseverance!


##70.RxPermissions
In a word: A framework for completing permission requests based on RxJava

Reason for listing: The second rights-to-service framework on the list, based on RxJava's design, allows you to concentrate on your business, and 3.7K star has proven its useful value

github https://github.com/tbruyelle/RxPermissions

By Thomas Bruyelle

use:

[! (Copy code) (//common.cnblogs.com/images/copycode.gif)] (javascript:void(0); "Copy Code")
repositories {
    jcenter() // If not already there
}

dependencies {
    compile 'com.tbruyelle.rxpermissions:rxpermissions:0.9.4@aar' }
[! (Copy code) (//common.cnblogs.com/images/copycode.gif)] (javascript:void(0); "Copy Code")
Elegant use:

[! (Copy code) (//common.cnblogs.com/images/copycode.gif)] (javascript:void(0); "Copy Code")
RxPermissions rxPermissions = new RxPermissions(this);

rxPermissions
    .request(Manifest.permission.CAMERA)
    .subscribe(granted -> { if (granted) { // I can control the camera now
        } else { // Oups permission denied
 }
    });
[! (Copy code) (//common.cnblogs.com/images/copycode.gif)] (javascript:void(0); "Copy Code")

##71.freeline
In a word: A dynamically replaced compilation build framework

Reason for listing: Following Facebook's Buck and Androdi's official Instagram account, Ant-Man has launched the Freeline compilation framework, which claims that Freeline is still several times faster than the industry's mainstream build-up; The compilation speed is not in the list of ranking factors, so freeline with 3.7 stars, temporarily ranked second in the compilation framework

Official address:https://www.freelinebuild.com/

github：https://github.com/alibaba/freeline

Author: alibaba

use:

[! (Copy code) (//common.cnblogs.com/images/copycode.gif)] (javascript:void(0); "Copy Code")
buildscript {
    repositories {
        jcenter()
    }
    dependencies {
        classpath 'com.antfortune.freeline:gradle:0.8.7' }
}
apply plugin: 'com.antfortune.freeline'

android {
    ...
}
File → Settings... → Plugins → Browse repositories →freeline.

[! (Copy code) (//common.cnblogs.com/images/copycode.gif)] (javascript:void(0); "Copy Code")


##72.RxLifecycle
In a word: A framework that provides the ability to manage the lifecycle capabilities of Activity and Fragment during the use of RxJava

Reason for listing: At the top of the list, you already know the power of RxJava and Rx Android, but some careless developers because they didn't cancel their subscriptions in time to cause a serious memory leak, don't worry, RxLifecycle can solve your problems, on gtihub has 3.7K star, well-known domestic software - know and Taobao are also using it

github https://github.com/trello/RxLifecycle

Author: Team trello

use:

Clone source to local


##73.classyshark
In a word: an executable browser

Reason for listing: The second apk reverse tool after Apktool in the list, if you like elegant graphical data display, then you must not miss him, classyshark can crack the results to graphical display users, easy analysis, 3.7K star, let it temporarily ranked apk reverse tool second place!

github https://github.com/google/android-classyshark

Author: google

use:

Download JAR


##74.acra
In a word: A framework that provides the ability to log app crash logs

Reason for listing: If you're faced with the need to collect APP crash logs, acra is a good choice. 3.7K star, let acra ranked first in the crash log framework leaderboard, acra has enough ability to record online APP, and sent back to the service side, acra also provides a pretty good crash log statistics service end framework Acralyzer,cralyzer works on top of Apache CouchDB, so in addition to CouchDB, there is no need to install any additional software, mobile developers can also learn the construction of the service side, both!

github https://github.com/ACRA/acra

The service side of the github https://github.com/ACRA/acralyzer

Author: acra team

use:

There is no easier way to get local than clone source code


##75.DiskLruCache
In a word: A framework that provides disk file cache management capabilities

Reason for listing: 3.7k star is not enough to show that DiskLruCache is excellent, just to manage disk file capacity alone to become a framework, the author needs a lot of courage, fortunately, the author did, and also become Google's official website advocated cache; DiskLruCache can handle it in one sentence!

github https://github.com/JakeWharton/DiskLruCache

By Jake Wharton

use:

compile 'com.jakewharton:disklrucache:2.0.2'
Or download the latest .jar


##76.dexposed
In a word: a support ali most of the App client hot repair, online debugging capacity of the framework

Reason for listing: The re-emergence of the hot repair framework on the list proves that App Hot Repair technology is hot, dexposed provides graphical performance monitoring, online hot fix bug vulnerabilities, supportS AOP Programming IdeaS, And So On, WhetheR You Are The Designer Of Enterprise Thermal Repair Technology Or IntendS To Explore The Field Of Thermal Repair, This Framework Is Very Suitable For You. 3.5k star to prove how much it exists as a technical framework!

github https://github.com/alibaba/dexposed

Author: alibaba

use:

dependencies {
        compile 'com.taobao.android:dexposed:0.1.1@aar' }


##77.Litho
In a word: A framework that provides the ability to build UI efficiently

Reason for listing: As a framework dedicated to building UI, Litho is efficient in opening up threads for rendering and layout separately, then passing the created components to the UI thread for final rendering, using fewer view levels to speed up the scrolling of the interface, and it's worth noting that it only allows developers to make immutable UI components, 3.5K star, proving its value in building UI, more wonderful things to look forward to yourself!

github https://github.com/facebook/litho

Author: Facebook

Use:

[! (Copy code) (//common.cnblogs.com/images/copycode.gif)] (javascript:void(0); "Copy Code")
ependencies { // ... // Litho
  compile 'com.facebook.litho:litho-core:0.3.1' compile 'com.facebook.litho:litho-widget:0.3.1' provided 'com.facebook.litho:litho-annotations:0.3.1' annotationProcessor 'com.facebook.litho:litho-processor:0.3.1'

  // SoLoader
  compile 'com.facebook.soloader:soloader:0.2.0'

  // Optional // For debugging
  debugCompile 'com.facebook.litho:litho-stetho:0.3.1'

  // For integration with Fresco
  compile 'com.facebook.litho:litho-fresco:0.3.1'

  // For testing
  testCompile 'com.facebook.litho:litho-testing:0.3.1' }
[! (Copy code) (//common.cnblogs.com/images/copycode.gif)] (javascript:void(0); "Copy Code")


##78.mosby
In a word: A framework that provides the ability to build MVP projects

Reason for listing: The top part of the list has introduced MVC, MVVM, MVP framework project, presumably at this time you are building enterprise project architecture, choose or develop a suitable MVP framework is imminent, mosby can be your first reference, you can encapsulate it, you can copy it, in any case, 3.4K star, prove how much it is popular with developers in framework design

github https://github.com/sockeqwe/mosby

Author: Hannes Dorfmann

use:

[! (Copy code) (//common.cnblogs.com/images/copycode.gif)] (javascript:void(0); "Copy Code")
dependencies {

  compile 'com.hannesdorfmann.mosby3:mvi:3.0.4' // Model-View-Intent // or
  compile 'com.hannesdorfmann.mosby3:mvp:3.0.4' // Plain MVP // or
  compile 'com.hannesdorfmann.mosby3:viewstate:3.0.4' // MVP + ViewState support
}
allprojects {
  repositories {
    ...

    maven { url "https://oss.sonatype.org/content/repositories/snapshots/" }
}
[! (Copy code) (//common.cnblogs.com/images/copycode.gif)] (javascript:void(0); "Copy Code")

##79.AndResGuard
In a word: A tool that provides confusion about resource file paths

Reason for listing: If you're a sensitive person to APK size, AndResGuard must be for you, and it works like Java Proguard, but only for resources. He'll shorten the already lengthy resource path, such as turning res/drawable/wechat into r/d/a, 3.4K star, proving that you're not alone in the battle to optimize APK!

github https://github.com/shwenzhang/AndResGuard

Author: wechat team

use:

The clone project goes local, which is actually a three- or two-sentence document



##80.StatusBarUtil
In a word: A framework that provides the ability to set an immersive status bar style

Reason for listing: Designer MM always complains that the system status bar is not elegant? Then give her a perfect immersive status bar. StatusBarUtil can set the status bar style as you like, 3.3K star, enough to show how much it is loved by the design MM

github https://github.com/laobie/StatusBarUtil

Author: Jaeger

use:

compile 'com.jaeger.statusbarutil:library:1.4.0'


##81.robolectric
In a word: a unit test framework that doesn't rely on Android devices,

Reason for listing: Sample lists use cases for android four components and common feature testing, 3.2K star, worth trying for curious people

Official address:http://robolectric.org/

github https://github.com/robolectric/robolectric

Author: robolectric

use:

testCompile "org.robolectric:robolectric:3.3.2"

##82.Fragmentation
In a word: A framework that provides the ability to manage Fragmen nested t

Reason for listing: For Activity and Fragment use, you must be handy, but if you want to do a common set of Active city and Fragment nested design, presumably you are a little overwhelmed, Fragmentation can be as your design Fragment management on the first step, 3.2K star, the author thinks it is a bit veritable, the project introduction is about Fragment's management capabilities, However, it does not provide The framentation and activity life cycle, task stack management capacity, so it is difficult to apply directly to enterprise projects, but the source code in the design ideas, worthy of the author and you to learn from, pick people's teeth Hui left yu Xiang!

github：https://github.com/YoKeyword/Fragmentation

Author: YoKey

use:

// appcompat v7包是必须的
compile 'me.yokeyword:fragmentation:0.10.7'
// 如果想使用SwipeBack 滑动边缘退出Fragment/Activity功能，请再添加下面的库 // compile 'me.yokeyword:fragmentation-swipeback:0.10.4'
83.Small
In a word: lightweight plug-in framework

Reason for listing: As a new member of the plug-in framework list, Small's advantage is light, suitable for small team plug-in development program, 3.1K star, let it get cool dog music and other well-known development team favor, if your team wants to gradually implement plug-in development, Small is a good choice!

Official address:http://code.wequick.net/Small/cn/cases

github https://github.com/wequick/Small

Author: wequick team

use:

[! (Copy code) (//common.cnblogs.com/images/copycode.gif)] (javascript:void(0); "Copy Code")
buildscript  {
    dependencies {
        classpath 'net.wequick.tools.build:gradle-small:1.2.0-alpha6' }
}

apply plugin: 'net.wequick.small' small {
    aarVersion = '1.2.0-alpha6' }
[! (Copy code) (//common.cnblogs.com/images/copycode.gif)] (javascript:void(0); "Copy Code")

##84.JsBridge
In a word: A framework that provides WebView and Javascript communication capabilities

Reason for listing: The framework provides the ability to allow H5 page calls to call app methods via JS;

gtihub https://github.com/lzyzsd/JsBridge

Author: hi big head ghost hi

Use:

[! (Copy code) (//common.cnblogs.com/images/copycode.gif)] (javascript:void(0); "Copy Code")
repositories { // ...
    maven { url "https://jitpack.io" }
}

dependencies {
    compile 'com.github.lzyzsd:jsbridge:1.0.4' }
[! (Copy code) (//common.cnblogs.com/images/copycode.gif)] (javascript:void(0); "Copy Code")

##85.richeditor-android
In a word: A powerful rich text editing framework

Reason to be on the list: 2.8k star, the first in the list to provide TextView with a framework for scalability, you don't need it for the time being, but you can't not forget it

github https://github.com/wasabeef/richeditor-android

Author: Daichi Furiya

use:

[! (Copy code) (//common.cnblogs.com/images/copycode.gif)] (javascript:void(0); "Copy Code")
repositories {
    jcenter()
}

dependencies {
    compile 'jp.wasabeef:richeditor-android:1.2.2' }
[! (Copy code) (//common.cnblogs.com/images/copycode.gif)] (javascript:void(0); "Copy Code")

##86.Transitions-Everywhere
In a word: A teaching project that teaches you to use the Transitions API correctly

Reason to be on the list: You may not have tried the Transitions framework of the Android API, you may have heard it, but you can't make the elegant and wonderful motion - don't worry, Transitions-Everywhere, like its name, will take you through the power of Transitions

github https://github.com/andkulikov/Transitions-Everywhere

Author: Andrey Kulikov

use:

dependencies {
    compile "com.andkulikov:transitionseverywhere:1.7.4" }

##87.android-viewbadger
In a word: the ability to quickly add a "medal" to an Android view

Reason for listing: If the word medal sounds strange, then show the number of unread, small red dot mark information this kind of words you must not be unfamiliar, the author believes that in your actual development often encountered for some item to add small red dot marker needs, smart everyone must have a variety of implementation programs, why can not be quickly and elegantly completed? Android-viewbadger can help you implement, of course, in some cases, you need the ability to modify the source code to meet the needs of the design MM! It's worth noting that this wide project hasn't been updated in five years!

github https://github.com/jgilfelt/android-viewbadger

Author: Jeff Gilfelt

use:

Clone source to local

View target = findViewById(R.id.target_view);
BadgeView badge = new BadgeView(this, target);
badge.setText("1");
badge.show();


##88.AndroidWiFiADB
In a word: a plug-in project that does not use a data cable can also let you debug the mobile device APP

Reason for listing: Are you still worried about the lifetime irreparable damage caused to your phone's battery and USB ports by high-intensity unplugged data cables during testing? Don't worry, there is wifi has Android WiFiADB, no data cable can also debug the application, more interesting is, in the test engineer while holding the phone while looking for you to talk about bugs, you have secretly fixed bugs on its phone, hidden in the name!

github https://github.com/pedrovgs/AndroidWiFiADB

Author: Pedro Vicente Gómez Sánchez

use:

Preferences/Settings->Plugins->Browse Repositories->serch AndroidWiFiADB

##89.emojicon
In a word: A framework that provides the ability to display emoji packs at TextView and EdiText

Reason for listing: 2.7k star, the second frame on the list to enhance the display capabilities of TextView, this is designed for emoji bags, if you have ever wondered how WeChat, QQ expression display is done? This frame is sure to satisfy your thirst for knowledge.

##90.packer-ng-plugin
In a word: a blast tool plug-in

On the list utilization: the author tries to maintain the comprehensiveness of the list involved, so the introduction of this plug-in project - the project claims to complete 100 channel packages only need 10 seconds, in the market a variety of multi-channel packaging programs today, choose a suitable for their own team, is the top choice

github https://github.com/mcxiaoke/packer-ng-plugin

Author: Xiaoke Zhang

use:

[! (Copy code) (//common.cnblogs.com/images/copycode.gif)] (javascript:void(0); "Copy Code")
buildscript {
    ......
    dependencies{ // add packer-ng
        classpath 'com.mcxiaoke.gradle:packer-ng:1.0.9' }
} 
[! (Copy code) (//common.cnblogs.com/images/copycode.gif)] (javascript:void(0); "Copy Code")
[! (Copy code) (//common.cnblogs.com/images/copycode.gif)] (javascript:void(0); "Copy Code")
apply plugin: 'packer' dependencies {
    compile 'com.mcxiaoke.gradle:packer-helper:1.0.9' }

 android { //...
 signingConfigs {
      release { // 满足下面两个条件时需要此配置 // 1\. Gradle版本 >= 2.14.1 // 2\. Android Gradle Plugin 版本 >= 2.2.0 // 作用是只使用旧版签名，禁用V2版签名模式
        v2SigningEnabled false }
    }
  }
[! (Copy code) (//common.cnblogs.com/images/copycode.gif)] (javascript:void(0); "Copy Code")

##91.android-priority-jobqueue
In a word: A framework that provides background task management capabilities

Reason to be on the list: If you're a developer interested in drilling down into multithreaded operations, don't miss out on this project, whether it's Active reloading, task priority and concurrency issues when Service uses thread pools, Job Manage takes care of priority, persistence, load balancing, latency, network control, grouping, 2.4K star, excellent multithreaded management capabilities, and it relies on few third-party frameworks that are worth a try

github https://github.com/yigit/android-priority-jobqueue

Author: Yigit Boyar



##92.Android-Debug-Database
In a word: A framework that provides the ability to test the app's internal database capabilities

Reason for listing: the second section of the list for debugging database framework, a line of code integration, directly in the browser to add and delete the app database, 2.3k star, heart is not as good as action!

github https://github.com/amitshekhariitbhu/Android-Debug-Database

Author: AMIT SHEKHAR

Use:

debugCompile 'com.amitshekhar.android:debug-db:1.0.0'
The browser types

 http://XXX.XXX.X.XXX:8080


##93.conceal
In a word: A facebook-provided framework for encrypting large local files

Reason for listing: If you're still worried about the privacy of images in the app, this facebook file encryption framework is enough to solve your problem, and facebook clients' images and data are encrypted using conceal

Official address:http://facebook.github.io/conceal/

github https://github.com/facebook/conceal

Author; facebook

use:

The clone project downloads jar to the local/official website


##94.ARouter
In a word: a framework for providing services and page jump routing

Reason for listing: As the author claims, the framework offers the ability to map from an external URL to an internal page, jump (page decoupling), block the jump process across modules, and more to discover, and 2.1K star, worthy of cheering for an enterprise-class framework

github https://github.com/alibaba/ARouter

Author: alibaba

use:

[! (Copy code) (//common.cnblogs.com/images/copycode.gif)] (javascript:void(0); "Copy Code")
ndroid {
    defaultConfig {
    ...
    javaCompileOptions {
        annotationProcessorOptions {
        arguments = [ moduleName : project.getName() ]
        }
    }
    }
}

dependencies { // 替换成最新版本, 需要注意的是api // 要与compiler匹配使用，均使用最新版可以保证兼容
    compile 'com.alibaba:arouter-api:x.x.x' annotationProcessor 'com.alibaba:arouter-compiler:x.x.x' ...
} // 旧版本gradle插件(< 2.2)，可以使用apt插件，配置方法见文末'其他#4' // Kotlin配置参考文末'其他#5'
[! (Copy code) (//common.cnblogs.com/images/copycode.gif)] (javascript:void(0); "Copy Code")


##95.MagicaSakura
In a word: A framework that provides multi-topic switching capabilities

Reason for listing: The ability provided by the framework has always been valued in this list, this multi-themed framework provided by bilibi, as the list covers the scope can be supplemented, 1.9 star, thanks to the contribution of the bibili team!

github https://github.com/Bilibili/MagicaSakura

Author: Bilibili

use:

compile 'com.bilibili:magicasakura:0.1.6@aar'


##96.CustomActivityOnCrash
In a word: A framework that automatically loads into an Action city when app crashes (instead of displaying Unfortunately, X has stopped)

Reason for listing: Novel ideas are needed for the list, so it won 1.8K stars; as developers should have the ability to take into account all kinds of latent bugs, but we can't always have everything, and colleagues on other system ends can also cause unexpected crash of the program, so how to make the program elegant cransh-> reboot is worth thinking about, this framework provides this ability

github https://github.com/Ereza/CustomActivityOnCrash

Author: Eduard Ereza Martínez

use:

dependencies {
    compile 'cat.ereza:customactivityoncrash:2.1.0' }
添加到 Application class:
[! (Copy code) (//common.cnblogs.com/images/copycode.gif)] (javascript:void(0); "Copy Code")
 @Override public void onCreate() {
    super.onCreate();

    CaocConfig.Builder.create()
        .backgroundMode(CaocConfig.BACKGROUND_MODE_SILENT)
        .enabled(false) //default: true
        .showErrorDetails(false) //default: true
        .showRestartButton(false) //default: true
        .trackActivities(true) //default: false
        .minTimeBetweenCrashesMs(2000) //default: 3000
        .errorDrawable(R.drawable.ic_custom_drawable) //default: bug image
        .restartActivity(YourCustomActivity.class) //default: null (your app's launch activity)
        .errorActivity(YourCustomErrorActivity.class) //default: null (default error activity)
        .eventListener(new YourCustomEventListener()) //default: null
 .apply();
}
[! (Copy code) (//common.cnblogs.com/images/copycode.gif)] (javascript:void(0); "Copy Code")


##97.XhsEmoticonsKeyboard
In a word: the happiest open source emoticon solution

Reason to be on the list: If you're still worrying about how to make your keyboard for your APP, this frame is perfect for you, and it also offers emoji display capabilities, and 1.7 stars prove it's unique. In addition, the author also attached a high imitation WeChat keyboard, QQ keyboard demo, to share with you

github https://github.com/w446108264/XhsEmoticonsKeyboard

Author: zhongdaxia

use:

[! (Copy code) (//common.cnblogs.com/images/copycode.gif)] (javascript:void(0); "Copy Code")
allprojects {
    repositories {
        jcenter()
        maven { url "https://jitpack.io" }
    }
}

dependencies {
    compile 'com.github.w446108264:XhsEmoticonsKeyboard:2.0.4' }
[! (Copy code) (//common.cnblogs.com/images/copycode.gif)] (javascript:void(0); "Copy Code")


##98.Android Debug Database
In a word: the most concise database debugging framework

Span style""font-size: 15px" > reasons to be on the list: debugging the database, is an essential part of your daily work, with the list has appeared facebook stetho, Android Debug Database's greatest advantage is simplicity: integration is simple, observation, operation database concise, there is a reason to recommend it! Stetho is very poor at reading when the number of data sheet fields exceeds 50, and today's recommended one has no doubt a huge advantage in the UI interface!

span style="font-size: 15px">github [https://github.com/amitshekhariitbhu/Android-Debug-Database(https://github.com/amitshekhariitbhu/Android-Debug-Database)

Author: AMIT SHEKHAR

use:



build.gradle：

debugImplementation 'com.amitshekhar.android:debug-db:1.0.3'

//配置端口

 debug {
            debuggable true
            resValue("string", "PORT_NUMBER", "9081")
    }


adb forward tcp:9081 tcp:9081


查看Logcat的ip日志：D/DebugDB: Open http://XXX.XXX.X.XXX:8080 in your browser

boomb！

[! (Copy code) (//common.cnblogs.com/images/copycode.gif)] (javascript:void(0); "Copy Code")
Three. The complete project

##1.iosche
In a word: Google's 2016 Developers Conference presentation project

Reason for listing: github has 13.4k star, ranked first in the enterprise project leaderboard, cattle forced developers, authoritative design model, standard project writing, worth a try;

github https://github.com/google/iosched

Author: Google


##2.Plaid
In a word: Open source apps that provide design news and inspiration

Reason to be on the list: Standard mateial design design, news app, 9k star volume on github is worth your time to get rid of the jagged news app on the market, quickly study it!

github https://github.com/nickbutcher/plaid

Author: Nick Butcher

##3.PocketHub
In a word: Github's Android version

Reason for listing: 8.7K star number, Github's biological son, open source code is worth exploring

github https://github.com/pockethub/PocketHub

Author: Fadil Sutomo

use:

All source code under down

##4.Signal Android
In a word: Signal is a secure messaging app,

Reason to be on the list: 7.9K of star number, tool-like app tag properties, make it unique in the leaderboard, if you are interested in SMS apps, you can dig deeper

github https://github.com/WhisperSystems/Signal-Android

Author: WhisperSystems

Use: the down source code on github

##5.android-UniversalMusicPlayer
In a word: A multimedia app that runs across devices

Reason for listing: Googlesamples Conscience recommends that github has 7.9k star, which can be used on Android phones, cars, tablets, and wearable devices, and will it be new for programmers who have only experienced Android phone development? You're worth a try!

github https://github.com/googlesamples/android-UniversalMusicPlayer

Author: Google

Use: the down source code on github

##6.HomeMirror
In a word: If you're a beautiful guy then you must need this mirror!

Reason for listing: Tool apps can hardly have a place on githubs unless they offer particularly novel features, such as HomeMirror, which has 7,599 stars on github simply because it provides mirror functionality. From now on, Android phones, pads, will become your travel home artifacts, worth having!

github https://github.com/HannahMitt/HomeMirror

Author: Hannah Mittens

HomeMirror First Experience:



##7.ExoPlayer
In a word: A media player that replaces Android's native MediaPlayer

Reason for listing: Perhaps Google is not very satisfied with its own MediaPlayer API, so the birth of ExoPlayer, ExoPlayer provides a powerful extension API, using it to make multimedia players faster, easier to expand, multimedia players interested colleagues can use it to make a big splash! 6.9K star, proving how much it's loved by developers, and what's even more valuable is that google is still updating and maintaining!

Official address:https://google.github.io/ExoPlayer/

github https://github.com/google/ExoPlayer

Author: google

use:

[! (Copy code) (//common.cnblogs.com/images/copycode.gif)] (javascript:void(0); "Copy Code")
repositories {
    jcenter()
}
compile 'com.google.android.exoplayer:exoplayer:r2.X.X' compile 'com.google.android.exoplayer:exoplayer-core:r2.X.X' compile 'com.google.android.exoplayer:exoplayer-dash:r2.X.X' compile 'com.google.android.exoplayer:exoplayer-ui:r2.X.X'
[! (Copy code) (//common.cnblogs.com/images/copycode.gif)] (javascript:void(0); "Copy Code")



##8.cheesesquare
In a word: Android material design exhibition project

Reason for listing: The author is known as the man behind Android Support Lib, and how can he write a show project that can't be recommended? Material design has been hyped for years, but as the most authoritative show project, you'll need it, and 6.7 stars prove how popular it is.

github https://github.com/chrisbanes/cheesesquare

Author: Chris Banes

9.DanmakuFlameMaster
In a word: android end open source bullet engine

Reason for listing: bilibili products, to ensure its thoroughbred quality, and ndk source code is also open source, can be said to be the conscience of the industry, the bomb engine open source to save a lot of video live small partners development costs, the author strongly recommended!

github https://github.com/Bilibili/DanmakuFlameMaster

Author: bilibili

Use:

[! (Copy code) (//common.cnblogs.com/images/copycode.gif)] (javascript:void(0); "Copy Code")
repositories {
    jcenter()
}

dependencies {
    compile 'com.github.ctiao:DanmakuFlameMaster:0.8.3' compile 'com.github.ctiao:ndkbitmap-armv7a:0.8.3' # Other ABIs: optional
    compile 'com.github.ctiao:ndkbitmap-armv5:0.8.3' compile 'com.github.ctiao:ndkbitmap-x86:0.8.3' }
[! (Copy code) (//common.cnblogs.com/images/copycode.gif)] (javascript:void(0); "Copy Code")


##10.facebook-android-sdk
In a word: A framework that provides access to the facebook platform

Reason to be on the list: Whether you have access to Facebook or the need to learn homemade sdk, this is a great way to develop an enterprise-class sdk, is a must-have for advanced and excellent development engineers, 4.1k star, facebook lasting update quality assurance, you deserve it!

github https://github.com/facebook/facebook-android-sdk

Author: Facebook

Use:

 https://developers.facebook.com/docs/android


##11.android-oss
In a word: Kickstarter open source Android client for foreign creative communities

Reason to be on the list: Exquisite enterprise APP, every page is handled very well, if you aspire to become an elegant engineer, this open source project must be right for you, 3.8k star proves its vitality

github：https://github.com/kickstarter/android-oss

Author: Kickstarter

Use;

Clone source to local


##12.k-9
In a word: Android client mail app

Reason for listing: Remember Zhang Xiaolong's masterpiece, FoxMail? If you want to make a mobile email app, k-9 has great reference value, and you'll have a deeper understanding of the application layer protocol

Official address: https://k9mail.github.io/

github https://github.com/k9mail/k-9

use:

Clone project to local

##13.Timber
In a word: a music player-like app

Reason for listing: 3K star, in full accordance with the material design specifications, to provide more than a dozen playback features, but also to provide the app's universal setup capabilities, which is equally excellent, for students who aspire to improve the development of technology is worth a try

github https://github.com/naman14/Timber

Author: Naman Dwivedi

use:

Clone source code is a good habit

##14.remusic
In a word: Imitation NetEase Cloud Music Android version of the app

Reason for listing: After learning Timer, isn't it enough to satisfy your appetite? Remusic can satisfy your appetite - it can even be taken directly as an online project! 2.9K star, based on Timber's design (starting with understanding Timber) is worth starting with; the question is: What would you do if you reconstructed it?

github https://github.com/aa112901/remusic

Author: MW

use:

Clone project

##15.Douya
In a word: open source pod client

Reason for listing: a comprehensive function, architecture design is excellent open source APP; just the bean petal APP design ideas and the reconstruction project, can be seen the author's obsession with products and love, 2.9K star, to prove that the project is not a hot-headed work, if every idea can be achieved, then our world will be wonderful!

github https://github.com/DreaminginCodeZH/Douya

Author: Zhang Hai

use:

Clone project to local

##16.BookReader
In a word: Open source novel reader

Reason for listing: 2.7K star, the first reader app in the list, has a high learning value (for students interested in the direction of reading tools)

github https://github.com/JustWayward/BookReader

Author: Just Wayward Team

use:

clone to local

##17.bilibili-android-client
In a word: high imitation bili's Android client

Reasons to be on the list: 2.5K star, the first video live open source app in the list; suitable for students interested in live video, community interaction; bilibili-android-client uses a lot of large-scale framework, this project is not suitable for students with weak foundation, do not lose heart, learning page layout design is also worth it!

github https://github.com/HotBitmapGG/bilibili-android-client

Author: Hcc

Use: clone to local

##18.AndroidChromium
In a word: Android chrome browser

Reason for listing: As the author claims:

Google Chrome Android Source Project
World-class Android architecture
Clear the business logic of this project can be fully competent for the domestic first-line company engineers
For about you who are interested in combing through the browser framework, it's worth having

github https://github.com/JackyAndroid/AndroidChromium

Author: Jack Y Android

use:

Clone source to local

Four. Development framework:
(Ranked in no order, by type only)

##1.libgdx(https://github.com/libgdx/libgdx)
In a word: a cross-platform android game development framework

Reason for listing: android development framework class first place, 11.7K star volume, game framework is its exclusive label, and more importantly, it is cross-platform

The official address http://libgdx.badlogicgames.com/

github https://github.com/libgdx/libgdx

##2.xUtils
In a word: the old enterprise-level development framework

Reason for listing: 4.9K star, xUtils as a much-admired development framework for programmers in ancient times, the biggest reason - worry- xUtls consists of four modules, which provide four operational capabilities: data manipulation, UI operation, Http protocol operation, picture operation. xUtils as the author's new Android framework design tutor project, in the author's many years of experience, see xUtils as a number of small and medium-sized banks Android end framework program preferred, enough to prove its popularity. The framework has now been updated to xUtils3, if you have some ideas about android frameworks involved, you can start with xUtils and move up to the ranks of frame masters. Although many of the engines in the framework are out of date and the practice of each module can be replaced by other frameworks, xUtils are proud of their domestic developers and the frame darlings of ancient times, worthy of your ownership!

github https://github.com/wyouflf/xUtils

Author: wyouflf

use:

compile 'org.xutils:xutils:3.5.0'


##3.android-common
In a word: An android rapid development framework

Reason for listing: Drop senior Android engineers produced, after many years of developer testing, with 4.3K standing in the fast development framework list third place, the framework provides picture cache, Http cache, DropDownListView, download modules, development of common tools, as the earliest ancient programmers summary development framework, it is the crystallization of a generation of wisdom, worthy of our applause for the author Trinea

github https://github.com/Trinea/android-common

Author: Trinea

use:

Clone code to local


##4.Vitamio
In a word: A cross-platform Android multimedia development framework

Reason for listing: If the exoplayer mentioned earlier doesn't meet your need to develop multimedia, I guarantee that viamio is worth a try

Official address:https://www.vitamio.org/

github https://github.com/yixia/VitamioBundle

Author: the yixia team

use:

Clone source to local



##5.Weex
In a word: Mobile cross-platform development solutions

Reason for listing: 14.4K star, enterprise-class hybrid development framework with mature application cases, Alibaba products, why not try it?

Official address:https://weex.apache.org/cn/

github https://github.com/alibaba/weex

Author: alibaba


##6.cordova-android (Hybrid Development Framework, WebApp Development Framework)
In a word: cross-platform development framework

Reason for listing: Cordova has the ability to do hybrid development, WebApp development requirements: whether you are a Web developer or a Native developer, cordova can make cross-platform apps

Official address:http://cordova.axuer.com/docs/zh-cn/latest/guide/overview/index.html

github https://github.com/apache/cordova-android


##7.react-native
In a word: A framework for operating multiple system languages (Ios, Android) in Javascript language

Reasons to be on the list: It's hard to say what category react-native belongs to, it's suitable for front-end engineers to develop mobile apps, and for Natify developers to develop across platforms, but for Navive developers, a steep learning curve scares away a lot of "framework enthusiasts"; It seems to take us one step closer to the future

Official address: http://facebook.github.io/react-native/docs/getting-started.html

github https://github.com/facebook/react-native

Author: Facebook

#Five. other:
##1.AndroidUtilCode
In a word: A large number of tool classes are available

Reason to list: 10.8K star number, enough to prove how popular it is, welcome to provide you with commonly used tool classes to grow it!

github https://github.com/Blankj/AndroidUtilCode/blob/master/README-CN.md

File → Settings... → Plugins → Browse repositories...

and search for .freeline

##2.kotiln
In a word: Google's Android programming language

Reason for listing: Just as Android Studio replaced Eclipse, Google's use of kotiln as The Official Programming Language for Android may have been to avoid patent litigation with Oracle, but kotlin's 100% java-compatible, dramatically streamlined java code volume, and the idea of functional programming are all worth noting, remember what we said before the list? The future is kotlin, the present is java, but we are on the road to the future - learning the programming language of the future, improving their productivity, leaving work early to play beans, why not?

Official address:http://kotlinlang.org/

github：https://github.com/JetBrains/kotlin

use:

http://kotlinlang.org/docs/reference/ provides resources such as api-android use cases-books

#Six. Book items
(Sort no order)
##1. Android developer China website training course
In a word: In line with China's national conditions, Google developer website sub-products - Android developer official website

Reasons to be on the list: Here are training courses, API use case courses, Sample use cases, dependency library introductions, AndroidStudio official website... Wait for a series of public free courses, although most of the content is still in English, but you are willing to rely on the English dictionary one by one gnawing, believe me, your Android knowledge level will kill most of the Android books on the domestic market in seconds

Official address:https://developer.android.google.cn/training/index.html

Author: google

##2.android-architecture
In a word: Google offers the basic framework of Android to the moment

Reason for listing: After reading it, mvp, mvvm will be cut into cut melons, autumn wind sweeps leaves in general...

github https://github.com/googlesamples/android-architecture

Author: google

##3.andorid-open-project
In a word: Navigation class directories that cover almost all of Android's open source projects

Reasons to be on the list: 23k star navigation category directory, and its reputation is not consistent with the project's navigation, browsing reading experience is very poor, recommend Chinese ed for leisure reading;

github https://github.com/Trinea/android-open-project

Author: Trinea
