# 通用指南

 - NPM包管理器yarn(推荐)、cnpm

 - package.json中的版本最好锁定

 - 优先使用utf-8编码进行编码，如遇其他编码的模板，静态资源需保持utf-8编码

 - 移动端定义viewport属性，一般定义格式如下,如果网站需要进行放大/缩小，需要根据实际情况定义scale的比例

 ```
 <meta content="width=device-width, initial-scale=1.0, maximum-scale=1.0, minimum-scale=1.0, user-scalable=0;"
  name="viewport"/>
 ```

**UED要求:**

 - 所有可交互的操做,要有适当的响应,比如a:hover要字体或者背景变化之类的提示.

 - 对于异步操作,需要做友好的提示.如:提交按钮变成disabled状态.

 - 对于所有用户操或者异步交互数据做异常处理,并做相应提示.


**代码优化:**

 - 尽量减少http请求数,合并请求次数,压缩代码等

 - 对于图片要采用合适的压缩方法,对于UI提供的图片要学会自行压缩.不得上传过大的图片文件.

 - 对于过大,过多的图片,要求使用懒加载文法.

 - Html代码要尽量减少dom层级

 - Css 代码要有可重用性,背景图片尽量拼合在一张图片里.如有矢量图标尽量用iconfont

 - JS 优化:尽量少用事件代理.尽量减少dom渲染次数.

**推荐阅读**

 - [移动WEB性能](http://www.webperformancetoday.com/tag/mobile-web-performance/)
 - [优化WEB缓存](https://developers.google.com/speed/docs/best-practices/caching)
 - [最小化RTT次数](https://developers.google.com/speed/docs/best-practices/rtt)
 - [最小化请求负载](https://developers.google.com/speed/docs/best-practices/payload)
 - [优化浏览器渲染](https://developers.google.com/speed/docs/best-practices/rendering)


