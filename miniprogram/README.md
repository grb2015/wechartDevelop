# wechartMiniProgram
微信小程序开发笔记

1. 在project.config.json里面设置自己的appid  
		appid如何查看?
		答案：通过"微信公众平台"登陆后---> 开发-->开发设置
2. 如何发布版本
		使用微信开发者平台工具进行开发，在右上角有上传功能，上传后就可以在通过"微信公众平台"登陆，在后台管理上看到
		注意：上传下一个体验版本时，必须在小程序网站后台管理里面，将上一个版本的代码删除掉
		
3. 小程序需要访问后端的话，必须在 通过"微信公众平台"登陆，在后台管理配置https的url请求地址

4. 如何设置https的请求地址？

5. 如何从微信小程序跳转到html网站
	答:使用小程序的web-view,但是这个只能小程序企业版才行  https://developers.weixin.qq.com/miniprogram/dev/component/web-view.html
	
6. 在小程序后台设置体验的时候，必须设置路径  pages/home/home

7. 小程序跳转到h5携带参数,如何调试呢？
   好像没有更好的方法进行调试,只能把传递过去的参数，使用html的<p>标签等,将参数在页面显示出来。而且必须h5改一遍，就部署h5到服务器一遍。


8. 给你一个新的企业小程序, 在微信公众平台里面都需要设置什么?  
	step1 : 将开发->开发设置 里面的appid拷贝到代码的project.config.json  
	step2 : 设置服务器域名  开发->开发设置->服务器域名 https://example.com:8002  
	step3 : 设置业务域名  开发->开发设置->业务域名 https://example.com (注意设置业务域名的时候需要进行校验，即把txt放到IIS网站https://example.com的根目录下)  
	step4 : 上传代码。在微信开发工具里面,导入项目，填写appid 。 然后右上角上传  
	step5 : 在微信公众平台里面，将上传的版本提交审核  
	step6 : 审核通过之后，在微信公众平台里面，点击发布  
9. 小程序本地素材单个不能超过2M。所以素材尽量都放到oss  https://developers.weixin.qq.com/miniprogram/dev/framework/subpackages.html

10. 一些小程序功能必须在微信最新的版本才支持。老的微信版本无法。产品出来后如何在特定的版本(安卓的微信，ios的微信)测试呢？微信开发工具里面可以设置。右上角详情(三条线的标准）-->本地设置-->调试基础库

