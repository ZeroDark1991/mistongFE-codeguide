# 项目结构

	|-dist                开发环境文件生成目标目录

	|-src                 源文件存放地址

	    |-dev             前端开发使用的临时文件

	    |-js              js脚本文件

	    |-less            less或者css文件

	    |-resource        其他资源存放地址

	        |-iconfont    图标文件

	        |-img         图片文件

	        |-libs        前端库存放地址（jquery、zepto ...）

	        |-plugins     前端插件存放地址 （MathJax、layerjs...）

	        |-swf         flash所需要的文件

	|-tools               项目工具脚本存放目录

各目录可以设置下级目录存放

html引用静态文件设置相应绝对路径引用  
比如: http://staticdev.kaike.la/js/jQuery.js