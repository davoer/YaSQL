# AuditSQL数据库审核和执行平台

AuditSQL是web版本的MySQL数据库审核平台，旨在降低DBA的运维成本

使用上的问题，可以提ISSUES或者加QQ群。

年底太忙，更新慢，谢谢理解！

## 组件
- Python 3.6
- Django 2.0
- Rest-framework
- AdminLTE
  
## 功能
- 自定义环境
  - 可以根据公司业务需求，定义多个环境，比如：测试环境、预发布环境、生产环境等
- 工单类型
  - 支持DML、DDL、运维工单、数据导出工单(csv,xlsx)
  - 支持钩子、上线版本等功能
- 数据字典
  - 支持生成指定库的数据字典功能
- SOAR支持
  - 集成了小米的soar
- 语法规则
  - 提供SQL语法审核（由Inception提供）
  - 支持格式化、高亮、注释、补全等功能
- 审核流程
  - 工单审核、执行、复核流程化
  - 支持单人、多人审核和复核功能
  - 工单历史
- 执行功能
  - DDL语句支持gh-ost改表
  - DML语句实现事务级别的执行保证
  - 一个工单内最大支持1000条SQL语句，支持一键「全部执行」
  - 自动生成DML回滚语句 
- 进度展示
  - 前台实时显示DML、DDL、数据导出的进度（websocket）
- 推送通知
  - 支持钉钉机器人
  - 支持邮件推送
  - 可同时支持启用钉钉和邮件
- SQL查询
  - MySQL查询功能
  - 支持列级授权
  - 通过黑名单、权限、业务分组进行灵活控制
  - 支持查看表结构、索引、元信息，支持补全、格式、limit等功能
- Xterm[不在支持]
- 数据导出
  - 支持xlsx，csv格式，支持海量数据的优化导出
- 其他功能
   - 支持自定义角色
   - 支持LDAP授权登陆功能
   - 支持本地自建用户，本地密码修改
   - 支持修改头像


## 效果展示
https://github.com/lazzyfu/AuditSQL/wiki/show

## 文档（使用和安装）
https://github.com/lazzyfu/AuditSQL/wiki


