imgui
================================
OpenGL3.2バックエンドを持つ軽量でマルチプラットフォームなGUIライブラリ

このライブラリは何？
-------------------------
コードのほとんどはリキャストライブラリから持ってきています : http://code.google.com/p/recastnavigation/

TrueTypeフォントの読み込みとレンダリングは、stb_truetypeを使用して行われます。 : http://nothings.org/stb/stb_truetype.h

OpenGLバックエンドは、主にMac OS Xコアプロファイルとの互換性を保つために、OpenGL immediate modeからOpenGL 3.2へ移植されました。

![Alt text](http://adrien.io/img/imgui/imgui.png)

ビルド方法
-------------------------
依存関係のあるライブラリはOpenGLだけです。GLFW、GLEWはサンプルプログラムに埋め込まれています。

Linux : Arch Linux, Ubuntu 12.10, Debian Wheezy で、さまざまなバージョンのgccコンパイラを使ってテストしています。

    premake4 gmake
    make debug
    make release
    ./sample


Mac OS X : 10.7 (Lion)、XCode 4.6でテストしています。コアプロファイルのコンテキストにのみ対応しています。

    premake4 gmake
    make debug
    make release
    ./sample

Windows : Windows 7、Visual Studio 2008および2010でテスト済み。

    premake4 vs2008 
    Open .sln file


使用法
----------------------------

詳細な使用例については、[sample.cpp](https://github.com/AdrienHerubel/imgui/blob/master/sample.cpp) をご確認ください。 
