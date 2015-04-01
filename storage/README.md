# 存储（Storage）

本章将介绍在Qt5中使用QtQuick存储数据。QtQuick只提供了有限的方法来直接存储本地数据。在这样的场景下，它更多的扮演了一个浏览者的角色。在大多数项目中，存储数据由C++后端来完成，并需要将这个功能导入到QtQuick前端。QtQucik没有提供类似Qt C++的主机文件系统接口来读取和写入文件。所以后端工程师需要编写一个这样的插件或者使用网络通道与本地服务器通信来提供这些功能。

每个应用程序都需要持续的存储少量或者大量的信息。可以存储在本地文件系统或者远程服务器上。一些信息将会被结构化、简单化例如程序配置信息，一些信息将会巨大并且复杂例如文档文件，一些信息将会巨大并且结构化需要与某种数据库连接。在这章我们将会讨论如何使用QtQuick通过网络和本地的方式存储数据。