# HTML

## 什么是静态网页？什么是动态网页？

#### 类型：`基础`

#### 级别：`W1`、`W2`、`W3`、`W4`、`W5`、`W6`

#### 解答（2 分）

- **2：** 静态网页：没有与服务端发生交互的网页；动态网页：与服务端有交互的网页

## 谈谈你对 HTML 语义化的理解

#### 类型：`基础`

#### 级别：`W1`、`W2`、`W3`、`W4`、`W5`、`W6`

#### 解答（3 分）

- **1：** What：通过语义化标签对网站进行结构化；
- **1：** Why：便于浏览器解析，便于特殊设备解析，便于搜索引擎收录，提高代码的可维护性和复用性；
- **1：** How：`header`-文档头、`nav`-导航区、`section`-文档块、`article`-内容、`aside`-侧边栏-广告栏、`footer`-文档脚注；

## 谈谈你对锚点的理解

#### 类型：`基础`

#### 级别：`W1`、`W2`、`W3`、`W4`、`W5`、`W6`

#### 解答（2 分）

- **1：** What & Why：文档中某一行的记号，用于链接到文档中指定的位置；避免用户频繁滚动页面，提升用户体验；
- **1：** How：`<h2 id="know">谈谈你对锚点的理解 <a href="#know">​</a></h2>`、`<div><a name="know">​</a><a href="#know">​</a></div>`、``；

## 超链接有哪些常见的表现形式？

#### 类型：`基础`

#### 级别：`W1`、`W2`、`W3`、`W4`、`W5`、`W6`

#### 解答（2 分）

- **2：**
  + 跳转链接：页面跳转，`<a href="http://www.baidu.com">百度</a>`
  + 下载链接：下载资源，`<a href="data.zip">本地</a>`
  + 锚点链接：锚点跳转，`<a href="#know">​</a>`
  + 邮箱链接：唤起邮箱，`<a href="mailto:xxx@xxx.com">xxx</a>`
  + 空链接：返回页面顶部，`<a href="">​</a>`
  + 代码块：执行代码，`<a href="javascript:void(0);">​</a>`

## img 标签的 title 和 alt 属性作用

#### 类型：`基础`

#### 级别：`W1`、`W2`、`W3`、`W4`、`W5`、`W6`

#### 解答（1 分）

- **1：** `title`属性是当鼠标悬停在图片上时，显示的提示文本；`alt`属性是图片无法正常显示时，显示的文本，如：图片加载失败、图片被屏蔽等。

## src 与 href 的区别

#### 类型：`基础`

#### 级别：`W1`、`W2`、`W3`、`W4`、`W5`、`W6`

#### 解答（1 分）

- **1：** `src`属性是资源路径，引入资源，属于当前页不可缺少的部分，如：`src="http://www.baidu.com/logo.png"`；`href`属性是超链接，引用资源，表示该资源与当前页有关联，如：`href="http://www.baidu.com"`。

## iframe 有哪些特点（优缺点）？

#### 类型：`基础`

#### 级别：`W1`、`W2`、`W3`、`W4`、`W5`、`W6`

#### 解答（4 分）

- **2：** 优点：
  + 内容独立：iframe 中的元素、变量、样式是独立的；
  + 并行加载：浏览器可以同时加载一个页面中多个 iframe 的资源；
  + 灵活性强：可以引入各类网站，即使跨域；
- **2：** 缺点：
  + 不利于 SEO：iframe 没有语义，iframe 中的内容无法被搜索引擎收录；
  + 性能问题：iframe 中的内容无法被浏览器缓存，每次刷新都需要重新加载，多个 iframe 存在相同资源也会重复加载；
  + 通讯复杂：iframe 中两个页面之间无法直接通信，需要借助中间服务，如：postMessage、window.name 等；

## 谈谈你对 Web 标准以及 W3C 的理解和认识

#### 类型：`拓展`

#### 级别：`W4`、`W5`、`W6`

#### 解答（2 分）

- **1：** Web 标准指的是万维网（World Wide Web）上各种网页、网页元素、网页设计、网页交互等网页制作规范。W3C 是万维网联盟（World Wide Web Consortium），致力于制定和推广开放网络标准，以支持互联网和万维网发展。
- **1：** 标签要闭合，英文小写，且不要嵌套混乱，用标签语义化未提高技索的概率。使用外链式的 css 和 JS 脚本，使结构、样式、行为分离，内容能被更广泛的设备所访问，代码精简 开发组件化 ，代码易维护、 可复用，改版、升级方便。

## 什么是严格模式与混杂模式？

#### 类型：`拓展`

#### 级别：`W1`、`W2`、`W3`

#### 解答（1 分）

- **1：** 严格模式：是以浏览器支持的最高标准运行, 混杂模式：页面以宽松向下兼容的方式显示，模拟老式浏览器的行为。

## script、script async 和 script defer 的区别？

#### 类型：`拓展`

#### 级别：`W1`、`W2`、`W3`

#### 解答（2 分）

- **2：** script - HTML 解析中断，脚本被提取并立即执行。执行结束后，HTML 解析继续。  
  
  async - 脚本的提取、执行的过程与 HTML 解析过程并行，脚本执行完毕可能在 HTML 解析完毕之前。当脚本与页面上其他脚本独立时，可以使用 async，比如用作页面统计分析。  
  
  defer - 脚本仅提取过程与 HTML 解析过程并行，脚本的执行将在 HTML 解析完毕后进行。如果有多个含 defer 的脚本，脚本的执行顺序将按照在 document 中出现的位置，从上到下顺序执行。

## 浏览器乱码的原因是什么？如何解决？

#### 类型：`拓展`

#### 级别：`W1`、`W2`、`W3`

#### 解答（2 分）

- **1：原因**
    1.网页源代码是gbk的编码，而内容中的中文字是utf-8编码的，这样浏览器打开即会出现html乱码，反之也会出现乱码;  

    2.html网页编码是gbk，而程序从数据库中调出呈现是utf-8编码的内容也会造成编码乱码;  

    3.浏览器不能自动检测网页编码，造成网页乱码。
- **1：解决办法**
    1.如果网页设置编码是gbk，而数据库储存数据编码格式是UTF-8，此时需要程序查询数据库数据显示数据前进程序转码;  

    2.如果浏览器浏览时候出现网页乱码，在浏览器中找到转换编码的菜单进行转换;  

## CSS中 link 和@import 的区别是什么？

#### 类型：`拓展`

#### 级别：`W1`、`W2`、`W3`

#### 解答（1 分）

- **1：**   link属于HTML标签，而@import是CSS提供的页面被加载的时，link会同时被加载，而@import引用的CSS会等到页面被加载完再加载;  

  import只在IE5以上才能识别，而link是HTML标签，无兼容问题;  

  link方式的样式的权重 高于@import的权重。

## CSS中 transition和animation的区别？

#### 类型：`拓展`

#### 级别：`W1`、`W2`、`W3`

#### 解答（1 分）

- **1：**  Animation和transition大部分属性是相同的，他们都是随时间改变元素的属性值，他们的主要区别是transition需要触发一个事件才能改变属性，
而animation不需要触发任何事件的情况下才会随时间改变属性值，并且transition为2帧，从from .... to，而animation可以一帧一帧的。

## 什么是 DOCTYPE， 有何作用？

#### 类型：`拓展`

#### 级别：`W1`、`W2`、`W3`

#### 解答（1 分）

- **1：**  Doctype是HTML5的文档声明，通过它可以告诉浏览器，使用哪一个HTML版本标准解析文档。在浏览器发展的过程中，HTML出现过很多版本，不同的版本之间格式书写上略有差异。如果没有事先告诉浏览器，那么浏览器就不知道文档解析标准是什么？此时，大部分浏览器将开启最大兼容模式来解析网页，我们一般称为怪异模式，这不仅会降低解析效率，而且会在解析过程中产生一些难以预知的bug，所以文档声明是必须的。