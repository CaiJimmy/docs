# 开始使用

## 环境要求

**最低 Hugo 版本要求为 0.74.0。**

以下情况需要用到 Hugo Extended 版本：

* 修改 SCSS 文件
* 或使用 GitHub 仓库的最新版本

第一次使用 Hugo 可以参考官方的安装手册：

{% embed url="https://gohugo.io/getting-started/installing/" %}

如果你在使用 Windows，我推荐使用 [Scoop](https://scoop.sh/) 来安装 Hugo：

```text
scoop install hugo-extended
```

## 下载主题

可以直接使用 GitHub 页面的 _Code_ 按钮来下载最新版本的主题：

![](.gitbook/assets/image%20%285%29.png)

下载后把 `hugo-theme-stack-master` 改名为 `hugo-theme-stack` 并放到站点目录的 `theme` 文件夹下。

如果是第一次使用本主题，建议把 `exampleSite` 文件夹中的 `assets` 和 `config.toml` 复制到站点目录下。后者是 Hugo 站点的配置文件，已经写入了主题的可配置字段。

