# b4x20220401
愚人節-B4X實驗: 如何在b4x使用java寫的程式???JavaObject,inline-java,庫Library API (B4J)分享

B4X實驗: 如何在b4x使用java寫的程式???JavaObject,inline-java,庫Library API (B4J)分享
參考資料:
https://developer.android.com/index.html
https://docs.oracle.com/javase/8/docs/api/
https://openjfx.io/javadoc/11/allclasses.html
https://www.runoob.com/java/java-tutorial.html
https://www.b4x.com/android/forum/threads/dbf-read-write-dbf-file-using-jdbf.136728/#content
https://www.b4x.com/android/forum/threads/inline-java-code.50141/


0.對java要有點那個喔???


1.如何引用java寫的程式
JavaObject,inline-java,庫Library API  
單獨???混用???哈...


Erel
我將分享一個秘密：除了 DJI 無人機 SDK 等非常專業的庫之外，我不再創建基於 Java/Objective C 的庫。
我發現直接在 B4X 中編寫任何我能寫的東西更容易，如果需要，使用 JavaObject 或內聯 Java / OBJC 來訪問本機 API。然後將該庫打包為 b4xlib 庫。
編寫 B4X 代碼要容易得多，結果在很多情況下是跨平台的，開發人員可以根據需要修改庫。
對於諸如 XLUtils 之類的複雜庫也是如此。


2.庫Library API  
slc
SimpleLibraryCompiler 建立一個LIB
https://www.b4x.com/android/forum/threads/tool-simple-library-compiler-build-libraries-without-eclipse.29918/#content
xml jar

3.JavaObject
https://www.b4x.com/guides/B4XJavaObject_NativeObject/?page=1

JavaObject can be used to access Android or Java objects or properties not directly exposed to B4A 
or B4J. 
The library is the same for B4A and B4J. 
NativeObject is similar to JavaObject but for B4i. 
To use JavaObject or NativeObject you should know or learn how the operating systems are 
constructed and how they work. 
The purpose of this booklet is to give an ‘entry point’ with examples, to better understand how to 
use it. 
It is not an encyclopedia of routines. 


//
	
	Private jo As JavaObject = Button2 'wrap the Label object
	
	jo.RunMethod("setText", Array("CENTER"))

	button2.text="CENTER"	

4.inline-java
https://www.b4x.com/android/forum/threads/inline-java-code.50141/#content













