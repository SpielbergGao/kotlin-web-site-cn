---
type: tutorial
layout: tutorial
title:  "《以 Eclipse IDE 入门》"
description: "本教程将指导我们使用 Eclipse ID E创建一个简单的 Hello World 程序"
authors: Nikolay Krasko
date: 2019-04-24
showAuthorInfo: false
---

## 配置环境

首先，您需要在系统上安装 Eclipse IDE。 您可以从[下载页面](https://www.eclipse.org/downloads/)下载到最新版本。 建议使用 “Eclipse IDE for Java Developers” 软件包。

在您的 Eclipse IDE 中下载该 _Kotlin Plugin for Eclipse_ 插件来添加对 Kotlin 的支持。我们建议从 [Eclipse Marketplace](http://marketplace.eclipse.org/content/kotlin-plugin-eclipse) 里安装 Kotlin 的插件。

另一种选择是将此按钮拖动到正在运行的 Eclipse 窗口中：

<a href="http://marketplace.eclipse.org/marketplace-client-intro?mpc_install=2257536" class="drag" title="Drag to your running Eclipse workspace."><img class="img-responsive" src="http://marketplace.eclipse.org/sites/all/themes/solstice/public/images/marketplace/btn-install.png" alt="Drag to your running Eclipse workspace." /></a>

或者，打开 __Help \| Eclipse Marketplace...__ 菜单栏后搜索 __Kotlin Plugin for Eclipse__ ：

   ![Eclipse Marketplace]({{ url_for('tutorial_img', filename='getting-started-eclipse/marketplace.png') }})

一种更老套的方法是直接使用 *update site* ：

```
https://dl.bintray.com/jetbrains/kotlin/eclipse-plugin/last/
```

插件安装完成后重启 Eclipse，请确保插件是正确安装的：打开  __Window \| Open Perspective \| Other...__ 后，里面有 __Kotlin perspective__。

   ![Kotlin Perspective]({{ url_for('tutorial_img', filename='getting-started-eclipse/open-perspective.png') }})

## 创建一个项目

现在您已准备好创建一个新的Kotlin项目。

1. 选择 __File \| New \| Kotlin Project__.

   ![New Kotlin Project]({{ url_for('tutorial_img', filename='getting-started-eclipse/project-name.png') }})

   一个空的 Kotlin/JVM 项目创建好了。
  
   对 Eclipse IDE 来说，这也是一个 Java 项目，但是配置了 Kotlin 的性质，这意味着他可以构建 Kotlin 并且有 Kotlin 运行库的引用。这个解决方案的好处是您可以将 Kotlin 和 Java 添加到同一个项目中。

   项目结构如下所示：

   ![Empty Kotlin Project]({{ url_for('tutorial_img', filename='getting-started-eclipse/empty-project.png') }})

2. 在源目录中创建一个新的 Kotlin 文件。

   ![New File From Context Menu]({{ url_for('tutorial_img', filename='getting-started-eclipse/new-file.png') }})
   
   您可以不填写后缀名 __.kt__。 Eclipse 会自动给它添加。
   
   ![New Kotlin File Wizard]({{ url_for('tutorial_img', filename='getting-started-eclipse/file-name.png') }})

3. 获得源文件后，添加一个 `main` 函数作为 `Kotlin` 程序的主入口。 您只需输入 `main` 并通过点击 `Ctrl + Space` 完成调用代码。

   ![Main Template]({{ url_for('tutorial_img', filename='getting-started-eclipse/main.png') }})

4. 添加一行简单的打印消息代码：

   ![Hello World Example]({{ url_for('tutorial_img', filename='getting-started-eclipse/hello-world.png') }})

## 运行这个程序

要运行该应用程序，请右键单击主文件中的某个位置，然后选择 __Run As \| Kotlin Application__。

   ![Run Kotlin Application]({{ url_for('tutorial_img', filename='getting-started-eclipse/run-as.png') }})
   
如果一切顺利，您将在 **Console** 窗口中看到结果。

   ![Program Output View]({{ url_for('tutorial_img', filename='getting-started-eclipse/output.png') }})

恭喜！ 您现在可以在 Eclipse IDE 中运行 Kotlin 应用程序。

