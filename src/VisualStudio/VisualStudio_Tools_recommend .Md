 因为最近录制视频的缘故，很多朋友都在QQ群留言，或者微信公众号私信我，问我一些工具和一些插件啊，怎么使用的啊？那么今天我忙里偷闲整理一下清单，然后在这里面公布出来。

# Visual Studio 2017 扩展
> Visual Studio 2017 15.4.4 : 目前是最新的版本号，所有的工具&插件都支持这个版本号。所以请对号入座。
 - **[ReSharper](http://www.jetbrains.com/resharper/)** : 首先的是Resharper,这个基本是目前是我开发过程中必备的工具集，唯一的缺点就是吃内存，所以你的内存要是低于8G，就不要使用它了。它的特点可以快速重构、高亮显示错误、导航和搜索都很方便、智能提示、**智能复制**这个我特别喜欢等等，用着它你会感受到很多惊喜。

- **[Extensibility Tools](https://marketplace.visualstudio.com/items?itemName=MadsKristensen.ExtensibilityTools)** :必备工具，他是基于visual studio上的拓展功能，增加了编码显示、智能感知、强化智能提示、代码段处理、自动提示html的标签工具等特点，而且下面提到的部分工具也是基于它的强化。

- **[GitHub Extension for Visual Studio](https://visualstudio.github.com/)**: 在Visual Studio中连接到GitHub的插件，直接在插件上管理github上的大部分功能都涵盖了。你如果不知道github是啥，请自行搜索。

- **[BrowserSync](https://marketplace.visualstudio.com/items?itemName=MadsKristensen.BrowserSync)**: ASP.NET项目的Visual Studio扩展，利用Browser Link来同步表单域项，页面导航和滚动位置。简单来说就是你在开发的时候同时打开了5个页面，它可以帮助你同时刷新这5个页面。
- **[Browser Reload on Save](https://marketplace.visualstudio.com/items?itemName=MadsKristensen.BrowserReloadonSave)** : 这个工具可以和上面的**[BrowserSync](https://marketplace.visualstudio.com/items?itemName=MadsKristensen.BrowserSync)**
工具配合，你在修改某个页面的时候，保存了同时所有的页面都会自动保存及刷新哦。


-    **[CodeMaid](http://www.codemaid.net/ "CodeMaid")**： 可快速整理代码文件，清理不必要的代码和杂乱的格式。并在开发时实时提供代码复杂度的报告，以便帮助开发人员降低代码复杂度、提高代码质量。

- **[ImageOptimizer](https://marketplace.visualstudio.com/items?itemName=MadsKristensen.ImageOptimizer)**: 它是一个图片的优化工具，优化任何JPEG，PNG、Gif 格式的图片文件，基本可以做到无损优化，1M的图片优化后只有300KB左右。
- **[ImageSprites](https://github.com/madskristensen/ImageSprites)**: 少侠，听过雪碧图吗？这就是个雪碧图插件。帮助我们把所有的图片都整合在一个图片上，以降低对服务器的请求数量和节约我们的流量。
- **[Web Compiler](https://visualstudiogallery.msdn.microsoft.com/3b329021-cd7a-4a01-86fc-714c2d05bb6c)** : 帮助我们对LESS, Sass, JSX, ES6 和CoffeeScript 这些文件做解析，当然功能比这个要强大点，但是我基本只用了它们，如果你用了前后端分离。估计这个插件就要退出舞台了。
- **[Bundler & Minifier](https://visualstudiogallery.msdn.microsoft.com/9ec27da7-e24b-4d56-8064-fd7e88ac1c40)**:将多个js或者css文件合并为一个文件。道理和雪碧图一样，但是如果你用了前后端分离。估计这个插件就要退出舞台了。

- **[File Differ](https://marketplace.visualstudio.com/items?itemName=MadsKristensen.FileDiffer)**: 顾名思义用于比较两个文件的不同之处，自己想想业务场景，是不是很需要啊。
- **[File Icons](https://marketplace.visualstudio.com/items?itemName=MadsKristensen.FileIcons)** : 为解决方案资源管理器无法识别的文件添加图标。简单来说根据后缀名把文件图标改改。
- **[File Nesting](https://marketplace.visualstudio.com/items?itemName=MadsKristensen.FileNesting)** : 帮助您将两个文件嵌套在一起，也可以把嵌套在一起的文件拆开。场景：bootstrap.js可以和bootstrap.min.js折腾成一个文件。
- **[Open Command Extension](https://marketplace.visualstudio.com/items?itemName=MadsKristensen.OpenCommandLine)**:支持所有类型的控制台，如cmd，PowerShell，Bash等等。您可以通过在选项中设置路径和参数来轻松配置使用哪一个。

- **[Indent Guides](https://marketplace.visualstudio.com/items?itemName=SteveDowerMSFT.IndentGuides)**:为缩进添加竖线。

-  **[ZenCoding](https://marketplace.visualstudio.com/items?itemName=MadsKristensen.ZenCoding)** 使用仿CSS选择器的语法来快速开发HTML和CSS ——由Sergey Chikuyonok开发，可以快速提升你的写HTML页面的速度。当然它现在改名叫做“Emmet”了，但是在VS里面依然叫做ZenCoding。GitHub地址：[ZenCoding](https://github.com/madskristensen/ZenCodingVS)
- **[Markdown Editor](https://visualstudiogallery.msdn.microsoft.com/eaab33c3-437b-4918-8354-872dfe5d1bfe)**:一个在visual studio 中的markdown工具，虽然在VS中用markdown工具有点杀鸡用牛刀但是偶尔还是比较实用的。
- **[CSS AutoPrefixer](https://marketplace.visualstudio.com/items?itemName=MadsKristensen.CSSAutoPrefixer)**: 这个工具就可以检测你的CSS，也支持变量、混合宏、未来的CSS特性，内联图像等等。内置了[PostCSS](https://github.com/postcss/postcss) 让你少些很多前缀代码。

- **[HTML Snippet Pack](https://marketplace.visualstudio.com/items?itemName=MadsKristensen.HTMLSnippetPack)**: 帮助你快速写HTML页面提供的代码段，作用和ZenCoding类似。
- **[Bootstrap Snippet Pack](https://marketplace.visualstudio.com/items?itemName=EricLebetsamer.BootstrapSnippetPack)** : 使用Bootstrap框架的网页开发人员的代码片段包，超级实用。配合ZenCoding如有神助。
- **[JavaScript Snippet Pack](https://marketplace.visualstudio.com/items?itemName=MadsKristensen.JavaScriptSnippetPack)** : 顾名思义，JS的代码段快速工具。

# 最后推荐它

- **[ABP Code Generator](https://marketplace.visualstudio.com/items?itemName=werltm.ABPCodeGenerator)**: ABP框架配套的代码生成器，用于大家在日常开发过程中节约时间，把更多的精力放于业务逻辑的处理中。目前支持.net framework版本，暂时不支持.net core。这个是我自己做的工具，喜欢abp框架的可以下载配套和它一起使用。

# 如何安装
1 你可以打开“https://marketplace.visualstudio.com/vs” 将名字逐一的复制进去，然后搜索下载安装。
![官网.png](http://upload-images.jianshu.io/upload_images/1979022-7952543f44f52ef5.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/800)
2 另外一种方式,打开VS 找到**工具**菜单栏下面的扩展和更新，进行搜索**yoyocms**就可以下载**ABP代码生成器**了，如下图。
 ![导航图.png](http://upload-images.jianshu.io/upload_images/1979022-a9beb9c09b3a35cf.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)




