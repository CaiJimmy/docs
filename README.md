# 介绍

![](.gitbook/assets/image%20%283%29.png)

### 功能

* 文章图片自带长宽比信息
* 图片懒加载 \(`loading="lazy"`\)
* 可以给分类 / 标签添加图片和介绍
* 归档页面
* 暗色模式 \(跟随系统设置\)
* 无 jQuery，纯原生 JavaScript
* 无 CSS 框架

**主题唯一的外部依赖是** [**Vibrant-Colors / node-vibrant**](https://github.com/Vibrant-Colors/node-vibrant) **这个库，没有使用到前端框架。**

文章缩略图使用了 Hugo 的 Image Processing 功能，自动裁剪成合适的大小来优化页面加载速度。缺点是第一次生成站点时耗时会比较长，第二次有缓存后就会恢复到正常速度（我博客生成速度 ~ 500ms ）。

页面头部加入了 Open Graph 标签，在 Telegram 或 Twitter 这些平台上贴链接时可以获得不错的效果。

### 版权

Licensed under the GNU General Public License v3.0

**请不要删除页脚的版权链接。**

如果要把主题移植到其他平台请提前通知我一声🙏。

### 捐赠

如果喜欢这个主题，欢迎通过以下链接来赞助其开发：

 [![Buy Me A Coffee](https://camo.githubusercontent.com/c58c9d4d7884c99daada0f44b7cf6a362f8c4fc7430aa860b5065e2c2d86b3af/68747470733a2f2f63646e2e6275796d6561636f666665652e636f6d2f627574746f6e732f76322f64656661756c742d677265656e2e706e67)](https://www.buymeacoffee.com/jimmycai)

多谢你的支持 ：）

### 致谢

* [Vibrant-Colors/node-vibrant](https://github.com/Vibrant-Colors/node-vibrant)
* [Normalize.css](https://necolas.github.io/normalize.css/)
* [Tabler icons](https://tablericons.com/)
* [Pure CSS implementation of Google Photos / 500px image layout](https://github.com/xieranmaya/blog/issues/6)
* [jonsuh/hamburgers](https://github.com/jonsuh/hamburgers)
* [PhotoSwipe](https://photoswipe.com/)
* [artchen/hexo-theme-element](https://github.com/artchen/hexo-theme-element)
* [MunifTanjim/minimo](https://github.com/MunifTanjim/minimo)
* [lepture/yue.css](https://github.com/lepture/yue.css)
* 相册语法来自 [Typlog](https://typlog.com/)

