# 快速开始

> `Fu Doc`支持将接口文档同步至第三方文档系统中 让你更加专注于程序开发 减少维护接口文档的工作量

!>目前支持的第三方文档系统有`YApi`、`ShowDoc` 后续还将继续接入其他第三方文档系统

## 使用

- 进入配置页面`Settings`->`Fu Doc`->`Fu Doc Sync`配置你需要同步到指定文档系统的地址
- 快捷键`ALT+S`(默认方式同步)、`ALT+SHIFT+S`(开启窗口方式同步)
- 右键菜单选择 `Fu Doc Sync` OR `Fu Doc Sync Confirm`
- 选择需要同步到哪一个分类下（可通过配置选择程序自动创建还是用户选择）
- 即可去该文档系统中查看当前接口

## 特性

- 支持通过配置自定义文档模板生成文档（`YApi可自定义配置备注内容`）
- 支持mock真实数据到接口文档中（`依赖` [Fu Request](zh-cn/request/quikstart.md)）
- 支持用户自行选择需要将接口文档同步到第三方文档系统中指定项目的指定分类下
- 支持记忆功能 如第一次选择同步至A分类下 下一次同步则无需用户选择可默认直接同步至A分类下(可通过`ALT+SHIFT+S`再次弹框选择同步至其他分类下)
- 支持一次性批量同步多个接口 可自行勾选哪些需要同步 哪些不需要同步 并且实时查看每一个接口同步状态 且支持`随时终止同步`
- 支持通过鉴权方式登录文档系统 让文档系统知道是哪个用户在同步文档 在文档系统中留痕
