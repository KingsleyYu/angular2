# angular2-lesson-lib

这是本demo[Angular2(Beta)入门](https://github.com/duanshanghanqing/angular2)使用的
库文件，你可以下载到本地练习。

文件清单：

* index.html - 测试文件
* gulpfile.js - 工程文件
* dist/angular2.beta.stack.min.js - 合并的库文件
* src/angular2-pollyfills.js - 浏览器功能增强库
* src/angular2.dev.js - angular2基础框架
* src/http.dev.js - angular2的HTTP访问库
* src/router.dev.js - angular2的路由库
* src/Rx.js - 反应式计算的JavaScript实现库
* src/typescript.js - TypeScript编译转码库
* src/system.config.js - systemjs配置文件
* src/tsloader.js - 自动编译页面中的typescript脚本

## 使用方法

直接在Html文件中引用angular2.beta.stack.min.js，并将TypeScript代码标注为：`text/typescript`

	<script type="text/javascript" src="dist/angular2.beta.stack.min.js"><script>
	<script type="text/typescript">
		import {Component} from "angular2/core";
		import {bootstrap} from "angular2/platform/browser";
		
		@Component({
			selector : "ez-app",
			template : "<h1>Hello</h1>"
		})
		class EzApp{}
		
		bootstrap(EzApp);
	</script>
	
## 构造

1.安装gulp
	
	~$ npm install -g gulp
	
2.安装gulp-concat和gulp-uglify

	~$ npm install gulp-concat gulp-uglify
	
3.执行gulp，生成dist/angular2-beta-stack.min.js

	~$ cd angular2-beta-stack
	~/angular2/beta-stack$ gulp

	
	
#### demo介绍
    1.快速上手
	    index1.html 	** hello world示例
	2.组件开发 - 声明元数据    
	    index2.html     ** selector - 声明选择符
	    index3.html     ** template/templateUrl - 声明模板
	    index4.html     ** styles/styleUrls - 设置样式
	    index5.html     ** properties - 声明属性
	    index6.html     ** 在子组件标签上定义的属性,并设置默认值
	    index7.html     ** events - 声明事件
	    index8.html     ** directives - 引用指令
	3.组件开发 - 模板基本语法    
	    index9.html     ** {{model}} - 文本插值
	    index10.html    ** [property] - 属性绑定 和 样式属性绑定
	    index11.html    ** (event) - 事件绑定
	    index12.html    ** #var - 局部变量
	4.组件开发 - 在模板中使用预置指令    
	    index13.html    ** NgStyle - 内联样式
	    index14.html    ** NgClass - 样式类
	    index15.html    ** NgIf- 条件逻辑
	    index16.html    ** NgSwitch - 分支逻辑
	    index17.html    ** NgFor- 循环逻辑
	    index18.html    ** | - 管道/Pipe  过滤器
	    index19.html    ** 预置过滤器
	    index20.html    ** 管道级联，多个管道
	    index21.html    ** 自定义过滤器
	    index22.html    ** 有状态管道：过滤器会自动检测数据变化，并输出
	    index23.html    ** AsyncPipe异步管道(异步过滤器)：等到服务器响应完成才会执行，详细看demo
	5.组件开发 - 在模板中处理表单输入
	    index24.html    ** NgForm - 表单指令
	    index25.html    ** NgControlName - 命名控件指令
	    index26.html    ** NgControlGroup - 命名控件组
	    index27.html    ** NgFormControl - 绑定已有控件对象
	    index28.html    ** NgFormModel - 绑定已有控件组
	6.指令开发 - 增强HTML功能 
	    index29.html    ** Directive - 定义指令元数据   
	    index30.html    ** inputs - 声明属性值映射：详情看demo中的3
	    index31.html    ** host - 声明事件监听：监听dom事件
	7.服务开发 - 封装与注入    
	    index32.html    ** 服务 - 封装可复用代码：把公用的逻辑抽出，封装成一个服务
	    index33.html    ** 注入服务 - providers。和index.32有很大区别
	    index34.html    ** 使用Injector - 注入器。实现注入，和index.33有很大区别
	    index34.html    ** 使用TOKEN - 服务标识。让依赖注入更简单
	    
	    
	    
	    
	    
	    
	    
	