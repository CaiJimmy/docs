# 配置主题

{% hint style="warning" %}
 主题最新的配置文件可以在 [exampleSite/config.toml](https://github.com/CaiJimmy/hugo-theme-stack/blob/master/exampleSite/config.toml) 找到，本页面的内容可能会过期。
{% endhint %}

Hugo 的配置存放在站点根目录的 `config.toml` 里（其实也可以使用 YAML，但本主题默认提供的配置文件为 TOML 格式）

与主题相关的配置字段存放在 `[params]` 对象下：

## params

站点全局设置

| Name | Description |
| :--- | :---------- |
| `mainSections` | 在首页和归档页面输出来自指定 section 的文章。默认会输出放在 content/post 文件夹下的页面。  Ref: [Content Sections](https://gohugo.io/content-management/sections/)|
| `featuredImageField` | 特色图片使用的字段，默认为 image。不建议修改。 |
| `rssFullContent` | RSS 输出文章完整内容 |
| `favicon` | 站点的图标 |

## dateFormat

日期格式设置。Go 的时间格式相比其他语言有很大的不同，请参考官方文档：[dateFormat](https://gohugo.io/functions/dateformat/)

| Name | Description |
| :--- | :---------- |
| `dateFormat.published` | 文章发布日期格式 |
| `dateFormat.lastUpdated` | 文章更新日期格式 |

## Sidebar

与左侧边栏相关的设置。

| Name | Description |
| :--- | :---------- |
| `avatar` | 博主头像。<br><ul><li><code>local</code>是否在本地</li><li><code>src</code><ul><li>本地：**请把图片存放在站点根目录的 assets/img 文件夹下**。<br>例如 `assets/img/avatar.png`， 并填入 `img/avatar.png`。</li><li>外部：头像地址</li></ul></li></ul> |
| `emoji` | 头像底部的 Emoji。留空不显示。 |
| `subtitle` | 站点介绍

## Article

文章页面相关的设置

<table>
  <thead>
    <tr>
      <th style="text-align:left">Name</th>
      <th style="text-align:left">Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left"><code>article.license</code>
      </td>
      <td style="text-align:left">
        <p>&#x6587;&#x7AE0;&#x534F;&#x8BAE;&#x8BBE;&#x7F6E;&#xFF0C;&#x663E;&#x793A;&#x5728;&#x9875;&#x9762;&#x5E95;&#x90E8;</p>
        <p></p>
        <ul>
          <li><code>enabled</code>&#xFF1A; &#x662F;&#x5426;&#x5728;&#x6240;&#x6709;&#x6587;&#x7AE0;&#x5E95;&#x90E8;&#x663E;&#x793A;&#x534F;&#x8BAE;&#x4FE1;&#x606F;&#x3002;&#x53EF;&#x4EE5;&#x5728;&#x6587;&#x7AE0;&#x7684;
            Front Matter &#x63D2;&#x5165; <code>license: false</code> &#x6765;&#x5355;&#x72EC;&#x5173;&#x95ED;</li>
          <li><code>default</code>&#xFF1A; &#x9ED8;&#x8BA4;&#x6587;&#x7AE0;&#x534F;&#x8BAE;&#x3002;&#x53EF;&#x4EE5;&#x5728;&#x6587;&#x7AE0;&#x7684;
            Frontmatter &#x63D2;&#x5165; <code>license: &quot;My custom licence&quot;</code> &#x6765;&#x81EA;&#x5B9A;&#x4E49;</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

## Comments

Comment system related settings

<table>
  <thead>
    <tr>
      <th style="text-align:left">Name</th>
      <th style="text-align:left">Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left"><code>enabled</code>
      </td>
      <td style="text-align:left">&#x662F;&#x5426;&#x5728;&#x6587;&#x7AE0;&#x5E95;&#x90E8;&#x9ED8;&#x8BA4;&#x663E;&#x793A;&#x8BC4;&#x8BBA;&#x7CFB;&#x7EDF;</td>
    </tr>
    <tr>
      <td style="text-align:left"><code>provider</code>
      </td>
      <td style="text-align:left">
        <p>&#x8BC4;&#x8BBA;&#x7CFB;&#x7EDF;&#x63D0;&#x4F9B;&#x5546;&#x3002;&#x76EE;&#x524D;&#x652F;&#x6301;&#x7684;&#x6709;&#xFF1A;</p>
        <ul>
          <li><code>disqus</code>
            <ul>
              <li>&#x9700;&#x8981;&#x5728; config.toml &#x6DFB;&#x52A0; disqusShortname
                &#x5B57;&#x6BB5;&#x3002;&#x53C2;&#x8003;&#x5B98;&#x65B9;&#x6587;&#x6863;&#xFF1A;
                <a
                href="https://gohugo.io/content-management/comments/#configure-disqus">Configure Disqus</a>
              </li>
            </ul>
          </li>
          <li><code>utterances</code>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

{% hint style="info" %}
可以在 `layouts/partials/comments/provider/` 下新建 `{provider}.html` 来添加更多评论系统的支持。
{% endhint %}

## **Widgets**

主页右侧边栏小部件设置

<table>
  <thead>
    <tr>
      <th style="text-align:left">Name</th>
      <th style="text-align:left">Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left"><code>widgets.enabled</code>
      </td>
      <td style="text-align:left">
        <p>&#x6570;&#x7EC4;&#xFF0C;&#x5E26;&#x6709;&#x8981;&#x663E;&#x793A;&#x7684;&#x5C0F;&#x90E8;&#x4EF6;&#x7684;&#x540D;&#x5B57;&#x3002;&#x76EE;&#x524D;&#x53EF;&#x7528;&#x7684;&#x503C;&#xFF1A;</p>
        <ul>
          <li><code>archives</code>: &#x5F52;&#x6863;</li>
          <li><code>tag-cloud</code>: &#x6807;&#x7B7E;&#x4E91;</li>
          <li><code>search</code>: &#x641C;&#x7D22;</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><code>widgets.archives</code>
      </td>
      <td style="text-align:left">
        <p>&#x5F52;&#x6863;&#x5C0F;&#x90E8;&#x4EF6;&#x8BBE;&#x7F6E;</p>
        <ul>
          <li><code>limit</code>: &#x8F93;&#x51FA;&#x6761;&#x6570;&#x9650;&#x5236;</li>
          <li><code>path</code>: &#x5F52;&#x6863;&#x9875;&#x9762;&#x7684;&#x76F8;&#x5BF9;&#x8DEF;&#x5F84;&#x3002;&#x4F8B;&#x5982; <code>/archive</code>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><code>widgets.tagCloud</code>
      </td>
      <td style="text-align:left">
        <p>&#x6807;&#x7B7E;&#x4E91;&#x5C0F;&#x90E8;&#x4EF6;&#x8BBE;&#x7F6E;</p>
        <ul>
          <li><code>limit</code>: &#x8F93;&#x51FA;&#x6761;&#x6570;&#x9650;&#x5236;</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

## Opengraph

 [Open Graph](https://ogp.me/) 标签相关设置

<table>
  <thead>
    <tr>
      <th style="text-align:left">Name</th>
      <th style="text-align:left">Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left"><code>opengraph.twitter</code>
      </td>
      <td style="text-align:left">
        <p></p>
        <ul>
          <li><code>site</code>: &#x535A;&#x4E3B; Twitter &#x7528;&#x6237;&#x540D;</li>
          <li><code>card</code>: <a href="https://developer.twitter.com/en/docs/twitter-for-websites/cards/overview/abouts-cards">Twitter Card &#x6837;&#x5F0F;</a>&#xFF0C;&#x53EF;&#x9009;&#xFF1A;summary
            / summary_large_image</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

## Default Image

默认特色图片设置

| Name | Description |
| :--- | :--- |
| `defaultImage.opengraph` | Open Graph 标签默认图片 |

格式如下：

* `enabled` ：是否启用
* `src`：图片地址
* `local`： 是否为本地图片。如果设置成 `true` ，主题会在站点根目录的 `assets` 文件夹下寻找 `src`

{% hint style="info" %}
**推荐把图片放在本地**，因为这样能被主题自动裁剪成合适的尺寸。
{% endhint %}

