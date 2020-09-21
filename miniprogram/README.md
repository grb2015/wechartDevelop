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
