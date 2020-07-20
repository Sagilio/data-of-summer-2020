# 第一周（July 1-July 7）

## 说明
第一周按照正常的计划，正式开始进行Casbin.AspNetCore的项目开发，由于其是Casbin.Sam需要依赖的上游项目，因此一些设计需要保证两者的使用上的基本一致。

## 本周总结：
1. 创建Casbin.AspNetCore项目，并实现核心设计与功能。
2. 优化Casbin.NET的单元测试的工作流程，解决[issue #47](https://github.com/casbin/Casbin.NET/issues/47)。
3. 使用dotnet-format实现代码风格的自动控制。

## Issue 或 Pull Request：
1. Issue [#47](https://github.com/casbin/Casbin.NET/issues/47) - PR [#48](https://github.com/casbin/Casbin.NET/pull/48) - Fix the IO exception when sometimes running unit tests. (Changes +248 -86) (Status - Closed)
2. Issue [#49](https://github.com/casbin/Casbin.NET/issues/49) - PR [#50](https://github.com/casbin/Casbin.NET/pull/50) - Use dotnet-format to automatically format the code. (Changes +388 -99) (Status - Reviewing)
3. PR [#1](https://github.com/casbin-net/Casbin.AspNetCore/pull/1) - Implement the core feature and the unit test of it. (Changes +897 -5) (Status - Closed)

## 下周计划：
1. 按照计划，初步实现Casbin Sam的项目整体结构的详细设计。
2. 继续开发Casbin.AspNetCore，创建项目并自动更进进度，配置CI。
3. 增加Casbin.NET对于Model和Encofer的构造方式或逻辑，以提供更灵活的管理，

# 第二周（July 8-July 14）

## 说明
第二周的后期和第三周的前半时间由于学校的安排的实习，将部分工作量略微向后推迟，预计在第四周重回正轨。

## 本周总结：
1. 开始进行对Casbin Sam的项目整体结构的设计，目前的最新进度体现在fork库中的master分支。
2. 梳理Casbin.NET需要对其他项目的支持所作出的更改，目前已经通过Issue提出
3. 由于Casbin.AspNetCore的结构需要与Casbin.Sam.AspNetCore保证一致，所以发布时间放缓至确认Casbin.Sam的大致方案之后。

## Issue 或 Pull Request：
1. Issue [#51](https://github.com/casbin/Casbin.NET/issues/51) Develop Casbin.AspNetCore to help use Casbin in ASP NET Core (Status - Only open issue)
2. Issue [#52](https://github.com/casbin/Casbin.NET/issues/52) Change the workflow of creating a model (Status - Only open issue)

## 下周计划：
1. 完成对Casbin Sam的项目整体结构详细设计并提交PR。
2. 跟进Casbin.AspNetCore的进度，做好发布的准备。
3. 跟进并完善Casbin.NET的代码，讲更多的想法通过Issue体现，具体方案将尽可能地遵循Go的实现。

# 第三周（July 15-July 21）

## 说明
本周的前半期间在学校的实习阶段，最后三天重新开始恢复正常的推进速度。

## 本周总结：
1. 提交Casbin Sam的项目整体结构的设计并进入Review阶段。
2. 增加Casbin.AspNetCore的CI支持，并准备MyGet账户。
3. 完善Casbin.NET的代码。

## Issue 或 Pull Request：
1. PR [#53](https://github.com/casbin/Casbin.NET/pull/53) Change PermConstants to static and fix some typos. (Changes +36 -36) (Status - Reviewing)

## 下周计划：
1. 落实Casbin.Sam项目整体设计，正式进入开发阶段。
2. 完善Casbin.AspNetCore的Sample，文档并发布第一个预览版。