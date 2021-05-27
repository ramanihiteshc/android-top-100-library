1. Retrofit　　
In a word: Retrofit is a type-safe network framework based on HTTP protocols that serves Android and java languages

Reason for the list: Retrofit topped the list with 21.8k stars and android sub-titles.

The official address http://square.github.io/retrofit/

github https://github.com/square/retrofit

Author: square team

use:

compile 'com.squareup.retrofit2:retrofit:2.3.0'


1. Retrofit　　
In a word: Retrofit is a type-safe network framework based on HTTP protocols that serves Android and java languages

Reason for the list: Retrofit topped the list with 21.8k stars and android sub-titles.

The official address http://square.github.io/retrofit/

github https://github.com/square/retrofit

Author: square team

use:

compile 'com.squareup.retrofit2:retrofit:2.3.0'


2.okhttp

In a word: okhttp is a network framework based on HTTP and HTTP2.0 protocols that serves java and android clients

For reasons of being on the list, okhttp finished second with a 20.4k stars and android subheadings. Large companies such as Taobao also package okhttp. Retrofit 2.0 began to build a built-in okhttp framework, Retrofit focused on packaging interface to complete business requirements, okhttp focused on the security and efficiency of network requests, the author will distinguish between the two, is to let later learners know that this is two sets of frameworks, learning the principles of the framework can be learned separately, so as not to understand confusion.

The official address http://square.github.io/okhttp/

github https://github.com/square/okhttp

Author: square team

use:

compile 'com.squareup.okhttp3:okhttp:3.8.0'

3.Butter Knife

In a word: Butter Butter provides the ability to generate template code using annotations to bind views to methods and parameters.

Reason for listing: 16.5K star on github, along with the Butter Knife plug-in from Android Studio, helps developers save on frequent findviewbyids, and the latest Butter Knife offers onclick bindings and string initialization, and beginners can check out Butter's Ander Knife and Knife Knife plug-ins for further learning!

Official address:http://jakewharton.github.io/butterknife/

github：https://github.com/JakeWharton/butterknife

Author: Jake Wharton is also a member of the Square team

use:

dependencies {
  compile 'com.jakewharton:butterknife:8.6.0' annotationProcessor 'com.jakewharton:butterknife-compiler:8.6.0' }

4.MPAndroidChart

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

5. glide

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


6.leakcanary

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

7.Android-Universal-Image-Loader

In a word: Once the picture loaded frame king, android development veterans have used it

Reasons to be on the list: Android-side picture loading frame big brother, 15.3k star is enough to prove its popularity, the biggest difference between UIL and gilde is customizable, UIL provides a large number of configuration methods, picture loading status callbacks (success, failure, in progress), loading animation, etc.; But the author still recommends you to use!

github https://github.com/nostra13/Android-Universal-Image-Loader

Author nostra13

use:

Download the address universal-image-loader-1.9.5 .jar


8.EventBus

In a word: EventBus is a framework for communication between local components

Reason for listing: Intercombusitive communication framework star volume first: 14.8k, in large projects Activities, fragments, Threads, Services can see its use scenario, although EventBus in the delivery of events to uninstaled components is somewhat limited, only suitable for "living" components to pass messages, but still does not prevent it from being active in the various scenarios of large projects.

The official address http://greenrobot.org/eventbus/documentation/how-to-get-started/

github https://github.com/greenrobot/EventBus

Author greenrobot

use:

compile 'org.greenrobot:eventbus:3.0.0'

9.zxing

In a word: Barcode image processing library

Reason for listing: If you've used QR codes, you've definitely used the famous zxing indirectly. 13.9K of star volume, let it ranked ninth in this list, really, if you have the need to understand the QR code, you may wish to understand, modify its source code to start.

github https://github.com/zxing/zxing

Author Sean Owen


10.picasso

In a word: powerful picture download, cache framework

Reason for listing: The third picture category framework appears in this list, the difference is that picasso more emphasis on image download, you can integrate picasso into your project, you can also combine gilde and UIL and picicasso, all three packaged into your project, on demand.

The official address http://square.github.io/picasso/

github https://github.com/square/picasso

Author square team

use:

compile 'com.squareup.picasso:picasso:2.5.2'
Or download it

Jar package


11.lottie-android

In a word: A framework that quickly shows the animation of Adobe Afeter Effect (AE) tools on the Android side

Reason for the list: Animation frame first place, github on 13.3k star proved his superiority, the use of json files to quickly achieve animation effects is its greatest convenience, and this json file is also provided by AdobeAfter Effects (AE) tool, in AE installed a Bodymovin plug-in, using this plug-in to eventually generate animation effects json file, This johnson file can be parsed by LottieAnimationView and generated brilliant animations. And it supports cross-platform yo.

github https://github.com/airbnb/lottie-android

Author: Airbnb Team


12.fresco

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


13.RxAndroid

In a word: A framework for asynchronous communication between Android client components

Reason for listing: 12.7k star on github, second in the component communication framework, only after EventBus, if you want to ask the difference between the two, Eventbus is used to replace the cumbersome Interface between components, RxAndroid is used to replace Ansy Task, not conflict;

github https://github.com/ReactiveX/RxAndroid

By Jake Wharton

use:

compile 'io.reactivex.rxjava2:rxandroid:2.0.1'
compile 'io.reactivex.rxjava2:rxjava:2.1.0'

14.SlidingMenu

In a word: Side-slip menu bar frame

Reason to be on the list: The Upper Paleo Frame, named after Userval-Image-loader, gives your app the ability to slide the menu bar The github flash has more than 10.5k stars, proving its enduring durability, and even with Google's launch of NavigationDrawer, it hasn't reduced developers' support for Silding Menu, a classic that has not been updated in four years; too many apps have used it, and you can see it on the open source license for the software!

github https://github.com/jfeinstein10/SlidingMenu

By Jeremy Feinstein

use:

Fork source code on gihub, integrated into the project


15.PhotoView

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


16.material-dialogs

In a word: A custom dialog framework

Reason for listing: 9.9k star, the third custom View framework after PhotosoView, SlidingMenu, maybe you're still a new to custom View, and you're a little rusty with Dialog, which you can use to improve your Dellaog usage

github https://github.com/afollestad/material-dialogs

By Aidan Follestad

use:

dependencies { // ... other dependencies here
    compile 'com.afollestad.material-dialogs:core:0.9.4.5'
}


17.Android-async-http

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


18.androidannotations

In a word: A fast development framework based on annotations

Reason for listing: Like Butterknife, annotations are used to quickly complete the initialization of view, except that androids offer more capabilities: simple threading models, etc.;

The official address http://androidannotations.org/

github https://github.com/androidannotations/androidannotations

Author: Wonder Csabo


19.fastjson

In a word: A framework based on json parsing and generation

Reason for listing: From its name is not difficult to see, fast is its biggest feature, Alibaba's origin to ensure the quality and superiority of the code, 9.4k star number, is also the first chinese open source framework in the list, involving the network of apps will use johnson, fastjson is worthy of your first choice!

github https://github.com/alibaba/fastjson

Author: alibaba

use:

compile 'com.alibaba:fastjson:1.1.58.android'


20.Material-Animations

In a word: An animated framework that provides the ability to transition scene transformation

Reason for listing: Android Animation Frames came in second place, with 9.3k stars, and unlike lottie-android, which ranks first on the Animation Frames list, Material-Animations offers animated effects for scene switching. Some of Transition's (transition animation) presentations are already available on Android's official website, and as beginners find it difficult to quickly expand into their projects, Material-Animations' examples save developers the hassle of copying them directly into their own apps.

github https://github.com/lgvalle/Material-Animations

Author: Luis G. Valle

use:

Down source code, modify learning


21.tinker

In a word: It is WeChat's Android hot patch solution

Reason for listing: 9.1k star, WeChat in use of hot patch scheme, heartbeat is not as good as action

The official address http://www.tinkerpatch.com/Docs/intro

github https://github.com/Tencent/tinker

Author: Tencent

