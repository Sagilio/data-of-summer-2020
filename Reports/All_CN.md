# 第一周（July 1-July 7）

## 本周总结：
1. 创建Casbin.AspNetCore项目，并实现核心设计与功能。
2. 优化Casbin.NET的单元测试的工作流程，解决[issue #47](https://github.com/casbin/Casbin.NET/issues/47)。
3. 使用dotnet-format实现代码风格的自动控制。

## Issue 或 Pull Request：
1. Issue [#47](https://github.com/casbin/Casbin.NET/issues/47) - PR [#48](https://github.com/casbin/Casbin.NET/pull/48) - Fix the IO exception when sometimes running unit tests. (Changes +248 -86) (Status - closed)
2. Issue [#49](https://github.com/casbin/Casbin.NET/issues/49) - PR [#50](https://github.com/casbin/Casbin.NET/pull/50) - Use dotnet-format to automatically format the code. (Changes +388 -99) (Status - reviewing)
3. PR [#1](https://github.com/casbin-net/Casbin.AspNetCore/pull/1) - Implement the core feature and the unit test of it. (Changes +897 -5) (Status - closed)

## 下周计划：
1. 按照计划，初步实现casbin-sam的项目整体结构的详细设计。
2. 继续开发Casbin.AspNetCore，创建项目并自动更进进度，配置CI。
3. 增加Casbin.NET对于Model和Encofer的构造方式或逻辑，以提供更灵活的管理，