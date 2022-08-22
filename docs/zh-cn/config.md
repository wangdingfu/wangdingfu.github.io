# 全局参数配置

> 你可以进入`Fu Doc`的配置页面(`IDEA-->Settings-->Other Settings-->Fu Doc`)配置一些自定义内容

![img.png](../img/img_70.png)

> 可以参考下方配置示例
```json
{
  "setting_customer_value": [
    {
      "alias": "pms",
      "value": "com.fuge.example.enumtype.Permission#value",
      "type": "annotation"
    }
  ],
  "setting_valid": {
    "message": {
      "type": "replace",
      "value": "不能为空,not null"
    }
  },
  "setting_enum": {
    "code": "code,index",
    "msg": "msg,desc,view"
  }
}

```

## setting_customer_value
```json
{
  "setting_customer_value": [
    {
      "alias": "pms",
      "value": "com.fuge.example.enumtype.Permission#value",
      "type": "annotation"
    }
  ]
}
```
> 用于一些需要在接口文档中渲染自定义数据的场景 例如需要将接口上权限注解的权限key渲染到接口文档模板上
- 类型：`array`
- 默认值：`null`

###### alias
> 给自定义数据起一个别名 在接口文档模板中可通过`fudoc.alias`的方式获取到自定义数据
- 类型：`String`
- 默认值：`null`

###### type
> 指定当前配置项从哪里取数据 目前默认从枚举中取数据
- 类型：`String`
- 默认值：`annotation`

###### value
> 指定当前配置项取数据的途径 当`type=annotation`时 `value`的格式应当是`注解全路径#属性名`
- 类型：`String`
- 默认值：`null`

---

## setting_valid
```json
{
  "setting_valid": {
    "message": {
      "type": "replace",
      "value": "不能为空,not null"
    }
  }
}
```
> 配置一些跟校验注解相关的配置 例如从校验注解中将注解`message`中的提示信息解析成字段说明
- 类型：`json`
- 默认值：`null`

#### message
> 配置将校验注解的`message`属性的提示信息解析成字段说明
- 类型：`json`
- 默认值：`null`

###### type
> 指定以哪种方式读取`message`的提示信息 默认替换指定内容方式
- 类型：`String`
- 默认值：`replace`

###### value
> 要替换的内容或则正则表达式
- 类型：`String`
- 默认值：`null`

---

## setting_enum
```json
{
  "setting_enum": {
    "code": "code,index",
    "msg": "msg,desc,view"
  }
}
```
> 读取枚举内容的相关配置
- 类型：`json`
- 默认值：`null`

###### code
> 指定将枚举中的哪个属性做为字典的`key` 支持以`,`号分隔填写多个属性名称 按照顺序优先级读取 如果没有命中 则会按照类型优先级`int>Integer>Short>Long>String`和属性在枚举中的顺序组合的优先级读取优先级最高的属性作为字典`key`
- 类型：`String`
- 默认值：`code,index`

###### value
> 指定将枚举中的哪个属性做为字典的`value` 支持以`,`号分隔填写多个属性名称 按照顺序优先级读取 如果没有命中 则会读取属性类型为`String`和属性在枚举中的顺序组合的优先级读取优先级最高的属性作为字典`value`
- 类型：`String`
- 默认值：`msg,message,desc,view`