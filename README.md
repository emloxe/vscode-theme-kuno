# 自定义配置vs code 主题

## 配置文件
“文件-首选项-颜色主题”即可显示所有可用的颜色主题，上下选择后Enter即可。也可通过Ctrl+Shift+P输入color theme回车后调出“首选项：颜色主题”面板。

记VSCode的安装目录为$RELEASE(我的安装目录为`C:\\Users\\Administrator\\AppData\\Local\\Programs\\Microsoft VS Code`)，默认的颜色主题配置文件都位于`$RELEASE/resources/app/extensions`目录中。以theme-开头的目录即为颜色主题配置（事实上，其中有些是文件图标主题）。除若干主题会共用一个目录外（theme-defaults），大多数主题都是一个主题一个目录。

每个颜色主题配置目录包含以下文件：themes目录、OSSREADME.json、package.json。themes目录下通常使用.json设置具体的配色方案；OSSREADME.json描述版权等相关信息，可以忽略；package.json令VSCode读取后能区分不同的配色方案。

下面新增一个灰色调颜色主题。在`$RELEASE/resources/app/extensions`目录下新增如下目录结构。如果你不关心配置文件相关参数的解释，可无需细读后面内容，只需将相应的配置文本复制至配置文件中即可，但需注意文件均为UTF-8编码。

```
$RELEASE/resources/app/extensions/
 \\_ theme-kuno/
     \_ themes/
     |   \_ kuno-color-theme.json
     |_ package.json
```

详细参数可参考
https://www.sublimetext.com/docs/3/scope_naming.html

## kuno主题
github中文件为我自定义的主题，使用方式只需要将文件粘贴在`$resources/app/extensions/theme-kuno`中，“文件-首选项-颜色主题”选择kuno即可