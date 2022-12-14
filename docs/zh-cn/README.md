# FuDoc

> 一个提升你工作效率的接口文档生成插件

# 概述

> `Fu Doc`可以一键帮你生成接口文档. 相比于`Swagger` `Api Fox` `Yapi`等. `Fu Doc`更能帮你提升工作效率.
使用`Fu Doc`不需要添加任何依赖, 不需要额外去配置一堆参数. 只需要按下快捷键就能生成你平时需要花费大量时间编写的接口文档
你只需要按照`JAVA DOC`规范写好注释即可

查看[快速开始](zh-cn/quickstart.md)了解详情。

## 特性

- 对开发项目完全零侵入
- 依托与IDEA插件市场 安装方便 使用简单 无任何学习成本
- 兼容`@Valid`校验注解
- 支持读取自定义注解内容渲染到接口文档
- 支持在接口文档模板中直接通过`${fudoc.tagName}`的方式获取注释内容
- 支持自定义编辑接口文档模板
- 支持枚举类生成`key-value`格式和`table`格式的字典说明
- 支持在字段上标识`@see`注解引用枚举 生成该字段的枚举字段描述说明信息
- 支持`Dubbo` `Feign`等接口生成接口文档
- 支持对`JAVA`对象的属性生成markdown格式的表格信息展示


## 示例

可以查看 [示例](zh-cn/example.md) 来了解更多使用`Fu Doc`的案例。
