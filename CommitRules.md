#代码提交规范

##编写文档

所有功能点尽量提交配套文档，文档建议满足以下要求。

说清楚问题的几个方面：what（是什么），why（为什么），how（怎么做），可根据问题的特性有所侧重。
how 部分包含详尽完整的操作步骤，必要时附上 **可运行** 的范例代码。
提供必要的链接，如术语解释和参考文档等。

##提交代码

###提交Merge Request

创建分支修改代码后提交MR合并到主干分支

由于谁也无法保证过了多久之后还记得多少，为了后期回溯历史的方便，提交 MR 时可提供以下信息。

1. 需求点
2. 升级原因（可以简要描述下为什么要处理）
3. 关注点（针对用户而言，一般是不兼容更新等，需要额外提示）

## 代码风格（待执行）

你的代码风格必须通过 eslint，你可以运行 $ npm run lint 本地测试。

##Commit提交规范

根据以下规范提交 commit， 这样 history 看起来更加清晰，还可以自动生成 changelog。

```
<type>(<scope>): <subject>
<BLANK LINE>
<body>
<BLANK LINE>
<footer>
```

###1. type

提交 commit 的类型，包括以下几种

* feat: 新功能
* fix: 修复问题
* docs: 修改文档
* style: 修改代码格式，不影响代码逻辑
* refactor: 重构代码，理论上不影响现有功能
* perf: 提升性能
* test: 增加修改测试用例
* chore: 修改工具相关（包括但不限于文档、代码生成等）
* deps: 升级依赖

###2.scope

修改文件的范围（包括但不限于 doc, middleware, core, config, plugin）

###3.subject

用一句话清楚的描述这次提交做了什么

###4.body

补充 subject，适当增加原因、目的等相关因素，也可不写。

###5.footer

当有非兼容修改(Breaking Change)时必须在这里描述清楚

###example
```
refactor(kkl.js): [BREAKING_CHANGE] 公共侧栏修改
原有的XXX不合理，会导致XXXXX
为配合XX需求，增加XX功能
BREAKING CHANGE:
  Dom结构变动，需要同步kkl.css v2.X版本
```