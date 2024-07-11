# REDROCK 移动开发部 Android 2024年暑假考核

## 📝写在前面

紧张的写课件阶段终于结束了，下面就是大家的开发考核环节。👏👏👏

不知不觉中一年的时间已经过去了，你已经在网校学习了一年了。相信大家在这一年中学习到了很多，从最开始的“Hello World”，到现在能够在指尖上跳跃的app，从软件的使用者到软件的开发者。

在这一年中你上的每一节课，做过的每一次作业，掉过的每一根头发，熬过的每一次夜，都是你成长的见证。这些经历不仅让你掌握了宝贵的编程技能，更培养了你解决问题的能力和坚持不懈的精神。

最后，这些努力将在即将到来的开发考核中得到检验。这不仅是对你学习成果的一次展示，更是将你的想法付诸实践的机会。相信通过这次考核，你会发现自己比想象中更强大，能够创造出令人惊叹的作品。

记住，编程不仅是一项技能，更是一种思维方式。希望你能够将这种创新和逻辑思维运用到生活的各个方面，继续探索、学习、成长。无论未来你是否选择以编程为职业，这一年的经历都将成为你人生旅程中宝贵的财富。

祝愿大家在考核中展现出最好的自己，创造出令人印象深刻的作品。加油！👨‍💻👩‍💻🚀



振奋人心的话说完了，下面我们来看一下考核要求

## 考核要求

- 考核采用多人开发，两个人一组选择一个选题。要求使用多模块开发，否则合并冲突会让你崩溃。（多模块开发参考群里面的课件，以及往年学长的demo，不过不是kts写法，[项目地址](https://github.com/RQ527/GitDemo)，推荐仔细阅读）
- 请合理分配团队工作
- 一个选题最多只能有两个组选择
- **每天至少需要一个commit**
- 个人表现和在团队里的贡献会作为最终评测标准。

## App要求

- API 兼容到 Android6.0（API 24）
- 只能使用 `Kotlin`
- 代码中**重要函数和变量**需要有注释，不要求全部都写
- 完整的 README，必须包含：
  - 每人都需要写一份README
  - APP简要介绍，使用步骤
  - 在团队里所做的工作介绍（所负责的模块、功能、使用步骤等）附 Gif 图片）
  - 使用到的比较重要的技术及知识点
  - 不足之处
  - 心得体会
- 考核期间如果遇到**运行时 bug**，原则上**不能向学长求助**，如果是无法编译问题，百度后仍无法解决则可以在大群里面提问
- 请使用自己擅长的技术，**不熟练就谨慎使用**
- 考核截止日期为2024年7月27日晚上18：00，在该时间点之前需要打一个apk上传至GitHub仓库，之后只允许修bug，不允许添加新功能
- 因为有 12 天开发 + 3 天改 bug，所以要求谈心时的最终版本无明显闪退 bug（**记得做好断网时的网络请求出错处理**）



### 依赖要求

- 禁止

  使用除以下库外的其他库，可使用的库如下：

  - 所有 `google` 库
  - 所有 `android` 以及 `androidx` 库
  - 所有 `jetbrains` 库（协程包含在这里面）
  - 部分第三方库
    - [`ARouter`](https://github.com/alibaba/ARouter)
    - [`Glide`](https://github.com/bumptech/glide)
    - [`Lottie`](https://lottiefiles.com/blog/working-with-lottie/getting-started-with-lottie-animations-in-android-app)
    - [`Retrofit`](https://github.com/square/retrofit)
    - [`Okhttp`](https://github.com/square/okhttp)
    - [`Gson`](https://github.com/google/gson)
    - [`Rxjava`](https://github.com/ReactiveX/RxJava)
    - [`RxPermissions`](https://github.com/tbruyelle/RxPermissions)：一个权限申请库
    - [`PhotoView`](https://github.com/Baseflow/PhotoView)：一个专门查看图片的库
    - 如果你做的项目需要使用到视频播放的功能，允许使用播放视频的第三方库（因为官方库有坑，很难用）
    - 如果对依赖有特殊要求，请在大群里提问
    - 如果使用自己的依赖库，有如下要求
      - 不能是 fork 来的
      - 绝大部分代码是自己所写

- 由于本次考核需要衡量你们接手掌邮的能力，所以**强烈不推荐**使用 `compose`。

- `Banner`（轮播图）请自己实现



### 设计要求

- MVVM 架构，允许在简单网络请求时不设计仓库层
- 需包含网络请求
- 好看的 UI

个人推荐大家熟悉一下的技术：

ViewBinding

Retrofit（切换线程推荐结合Rxjava）

Rxjava（不强制要求）

协程+flow（不强制要求）

常用的JetPack（LiveData、ViewModel、Navigation等）

RecyclerView的使用

本地储存推荐SP或者Room（数据库的话第一次使用可能会踩坑）



### 特殊要求

- 需要公开你的仓库，**从考核第一天开始**
- 如果不想公开，可以在私有仓库的情况下把我们设置成贡献者
  - 点击 Settings - Collaborators - Add people
  - 输入以下学长的 github 名字
    - 李：lytMoon
    - 胡：Black-Skyline
- 别忘了前面要求的**每天至少一个commit**



## 考核选题

### 开眼（不考虑登录情况）

接口很凌乱，但能写出来一个完整的 `app`，以下给出一些其他项目，里面包含了部分接口

https://www.wanandroid.com/blog/show/2718

https://github.com/fmtjava/Jetpack_Kotlin_Eyepetizer

详细的接口分析文档：https://github.com/1136535305/Eyepetizer/wiki/开眼-API-接口分析

![img](https://raw.githubusercontent.com/985892345/Redrock2022-AndroidSummerWork/main/img/%E5%BC%80%E7%9C%BC%E9%83%A8%E5%88%86%E6%8E%A5%E5%8F%A3.png)



### 网易云音乐

接口文档：[网易云音乐 API](https://binaryify.github.io/NeteaseCloudMusicApi/#/)

音乐播放器和MV播放可使用三方库。

注意：

文档中的的接口是没有指定根地址的，而我们这次的根地址是：

> https://1258656679-dk116gec67-gz.scf.tencentcs.com

举个例子，![QQ_1720686459666](https://github.com/lytMoon/Redrock2024-AndroidSummerAssessment/assets/117186626/5366b0c1-ae96-4a0c-879d-d8c22fcd0004)


根据调用例子，所以我们完整的请求地址是：跟地址加相对地址

> https://1258656679-dk116gec67-gz.scf.tencentcs.com/song/url/v1?id=33894312&level=exhigh

可以通过postman调试



### GitHub

github 的大部分操作都是公开了 api 的，可以在下面找到：

https://docs.github.com/cn/rest

如果感觉看不懂，可以百度一下，有很多总结了的文章。

下面我推荐一些文章，都是可以百度到的

[**github api接口**](“https://www.jianshu.com/p/a6779929fad2)

[**一篇文章搞定Github API 调用 (v3）**](https://segmentfault.com/a/1190000015144126)

[**官方接口列表**](https://docs.github.com/en/rest/issues/comments?apiVersion=2022-11-28#update-an-issue-comment)



## 其他问题

**考核完后可以回家吗？**

具体询问自己辅导员，通过了这边就可以放人。

**学校让暑假做社会实践怎么办？**

社会实践在暑假留校后就可以在网校开证明，考核没有通过的也能开。



**重要的事情说三遍：**

### 不要熬夜！

## 不要熬夜！

# 不要熬夜！

### 严禁通宵！

## 严禁通宵！

# 严禁通宵！

