###iOS上线流程
#### 具体步骤如下网站介绍的很清楚，一步一步来就可以。
 
  [【简书】iOS 上线流程](http://www.jianshu.com/p/06c3c1b0bf9b)
  
#### 一些容易遇到的问题。
 
- 如果发现项目中HTTP请求失败，请检查项目中的Info.plist 中是否允许HTTP协议传输。如果没有，请添加。


	 	<key>NSAppTransportSecurity</key>
		<dict>
			<key>NSAllowsArbitraryLoads</key>
			<true/>
		<dict>
 		
- 如果项目中有__weak 修饰词找不到或者报错的
 
	 xcode -> Build Settings -> Apple LLVM 7.1-Language - Objective C -> Weak Refrernces in Manual Retain Release  设置为YES

- 修改项目名称
 
   xcode -> Build Settings -> Product Name 	

 	
 	
