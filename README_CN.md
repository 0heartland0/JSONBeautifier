## JSON格式化

[English Doc](README.md) | Chinese Doc

由于我使用的 BurpSuite 版本是 1.7.x，为了方便，特地编译了这个插件。


这是一个用于美化 JSON 输出的 BurpSuite 扩展。 BApp Store 目前有一个 [python 版本](https://portswigger.net/bappstore/showbappdetails.aspx?uuid=ceed5b1568ba4b92abecce0dff1e1f2c)。 原作者没有生成jar包。 我选择生成一个jar包。 打包过程中遇到了一些小问题，已成功解决了，生成了一个新的jar包。

#### 使用前
<img src="/img/JSONRaw.PNG"/>

#### 使用后
<img src="/img/JSONBeautified.PNG"/>

### 编译
这里需要注意的是IntelliJ IDEA自带的Gradle版本比较高，会导致编译失败。 Gradle 版本需要修改才能编译成功。

使用 IntelliJ IDEA 自带的 Gradle 编译结果：
![1](https://user-images.githubusercontent.com/89680763/149082215-fc6a0c1f-6c5f-40ae-bfae-8e75b1c5470b.png)

修改Gradle版本后，编译成功：
![2](https://user-images.githubusercontent.com/89680763/149083280-715f2b22-690a-4470-b7f1-92f291e505cd.png)
![3](https://user-images.githubusercontent.com/89680763/149083289-c6df0d54-677c-4dac-9c48-3893babf599d.png)

编译后的jar包已经生成。
如果担心使用中出现问题，可以下载代码自行编译。
参考我使用的版本（IntelliJ IDEA 2021.3.1、JDK 1.8.0_202、Gradle 6.9.2）编译，或者自己解决编译环境问题（主要是Gradle版本）。


原作者代码地址：https://github.com/NetSPI/JSONBeautifier

构建一个 jar 文件:
```sh
gradle fatJar
```    

## 致谢
- 感谢 [NetSPI](https://github.com/NetSPI) 提供的源代码;
- 感谢 [Skay](https://github.com/0linlin0)@[白帽一百安全攻防实验室](https://www.whitecap100.org) 提供的技术支持.
