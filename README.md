## 1. 书写规范

#### 1.1 项目结构
    ---/html/
    |---- /index       			    
    |---- /index/index.html         首页  
    |---- /user/ 				   与用户相关的页面  
    |---- /user/login.html          登录页
    ---/css/
    |---- /base.css       		  重置浏览器样式    
    |---- /page       			  逻辑页面的css
    |---- /page/pagename.css        单独书写的css
    |---- /common.css        	   css通用样式库
    ---/js/
    |---- /lib       			   公用组件
    |---- /lib/jquery.2.2.3.min.js  调用jq库文件 
    |---- /page       			  逻辑页面的js
    |---- /page/pagename.js         单独书写的js
    |---- /common.js    			公用方法
    ---/img/
    |---- /page       			  页面对应的图片
    |---- /page/wap      		   手机端图片夹
    |---- /page/wap/wap_icon.png    手机端图标
    |---- /logo.png       		  公用图片

#### 1.2 项目命名规范  

	* 项目：用项目对应的英文单词命名
	* 文件及文件夹:
		* 全部英文小写字母，可以使用中线，不可出现其他字符，如login,my-order
		* 调用 `/lib`里面的文件需包含版本号，压缩文件需包含`min`关键词，其他插件则可不包含，如：`/lib/jquery.1.9.1.js`

#### 1.3 格式&编码
	* 文本文件： `.xxx` UTF-8_\(无BOM\)_ 编码
	* 图片文件： `.png` _(PNG-24)_ `.jpg` _(压缩率8-12)_
	* 动态图片： `.gif`
	* 压缩文件： `.tar.gz` `.zip``.rar`

## 2. CSS 规范

#### 2.1 CSS 命名规范  
	* 所有的命名用小写的英文单词
	* 不使用简单的方位词直接命名，如“left”，“bottom”
	* 不缩写单词，除非一看就明白的单词
	* 长名称或词组可以使用下划线作为连接符
	* 避免选择器嵌套层级过多，少于3级
	* 不要随意使用id，id应该按需使用，而不能滥用
	* 使用CSS缩写属性 ，比如padding:0 10px 5px 5px等等，这样精简代码同时又能提高用户的阅读体验。
命名参考如下：
<table width="680px" border="0" style="border-collapse: collapse;">
<tbody>
    <tr>
        <th width="40%">CSS样式命名</th>
        <th width="60%">说明</th>
    </tr>
    <tr>
        <th colspan="2">网页公共命名</th>
    </tr>
    <tr>
        <td>wrapper</td>
        <td>页面外围控制整体布局宽度</td>
    </tr>
    <tr>
        <td>container或content</td>
        <td>容器,用于最外层</td>
    </tr>
    <tr>
        <td>layout</td>
        <td>布局</td>
    </tr>
    <tr>
        <td>head, header</td>
        <td>页头部分</td>
    </tr>
    <tr>
        <td>foot, footer</td>
        <td>页脚部分</td>
    </tr>
    <tr>
        <td>nav</td>
        <td>主导航</td>
    </tr>
    <tr>
        <td>sub_nav</td>
        <td>二级导航</td>
    </tr>
    <tr>
        <td>menu</td>
        <td>菜单</td>
    </tr>
    <tr>
        <td>sub_menu</td>
        <td>子菜单</td>
    </tr>
    <tr>
        <td>side_bar</td>
        <td>侧栏</td>
    </tr>
    <tr>
        <td>sidebar_l, sidebar_r</td>
        <td>左边栏或右边栏</td>
    </tr>
    <tr>
        <td>main</td>
        <td>页面主体</td>
    </tr>
    <tr>
        <td>tag</td>
        <td>标签</td>
    </tr>
    <tr>
        <td>msg message</td>
        <td>提示信息</td>
    </tr>
    <tr>
        <td>tips</td>
        <td>小技巧</td>
    </tr>
    <tr>
        <td>vote</td>
        <td>投票</td>
    </tr>
    <tr>
        <td>friendlink</td>
        <td>友情链接</td>
    </tr>
    <tr>
        <td>title</td>
        <td>标题</td>
    </tr>
    <tr>
        <td>summary</td>
        <td>摘要</td>
    </tr>
    <tr>
        <td>login_bar</td>
        <td>登录条</td>
    </tr>
    <tr>
        <td>search_input</td>
        <td>搜索输入框</td>
    </tr>
    <tr>
        <td>hot</td>
        <td>热门热点</td>
    </tr>
    <tr>
        <td>search</td>
        <td>搜索</td>
    </tr>
    <tr>
        <td>search_output</td>
        <td>搜索输出和搜索结果相似</td>
    </tr>
    <tr>
        <td>search_bar</td>
        <td>搜索条</td>
    </tr>
    <tr>
        <td>search_results</td>
        <td>搜索结果</td>
    </tr>
    <tr>
        <td>copyright</td>
        <td>版权信息</td>
    </tr>
    <tr>
        <td>branding</td>
        <td>商标</td>
    </tr>
    <tr>
        <td>logo</td>
        <td>网站LOGO标志</td>
    </tr>
    <tr>
        <td>site_info</td>
        <td>网站信息</td>
    </tr>
    <tr>
        <td>site_info_legal</td>
        <td>法律声明</td>
    </tr>
    <tr>
        <td>site_info_credits</td>
        <td>信誉</td>
    </tr>
    <tr>
        <td>join_us</td>
        <td>加入我们</td>
    </tr>
    <tr>
        <td>partner</td>
        <td>合作伙伴</td>
    </tr>
    <tr>
        <td>service</td>
        <td>服务</td>
    </tr>
    <tr>
        <td>regsiter</td>
        <td>注册</td>
    </tr>
    <tr>
        <td>arr arrow</td>
        <td>箭头</td>
    </tr>
    <tr>
        <td>guild</td>
        <td>指南</td>
    </tr>
    <tr>
        <td>site_map</td>
        <td>网站地图</td>
    </tr>
    <tr>
        <td>list</td>
        <td>列表</td>
    </tr>
    <tr>
        <td>home_page</td>
        <td>首页</td>
    </tr>
    <tr>
        <td>sub_page</td>
        <td>二级页面子页面</td>
    </tr>
    <tr>
        <td>tool, toolbar</td>
        <td>工具条</td>
    </tr>
    <tr>
        <td>drop</td>
        <td>下拉</td>
    </tr>
    <tr>
        <td>drop_menu</td>
        <td>下拉菜单</td>
    </tr>
    <tr>
        <td>status</td>
        <td>状态</td>
    </tr>
    <tr>
        <td>scroll</td>
        <td>滚动</td>
    </tr>
    <tr>
        <td>tab</td>
        <td>标签页</td>
    </tr>
    <tr>
        <td>left right center</td>
        <td>居左、中、右</td>
    </tr>
    <tr>
        <td>news</td>
        <td>新闻</td>
    </tr>
    <tr>
        <td>download</td>
        <td>下载</td>
    </tr>
    <tr>
        <td>banner</td>
        <td>广告条(顶部广告条)</td>
    </tr>
</tbody>
</table>
	
#### 2.2 CSS 书写规范
	* 向“无ID，无层级，无标签”准则靠拢，可有效提高重用性，减小文件大小，提升渲染效率


#### 2.3 CSS 注释格式
	* 用来区分页面的注释，如/******************************************产品中心****************************************/
	* 模块的注释,如/*首页导航栏*/
        
#### 2.4 CSS各属性的排列顺序：不做硬性要求
	* Positioning（定位，如position，top，z-index）
	* Box model（盒模型，如display，box-sizing，width，border）
	* Typographic（排版，如font，line-height，text-align）
	* Visual（视觉，如background，color,opacity）
	* Other（其他，如cursor）
	
	由于定位（positioning）可以从正常的文档流中移除元素，并且还能覆盖盒模型（box model）相关的样式，因此排在首位。盒模型决定了组件的尺寸和位置，因此排在第二位。
	其他属性只是影响组件的内部（inside）或者是不影响前两组属性，因此排在后面。
	


#### 2.5 CSS格式化

	使用不换行方式书写，增加书写速度
    .box{background: none repeat scroll 0 0 transparent;bottom: 11px;position: relative;width: 22px;z-index: 33;}

#### 2.6 CSS字体单位
	* px像素（Pixel），相对长度单位，像素px是相对于显示器屏幕分辨率而言的。
	* em是相对长度单位。相对于当前对象内文本的字体尺寸。如当前对行内文本的字体尺寸未被人为设置，则相对于浏览器的默认字体尺寸。
    * rem也是相对长度单位，但相对的只是HTML根元素。
    * vw代表视窗(Viewport)的宽度为1%，如果视窗宽度为1000px，那么50vw = 500px
    * vh代表窗口高度的百分，如果视窗高度为800px，那么50vh = 400px
	* 公司项目使用时注意事项：现有项目都是使用px作为单位，现推荐使用rem,vw,vh作为单位
	
## 3. JS 规范

### 3.1 JS命名规范
#### 3.1.1 JS 变量命名
	* 命名方法：小驼峰式命名法
	* 命名规范：前缀应当是名词。(函数的名字前缀为动词，以此区分变量和函数)
	* 命名建议：尽量在变量名字中体现所属类型，如:length、count等表示数字类型；而包含name、title表示为字符串类型。
	* 示例
		// 好的命名方式
		var maxCount = 10;
		var tableTitle = 'LoginTable';
		
		// 不好的命名方式
		var setCount = 10;
		var getTitle = 'LoginTable';

#### 3.1.2 JS 函数命名
	* 命名方法：小驼峰式命名法
	* 命名规范：前缀应当为动词
	* 命名建议：可使用常见动词约定
<table style="height:175px;width:676px;border-collapse:collapse" border="0" ="0">
	<tbody>
		<tr>
			<td style="text-align: center;">动词</td>
			<td>含义</td>
			<td>返回值</td>
		</tr>
		<tr>
		<td style="text-align: center;">can</td>
		<td>判断是否可执行某个动作(权限)</td>
		<td>函数返回一个布尔值。true：可执行；false：不可执行</td>
		</tr>
		<tr>
		<td style="text-align: center;">has</td>
		<td>判断是否含有某个值</td>
		<td>函数返回一个布尔值。true：含有此值；false：不含有此值</td>
		</tr>
		<tr>
		<td style="text-align: center;">is</td>
		<td>判断是否为某个值</td>
		<td>函数返回一个布尔值。true：为某个值；false：不为某个值</td>
		</tr>
		<tr>
		<td style="text-align: center;">get</td>
		<td>获取某个值</td>
		<td>函数返回一个非布尔值</td>
		</tr>
		<tr>
		<td style="text-align: center;">set</td>
		<td>设置某个值</td>
		<td>无返回值、返回是否设置成功或者返回链式对象</td>
		</tr>
		<tr>
		<td style="text-align: center;">load</td>
		<td>加载某些数据</td>
		<td>无返回值或者返回是否加载完成的结果</td>
		</tr>
	</tbody>
</table>

#### 3.1.3 JS 常量命名
	* 命名方法：名称全部大写
	* 命名规范：使用大写字母和下划线来组合命名，下划线用以分割单词
	* 示例
		var MAX_COUNT = 10;
		var URL = 'http://www.baidu.com';	

#### 3.1.4 JS 文件命名
	* 使用短线（-）或句点（.）作为分隔符号，推荐使用句点，最好使用小写英文字符，不要使用其他符号和扩展字符，如 jQuery UI 1.9.0 的源文件可命名为“jquery-ui-1.9.0.js”
	* 使用 .js 扩展名，这个扩展名的兼容性最好。其实任何扩展名都可以，只要是 text 类型、编码正确即可
	* 用句点分隔表示名称中的从属关系，范围大的在前，如jQuery 的表单插件 Form既可以命名为jquery.form.js
	 
#### 3.2 js 注释格式 
	* 使用多行注释,以/*开头，*/结尾

#### 3.3 js 注意事项
	* 书写格式
		* JS 换行缩进：采用tab（打散为4个空格）
		* 结束行需添加分号`;`
	* 性能
		* 尽量选用局部变量而不是全局变量
		* 尽量使用链式写法
		* 尽量减少DOM调用
		* 将js脚本放到页面底部
		* 使用jquery的data来存取数据，减少对dom的操作
		* 使用on方法绑定事件，这是jquery的推荐使用
		* 选择器的选择：尽量不用标签选择器，能用ID选择器的就不用class选择器
		
		

## 4. HTML 规范

#### 4.1 标签使用规范
	* 尽量减少标签层级
	* 双标签必须闭合，单标签用斜线闭合
	* HTML第一行统一使用HTML5标准<!DOCTYPE html>
	* 一律统一标签结尾斜杠的书写形式：`<br />` `<hr />` 注意之间空格
	* 避免使用已过时标签，如：`<font>` `<frame>` `<s>`
	* `<img>`标签默认缺省格式：`<img src="#" alt="缺省时文字" />`
	* `<a>`标签缺省格式：`<a href="#" title="链接名称">xxx</>` 注：`target="_blank"` 根据需求决定
	* style、link、script可省略type属性，因为 text/css 和 text/javascript 分别是他们的默认值
    
#### 4.2 HTML注释
	<!--内容-->
	 <div class="content">
		<p>content</p>
	  </div>
#### 4.3 注意事项
	* 手机端的自适应布局尽量采用弹性布局，而不是百分比
	* `css`文件都 置于头部
	* HTML换行缩进：采用 tab空格
	* 其他效果`js`及`统计代码` 文件置于尾部
    * 手机端的页面都按750px来做，显示效果按375px
	
## 5. Image 规范
#### 5.1 图片规范
	* 图片大小：切图时使用web格式保存，减小图片大小
	* 图片尺寸：一律采用整数，如20X20，50X50
	* 图片合并：小图片一律要合并，并保存对应的psd文件，以便后期修改
	

