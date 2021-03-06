本项目基于VuePress构建，因此可能会有一些编写/提交前需要注意的东西。

## 编写需要注意的

在编写前，请先安装一些node.js包。在项目目录下运行以下代码：
``` bat
npm install
```
运行完成后，你的所有依赖都会被安装。

### 文件结构

所有的教程Markdown文件都位于`docs`目录下，第一节位于1文件夹，第二节位于2文件夹，以此类推。

所有的图片文件都位于`docs/.vuepress/public`目录下，第一节位于1文件夹，第二节位于2文件夹，以此类推。其中sv.ico与sv.png为网页标题和导航栏的图片文件，请不要修改。

其他文件均不需要修改。

### 文档注意事项

在一些编辑器（例如Visual Studio Code）中图片和提示框可能无法正确显示，因此你可以运行根目录下的`debug.bat`在本地启动一个预览服务器。

你可以在文档中使用提示/注意/警告框

提示框：

``` markdown
::: tip 标题
内容
:::
```
注意框：

``` markdown
::: warning 标题
内容
:::
```
警告框：

``` markdown
::: danger 标题
内容
:::
```

图片请按以下方式插入：

``` markdown
![图片简介](图片地址)
```
其中图片地址为（以`docs/.vuepress/public`文件夹下的`1/1.3.png`为例）：/synthesizer-v-r2-docs/1/1.3.png

### 教程编写结束后
请在文档末尾**添加以下代码以启动评论系统**：
``` markdown
<Vssue :title="$title" />
```
如果你编写了一个新的章节，请修改`docs/.vuepress/config.js`中第30行左右的你编写章节的导航地址。

## 提交需要注意的

请在Github提交！Gitee只做国内镜像！

在你的教程编写完毕后即可直接提交Pull Request。