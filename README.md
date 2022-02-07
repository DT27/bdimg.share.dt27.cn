HTTPS版百度分享
# 使用方法：
直接替换百度分享代码中的js文件连接即可。
例如百度分享官方代码：
```html
<div class="bdsharebuttonbox"><a href="#" class="bds_more" data-cmd="more"></a><a href="#" class="bds_qzone" data-cmd="qzone" title="分享到QQ空间"></a><a href="#" class="bds_tsina" data-cmd="tsina" title="分享到新浪微博"></a><a href="#" class="bds_tqq" data-cmd="tqq" title="分享到腾讯微博"></a><a href="#" class="bds_renren" data-cmd="renren" title="分享到人人网"></a><a href="#" class="bds_weixin" data-cmd="weixin" title="分享到微信"></a></div>
<script>window._bd_share_config={"common":{"bdSnsKey":{},"bdText":"","bdMini":"2","bdMiniList":false,"bdPic":"","bdStyle":"1","bdSize":"24"},"share":{}};with(document)0[(getElementsByTagName('head')[0]||body).appendChild(createElement('script')).src='http://bdimg.share.baidu.com/static/api/js/share.js?v=89860593.js?cdnversion='+~(-new Date()/36e5)];</script>
```
只需要将其中的
```
http://bdimg.share.baidu.com/static/api/js/share.js
```
替换为
```
https://bdimg.share.dt27.cn/share.js
```


另外站点https配置建议增加以下配置项来禁止加载非https图片：

    Header set Content-Security-Policy "img-src https: data:;"

