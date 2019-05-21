# framework
common-lib

本AAR文件为Android项目基础库

使用方式

在项目根build.gradle中加入
allprojects {
  maven { url "https://raw.githubusercontent.com/mvn-repo-aar/framework/master" }
}

在目标工程中使用
implementation('com.wwxframe:aar:+@aar'){transitive=true}

解决不能调用aar中三方依赖问题(dependencies)
{transitive=true}
