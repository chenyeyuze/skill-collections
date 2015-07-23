# 前端组件整理（持续更新中。。。）
## 目录
* [工具类](#tool)
* [浏览器增强类](#browser-strong)
* [表单类](#form)
* [图片类](#img)
* [通用UI组件类](#ui)
* [专用工具类](#specialtool)
* [移动端框架](#mobile)
* [其他类](#other)
* [JS Plugins仓库](#repository)

## <a name="tool">工具类</a>
* 方便操作对象，数组等的工具库
    * [underscore.js](http://underscorejs.org/)提供了一整套函数式编程的实用功能，但是没有扩展任何JavaScript内置对象
    * [immutable](https://github.com/facebook/immutable-js) facebook的，持久化JS的集合数据
    * [lo-dash](http://lodash.com/) 与underscore.js的api基本一致。与underscore比其优势是，效率高；可自定义构建
    * [Sugar](https://github.com/andrewplummer/Sugar/) 在原生对象上增加一些工具方法
    * [functional.js](https://github.com/leecrossley/functional-js/) 提够了一些Curry的支持
    * [bacon.js](https://github.com/baconjs/bacon.js/) 函数式编程，cool
    * [streamjs](https://github.com/winterbe/streamjs) 用流的方式来对数组，对象进行系列操作
    * [jsonSelect](http://jsonselect.org/#docs) 像CSS3选择器一样去查询Json数据
* 异步流程控制
    * 发布订阅
        * [eventproxy](https://github.com/JacksonTian/eventproxy) 朴灵出品
        * [Arbiter.js](http://arbiterjs.com/)
    * [q](https://github.com/kriskowal/q/) Promise风格的
    * [Async.js](https://github.com/caolan/async/)
* 时间库
    * [moment](http://momentjs.com/)
    * [datejs](https://github.com/datejs/Datejs)
* 浏览器探测
    * [Bowser](https://github.com/ded/bowser) 探测具体浏览器和版本
    * [ua-parser-js](https://github.com/faisalman/ua-parser-js) 探测具体浏览器和版本，操作系统，设备类型等
* 调试地图
    * [JavaScript Debug](http://benalman.com/projects/javascript-debug-console-log/) 对console.log的简单封装，当浏览器不支持console.log时，输出在一个页面元素里
    * [log](https://github.com/adamschwartz/log) 让控制台输出的log有样式
* [uri.js](https://github.com/medialize/URI.js) uri操作
* [cookie](https://github.com/ScottHamper/Cookies) 增删改cookie的工具库
* [BigDecimal.js](https://github.com/dtrebbien/BigDecimal.js) 提高精度的数字操作
* [big.js](https://github.com/MikeMcl/big.js)提高精度的数字操作
* 前端数据库
    * [taffydb](http://www.taffydb.com/) 像操作mongo一样
    * [其他](http://blog.jobbole.com/31166/) 真不少，选择一款自己的哦


## <a name="browser-strong">浏览器增强类</a>
### 让一些旧浏览器变牛逼的库
* [Selectivizr](https://github.com/keithclark/selectivizr)  让IE 6-8一些的css3选择器
* [ieBetter](https://github.com/zhangxinxu/ieBetter.js) 让ie6-8有高级浏览器的特性
* [ExplorerCanvas](https://github.com/arv/ExplorerCanvas) 让IE8-的浏览器支持canvas
* [CSS3 Pie](http://css3pie.com/) 让IE6-9支持border-radious,box-shadow,linear-gradient。 可以使用.htc文件（注意Mine type）或.js文件。在用Pie.js时，box-radious的元素有背景色时，不显示背景色。。。
* [https://github.com/anselmh/object-fit](https://github.com/anselmh/object-fit) 让浏览器支持`object-fit`这css规则
* [HTML5 Cross Browser Polyfills](https://github.com/Modernizr/Modernizr/wiki/HTML5-Cross-Browser-Polyfills) 一堆Polyfills

### 选择器增强
* [Lining.js](https://github.com/zmmbreeze/lining.js) 让浏览器实现类似`::nth-line(), ::nth-last-line()`的效果

### 未归类
* [prefixfree](https://github.com/LeaVerou/prefixfree/) 用了它，写css时，就不需要加浏览器的前缀了

## <a name="form">表单类</a>
### 上传组件
* [jquery-fileapi](http://rubaxa.github.io/jquery.fileapi/) 上传裁剪图片，上传多张文件，拖拽上传，视频webcam上传
* [AjaxFileUpload](https://github.com/davgothic/AjaxFileUpload) ajax上传
* [jQuery File Upload](https://blueimp.github.io/jQuery-File-Upload/) 多文件、拖拽上传、进度条、验证、预览图片、音频视频、跨域，客户端图片重新调整等功能
* [multiple-file-upload](http://www.fyneworks.com/jquery/multiple-file-upload/) 多文件上传
* [uploadify](http://www.uploadify.com/documentation/) 需要flash

### 树组件
* [zTree](http://www.ztree.me/v3/main.php#_zTreeInfo) 文件树形视图控件

### 表单验证
* [jquery-validation](https://github.com/jzaefferer/jquery-validation)
* [jQuery-Validation-Engine](http://posabsolute.github.io/jQuery-Validation-Engine/)
* [parsleyjs](http://parsleyjs.org/) jQuery >= 1.8才能使用

### 表单元素美化 
* [uniform](https://github.com/pixelmatrix/uniform) 提供对下拉框，单，复选框，按钮等表单元素的美化
* [DropKick](https://github.com/Robdel12/DropKick) 下拉框，单，多选。外观比uniform好
* [switchery](http://abpetkov.github.io/switchery/) ios7风格的开关组件
* [nouislider](http://refreshless.com/nouislider/) 用滚动条来设置/控制（音量等）
* [range.css](http://danielstern.ca/range.css/) 美化`input[type=range]`元素的外观  
* 多选下拉框 
       * [select2](http://ivaynberg.github.io/select2/index.html) 多选下拉框
       * [MULTIPLE-SELECT](http://wenzhixin.net.cn/p/multiple-select/docs/index.html?locale=zh_CN) 多选下拉框
       * [jQueryUIMultiSelectWidget](http://www.erichynds.com/examples/jquery-ui-multiselect-widget/demos/#basic) 多选下拉框


## <a name="img">图片类</a>
* [holderjs](http://imsky.github.io/holder/) 生成占位图片
* [jquery_lazy.load](https://github.com/tuupola/jquery_lazyload) 图片延迟加载
* [imagesLoaded](http://desandro.github.io/imagesloaded/) 选取的图片都加载好后执行调回

### 浏览图片
* [fancybox](http://fancyapps.com/fancybox/) 弹出查看图片，视屏等等 [demo](http://fancyapps.com/fancybox/demo/)
* [yoxview](http://www.yoxigen.com/yoxview/) 弹出查看图片，图片尺寸缩放很自然
* [FlexSlider 2](http://flexslider.woothemes.com/index.html)响应式幻灯片，切换视频/切换图片
* [bxslider](http://bxslider.com/) 响应式幻灯片
* [lightbox2](http://lokeshdhakar.com/projects/lightbox2/) 
* [Lightbox for Bootstrap 3](http://ashleydw.github.io/lightbox/) 基于bootstrap3的modal做的幻灯片
* [photoswipe](http://photoswipe.com/) 有分享按钮的响应式图片浏览组件
* [coin-slider](https://github.com/kopipejst/coin-slider/) 兼容IE6。蛮好的~。不过其切换方式是一块块的。不能配置切换方式。。。
* [wowslider](http://wowslider.com/rq/jquery-image-viewer/)  幻灯切换时各种很炫的效果。收费。
* [cycle2](http://jquery.malsup.com/cycle2/) 普通的幻灯，竟然不支持垂直滚动。。。
* [jcarousel](http://sorgalla.com/jcarousel/) 普通的幻灯，不兼容IE6

### 图片墙(瀑布流)
* [wookmark](http://www.wookmark.com/jquery-plugin)
* [waterfall](https://github.com/duitang/waterfall) 堆糖瀑布流图片墙，国人的,自适应
* [masonry](https://github.com/desandro/masonry)
* [Grid-A-Licious](http://suprb.com/apps/gridalicious/) 自适应
* [blocksit](http://www.inwebson.com/demo/blocksit-js/) 自适应

### 裁剪图片
* [Jcrop](http://deepliquid.com/content/Jcrop.html) 

## <a name="ui">通用UI组件类</a>

### 时间选取组件
* [jQuery ui datepicker](http://jqueryui.com/datepicker/) 经典，不是很好看
* [pickadate](http://amsul.ca/pickadate.js/) 轻量级，手机友好的，漂亮。但貌似只能在弹出层中显示，而没有下拉这种方式显示。
* [zebra-datepicker](http://stefangabos.ro/jquery/zebra-datepicker/) 可配置性很强。但貌似只能在弹出在右上方。。。
* [bootstrap-datepicker](http://www.eyecon.ro/bootstrap-datepicker/) bootstrap风格。
* [dateRangePicker](https://github.com/dangrossman/bootstrap-daterangepicker) 选取时间段。bootstrap风格。该组件依赖Twitter Bootstrap, Moment.js和jQuery.
* [My97 DatePicker](http://www.my97.net/) 谁用谁知道，炒鸡好用，好多网站和企业系统用，貌似12306也用
* [mobiscroll](https://github.com/acidb/mobiscroll)移动端日期选择器，该公司的组件其他是收费的，日期免费

### 滚动条组件
* [perfect scrollbar](https://github.com/noraesae/perfect-scrollbar) 轻量级的滚动条。外观与mac上chrome的滚动条一样。
* [iscroll](http://iscrolljs.com) 在移动设备上用不错
* [jQuery slimScroll](http://rocha.la/jQuery-slimScroll) 监听scroll事件，隐藏显示滚动条
* [jquery-scrollspy](https://github.com/sxalexander/jquery-scrollspy) 
* [bootstrap-scrollspy](http://v3.bootcss.com/javascript/#scrollspy) 

###提示组件
* [opentip](http://www.opentip.org/) 漂亮的提示组件，各种方向
* [simple-hint](https://github.com/catc/simple-hint) 提示信息。用css做的。兼容性IE 9+。

### 表格组件
* [datatables](http://www.datatables.net/) 表格可交互（对内容进行排序，删除等）
* [backgrid](http://backgridjs.com/) 各种功能，带分页，可编辑表格内容。很棒。
* [JqGrid](http://www.trirand.com/blog/?page_id=5) jqGrid相关的几个表格组件,jqGrid，treeGrid
* [excellentexport](https://github.com/jmaister/excellentexport) 把表格的内容生成excel。兼容 Firefox, Chrome, IE6+

### 排序组件
* [Sortable](http://rubaxa.github.io/Sortable/) 拖拽排序，包括文字、图片等都可以排序 

### 菜单组件
* [Sidr](http://www.berriart.com/sidr/) 响应式的侧边菜单栏
* [flexnav](https://github.com/indyplanets/flexnav) 响应式菜单栏
* [smartmenus](http://www.smartmenus.org/) 响应式菜单栏

###进度条
* [nprogress](https://github.com/rstacruz/nprogress) github 9k+ stars google,youtube都在用啊
* [pacejs](http://github.hubspot.com/pace/docs/welcome/) 7k+ 个人认为很不错的一款
* [nanobar](https://github.com/jacoborus/nanobar) 轻量款
* [cprogress](http://p.ar2oor.pl/cprogress/) 转轮式进度条

### 选取颜色
* [Spectrum](http://bgrins.github.io/spectrum/?color=&color2=%233355cc&color3=%23000000#toc0)

### 编辑器
* [ace](http://ace.c9.io) 代码编辑器，可以用来做demo演示
* [codemirror](http://codemirror.net/) 代码编辑器，可以用来做在线代码编辑器，可代码高亮，语法检查等
* [ckeditor](http://ckeditor.com/) 个人感觉比较重，自己曾经二次开发过，也改过其源码
* [kindeditor](http://kindeditor.net/demo.php) 国人做的，好些网站也用
* [ueditor](http://ueditor.baidu.com/website/) 百度做的
* [tinymce](http://www.tinymce.com/tryit/full.php) 对html内容进行实时的编辑
* [summernote](https://github.com/summernote/summernote) 在移动设备上用不错

###代码高亮
* [syntaxhighlighter](https://github.com/syntaxhighlighter/syntaxhighlighter) 好多网站使用此组件
* [highlightjs](https://highlightjs.org/)  也很不错
* [google-code-prettify](https://code.google.com/p/google-code-prettify/)
* [DlHighlight](http://mihai.bazon.net/projects/javascript-syntax-highlighting-engine)仅支持JavaScript、CSS、XML、HTML 这4语法高亮
* [其他](https://codegeekz.com/15-code-syntax-highlighters-to-prettify-your-code/)

### HTML5播放器
* [jwplayer](http://www.jwplayer.com/) 被大量网站使用
* [videojs](https://github.com/videojs/video.js) HTML5视频播放器，支持HTML5和Flash
* [html5media](http://html5media.info/) 简单的h5player，轻量级
* [jplayer](http://jplayer.org/) 功能强太，可换肤
* [jQueryMedia](http://jquery.malsup.com/media/) 网页插入多媒体文件


### 弹出框
* [Magnific-Popup](https://github.com/dimsemenov/Magnific-Popup) 可以做图片查看/兼容PC，Mobile。还不错，有6k+的star
* [layer](https://github.com/sentsin/layer) 国人开发的，兼容ie6+。不喜欢其调用方式。

### 自适应textarea高度
* [AutoSize](http://www.jacklmoore.com/autosize/) 自适应textarea高度
* [flexText](https://github.com/alexdunphy/flexText)

### 动画效果
* [mixitup](https://mixitup.kunkalabs.com/) 用漂亮的动画效果来完成排序和筛选
* [jQuery.Marquee](https://github.com/aamirafridi/jQuery.Marquee) 跑马灯效果
* [quickflip](http://jonraasch.com/blog/quickflip-jquery-plugin) 卡片翻转效果
* [卡片翻转效果2](http://nnattawat.github.io/flip/) 兼容性可以。写的比较简单：1，只支持x方向翻转 2,类名都是规定好的 3，只能被调用一次。 需要改写一下。改进版见[这里](https://github.com/iamjoel/be-grace-front-end-developer/tree/master/my-lib/flip/quickflip.js)
* [TheaterJS](https://github.com/Zhouzi/TheaterJS) 模拟两个人在屏幕上对话，像打字聊天
* [midnight.js](https://github.com/Aerolab/midnight.js) 文字颜色随着背景变，屌炸了
* [color-animation](http://www.bitstorm.org/jquery/color-animation/) jquery的颜色渐变动画插件。jquery的动画不支持颜色值的变化。改库提供了这个支持。
* [transit](https://github.com/rstacruz/jquery.transit) 对元素进行css的变换
* [velocity](http://julian.com/research/velocity/) 动画加速

#### 视觉差插件
* [scrollorama](https://github.com/johnpolacek/scrollorama) 比较简单 
* [superscrollorama](https://github.com/johnpolacek/superscrollorama) 能做的效果更多，但要用第三方Tween的库，使用起来比较复杂。
* [scrolldeck](https://github.com/johnpolacek/scrolldeck.js)

###分页组件
* [jQuery Pagination](http://esimakin.github.io/twbs-pagination/)
* [11款分页](http://www.htmleaf.com/css3/daohangcaidan/201501241268.html)

###小组件
* [Widgster](https://github.com/flatlogic/widgster)小的jQuery插件，提供简单的方式处理像伸缩、关闭、异步刷新、全屏的效果
* [flippant](https://github.com/mintchaos/flippant.js)仅仅关注于翻转效果的组件
* [Intro.js](http://usablica.github.io/intro.js/) 用来介绍网站的功能很不错。也可以做新手引导。
* [blockUI](http://jquery.malsup.com/block/) Lolding组件。
* [dotdotdot](https://github.com/BeSite/jQuery.dotdotdot) 文字溢出时，添加在文字末尾加省略号
* [AnythingZoomer](https://github.com/CSS-Tricks/AnythingZoomer/) 放大镜功能
* [please](http://www.checkman.io/please/) 按要求随机舒服的颜色


### flash
* [swfobj](http://code.google.com/p/swfobject/wiki/documentation) 能够自动检测PC、Mac机器上各种主流浏览器对Flash插件的支持情况。它使得插入Flash媒体资源尽量简捷、安全。而且它是非常符合搜索引擎优化的原则的。此外，它能够避免您的HTML、XHTML中出现object、embed等非标准标签，从而符合更加标准。

## <a name="specialtool">专用工具类</a>
### 数据可视化(图表)
* [Echarts](http://echarts.baidu.com/) 百度出品
* [highcharts](http://www.highcharts.com/) 功能强大。是收费的。
* [Plottable.JS](http://plottablejs.org/) 基于D3的一个图表库
* [flot](http://www.flotcharts.org/) 文档不给力
* [chartJs](http://www.chartjs.org/) [中文文档](http://www.bootcss.com/p/chart.js/docs/)  demo很漂亮，很清晰。比较轻量级。
* [ichartJs](http://www.ichartjs.com/) 中国的一个家伙搞的，感觉还不错。
* [jQuery Sparklines](http://omnipotent.net/jquery.sparkline/#s-about) 星波图
* [rickshaw](http://code.shutterstock.com/rickshaw/) 交互式时间序列图
* [D3](http://d3js.org/) 让数据富有生命，并绚丽夺目
* [Two](http://jonobr1.github.io/two.js/#examples) 二维绘制图API

### 待办事宜日历
* [full calendar](http://arshaw.com/fullcalendar/) 支持脱放的方式来改变待办事宜的时间
* [Simple Events Calendar](http://codecanyon.net/item/simple-events-calendar-js/full_screen_preview/462149?ref=themespotters) 外观很喜欢。收费 5$

### 展示
* [Impress.js](https://developer.cdn.mozilla.net/media/uploads/demos/b/a/bartaz/54e3827142e4149a5c01db64c9517c84/impressjs_1333223745_demo_package/index.html#/bored) 各种旋转，和奇特的体验
* [fullPage](http://alvarotrigo.com/fullPage) 全屏显示。用滚轮来翻页
* [pagePiling](http://alvarotrigo.com/pagePiling/) 和fullPage类似
* [turn.js](https://github.com/blasten/turn.js) 做一本书，带漂亮的翻页的效果
* [appshowcase](http://www.htmleaf.com/css3/css3donghua/20141019233.html) 展示app页面的组件，效果很炫，做app宣讲用很不错
* [remark](https://github.com/gnab/remark) 网页幻灯片，做PPT，做书都行
* [reveal](https://github.com/hakimel/reveal.js) 3d滚动。做ppt相当不错
* [nodePPT](https://github.com/ksky521/nodePPT) 国人做的，做ppt也相当不错。有些方面比 reveal做的还好。但生成导出的html有些问题
* [Deck.js](http://imakewebthings.com/deck.js/)

###地图处理
* [openlayer](http://openlayers.org/) 个人用过OpenLayer2，新版是OpenLayer3
* [mapbox](https://www.mapbox.com/developers/) 定制化的地图，没试过，但看页面很炫
* [jQuery Mapael](http://www.vincentbroute.fr/mapael/) 在地图上建立漂亮的可视化数据模型
 
### 压缩文件
* [jszip](https://stuk.github.io/jszip/) 建立，读取，编辑zip文件

### 拖拽组件
* [jQueryEventDragDrop](http://threedubmedia.com/code/event/drag) 不错的拖拽组件


## <a name="mobile">移动端框架</a>
* [App Framework](http://app-framework-software.intel.com/) 
* [jQuery Mobile](https://jquerymobile.com/)

## <a name="other">其他类</a>
* [Ink](http://zurb.com/ink/) 响应式html邮件框架
* [性能测试](http://benchmarkjs.com/)
* 抓取，解析RSS内容（不能跨域，所以后台要做代理，所谓的解析Rss其实就是解析xml）
    * [jFeed](https://github.com/jfhovinne/jFeed)
    * [jRss](https://github.com/malderete/jRss)  简单版的jFeed
* [scriptcam](http://www.scriptcam.com/) 与摄像头交互

## <a name="repository">JS Plugins仓库</a>
* [jster](http://jster.net/)
* [awesome-nodejs](https://github.com/vndmtrx/awesome-nodejs)


####部分参考[前端整理]：(https://github.com/iamjoel/front-end-plugins)
