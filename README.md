## JSONBeautifier

English Doc | [Chinese Doc](README_CN.md)


This is a BurpSuite extension for beautifying JSON output. The BApp Store currently has a [python version](https://portswigger.net/bappstore/showbappdetails.aspx?uuid=ceed5b1568ba4b92abecce0dff1e1f2c) in the BApp Store at the moment.. The original author did not generate a jar package. I choose to generate a jar package. Some minor problems were encountered during the packaging process, which have been successfully resolved and a new jar package was generated.

#### Before
<img src="/img/JSONRaw.PNG"/>

#### After
<img src="/img/JSONBeautified.PNG"/>

### Building
It should be noted here that the version of Gradle that comes with IntelliJ IDEA is relatively high, which will cause compilation failure. The Gradle version needs to be modified to compile successfully.

Compiling results using Gradle that comes with IntelliJ IDEA：
![1](https://user-images.githubusercontent.com/89680763/149082215-fc6a0c1f-6c5f-40ae-bfae-8e75b1c5470b.png)

After modifying the Gradle version, the compilation is successful:
![2](https://user-images.githubusercontent.com/89680763/149083280-715f2b22-690a-4470-b7f1-92f291e505cd.png)
![3](https://user-images.githubusercontent.com/89680763/149083289-c6df0d54-677c-4dac-9c48-3893babf599d.png)

The compiled jar package has been generated.
If you are worried about problems in use, you can download the code and compile it yourself.
Refer to the version I use (IntelliJ IDEA 2021.3.1, JDK 1.8.0_202, Gradle 6.9.2) to compile, or solve the compilation environment problem by yourself (mainly the Gradle version).


Original author code address ：https://github.com/NetSPI/JSONBeautifier

To build a jar file:
```sh
gradle fatJar
```    

## Thanks
- Thanks to [NetSPI](https://github.com/NetSPI) for providing the source code;
- Thanks to Skay(White Hat 100 Security Attack and Defense Lab) for technical support.
