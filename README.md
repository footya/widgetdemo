# widget开发规范 #

> 组件开发约定,只约定了目录结构和变量命名，在保证可读的情况下，尽量不干涉大家的开发习惯

## 命名约定 ##
- 文件和目录名只能包含 [a-z\d-]，并以英文字母开头
- 首选合适的英文单词且全部小写
- 类名驼峰，并且首字母要大写 CamelName
- 常量全大写 UPPERCASE_WORD
- 变量驼峰 varName

## 目录结构示例 ##
>seed 目录为按如下规则建立的一个种子项目,可以直接copy一份放在当前文件夹内来开发自己的widget,lib 为大家可能用到的一些辅助内容如jquery等

<pre>
widgetname
  -- img                      存放组件用到的 img 等文件
      -- imgname.png
  -- css                      存放 js, css 文件
      -- cssname.css
  -- js 
      -- jsname.js
  -- demo                     演示页面
      -- demo.html
  -- tests                    单元测试[可选]
       -- jsname-test.js
  -- history.md               更新说明
  -- readme.md                组件总体说明,用来描述组件的功能，和提供的api
  -- package.json             模块元信息，描述作者等相关信息
</pre>

## 文档约定 ##

###readme.md###
>每个组件必须有 readme.md 文件，用来描述组件的基本情况

<pre>
# 模块名称
>该模块的概要介绍。
## 使用说明 ##
如何使用该模块，可以根据组件的具体特征，合理组织。
## API ##
需要提供 API 说明，属性、方法、事件等。
</pre>
###history.md###
>记录组件的变更。

<pre>
### 1.1.0

* [fixed] 修复了 XXX 问题
* [fixed] 修复了 YYY 问题
* [new] 增加了 ZZZ 功能
* [improved] 优化了 BBB 代码

### 1.0.0

* [new] 第一个发布版本
</pre>

###package.json###

<pre>
{
  "name": "widgetname", //模块名称
  "version": "0.1.0", //版本信息
  "description": "angularjs,requirejs", //描述
  "main": "app.js", //入口文件
  "author": "name", //作者
  "keywords": [ //关键词,便于后期做检索
    "suggest+jquery"
  ]
}
</pre>


