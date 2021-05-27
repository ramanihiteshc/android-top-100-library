

## \ 1. Retrofit　　
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
