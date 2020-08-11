# 第一周（July 1 - July 7）

## 说明
第一周按照正常的计划，正式开始进行Casbin.AspNetCore的项目开发，由于其是Casbin.Sam需要依赖的上游项目，因此一些设计需要保证两者的使用上的基本一致。

## 本周总结：
1. 创建Casbin.AspNetCore项目，并实现核心设计与功能。
2. 优化Casbin.NET的单元测试的工作流程，解决[issue #47](https://github.com/casbin/Casbin.NET/issues/47)。
3. 使用dotnet-format实现代码风格的自动控制。

## 贡献：
1. Issue [#47](https://github.com/casbin/Casbin.NET/issues/47) - PR [#48](https://github.com/casbin/Casbin.NET/pull/48) - Fix the IO exception when sometimes running unit tests. (Changes +248 -86) (Status - Closed)
2. Issue [#49](https://github.com/casbin/Casbin.NET/issues/49) - PR [#50](https://github.com/casbin/Casbin.NET/pull/50) - Use dotnet-format to automatically format the code. (Changes +388 -99) (Status - Reviewing)
3. PR [#1](https://github.com/casbin-net/Casbin.AspNetCore/pull/1) - Implement the core feature and the unit test of it. (Changes +897 -5) (Status - Closed)

## 下周计划：
1. 按照计划，初步实现Casbin Sam的项目整体结构的详细设计。
2. 继续开发Casbin.AspNetCore，创建项目并自动更进进度，配置CI。
3. 增加Casbin.NET对于Model和Encofer的构造方式或逻辑，以提供更灵活的管理，

# 第二周（July 8 - July 14）

## 说明
第二周的后期和第三周的前半时间由于学校的安排的实习，将部分工作量略微向后推迟，预计在第四周重回正轨。

## 本周总结：
1. 开始进行对Casbin Sam的项目整体结构的设计，目前的最新进度体现在fork库中的master分支。
2. 梳理Casbin.NET需要对其他项目的支持所作出的更改，目前已经通过Issue提出
3. 由于Casbin.AspNetCore的结构需要与Casbin.Sam.AspNetCore保证一致，所以发布时间放缓至确认Casbin.Sam的大致方案之后。

## 贡献：
1. Issue [#51](https://github.com/casbin/Casbin.NET/issues/51) Develop Casbin.AspNetCore to help use Casbin in ASP NET Core (Status - Only open issue)
2. Issue [#52](https://github.com/casbin/Casbin.NET/issues/52) Change the workflow of creating a model (Status - Only open issue)

## 下周计划：
1. 完成对Casbin Sam的项目整体结构详细设计并提交PR。
2. 跟进Casbin.AspNetCore的进度，做好发布的准备。
3. 跟进并完善Casbin.NET的代码，将更多的想法通过Issue体现，具体方案将尽可能地遵循Go的实现。

# 第三周（July 15 - July 22）

## 说明
本周的前半期间在学校的实习阶段，在本周后三天重新开始恢复正常的推进速度。

## 本周总结：
1. 提交Casbin Sam的项目整体结构的设计并进入Review阶段。
2. 增加Casbin.AspNetCore的CI支持，并准备MyGet账户。
3. 完善Casbin.NET的代码。

## 贡献：
1. Issue [#56](https://github.com/casbin/Casbin.NET/pull/53) Change PermConstants to static and fix some typos. (Changes +36 -36) (Status - Reviewing)

## 下周计划：
1. 完善Casbin.Sam项目的设计。
2. 完善Casbin.AspNetCore的项目。

# 第四周（July 23 - July 30）

## 本周总结：
1. 提出并处理了有关抽象层实现 (接口实现) 的方案。
2. 提出了有关 API 实现结构的更改。
3. 为Casbin.NET增加了Benchmark项目。

## 贡献：
1. Issue [#56](https://github.com/casbin/Casbin.NET/pull/56) Change the way of integrating RBAC API and Management API to a one Enforcer (Status - Opened)
2. Reivew pull request [#55](https://github.com/casbin/Casbin.NET/pull/55) Provide interface of enforcer to make testing easier (Status - Merged)
3. PR [#57](https://github.com/casbin/Casbin.NET/pull/57) - Format the interface code and add an obsolete attribute on it. (Changes +101 -140) (Status - Merged)
4. Issue [#54](https://github.com/casbin/Casbin.NET/issues/54) - PR [#58](https://github.com/casbin/Casbin.NET/pull/58) - Add benchmark project to monitor the performance change. (Changes +750 -25) (Status - Closed)

## 下周计划：
1. 配置Casbin.AspNetCore的项目的CI与构建发布的支持。
2. 在CI自动执行Casbin.NET的Benchmark项目。
3. 完善Casbin.AspNetCore的基础功能。


# 第五周（July 31 - August 6）

## 本周总结：
1. 解决了filter方法的可能会清空数据的问题。
2. 增加KeyMatch4函数的实现。
3. 使Benchmark项目在CI自动执行。
4. 配置Casbin.AspNetCore的项目的CI与构建版本发布。
5. 完善Casbin.AspNetCore项目的基础功能。

## 贡献：
1. Issue [#59](https://github.com/casbin/Casbin.NET/issues/59) - PR [#60](https://github.com/casbin/Casbin.NET/pull/60) - Change the filter workflow at model . (Changes +45 -31) (Status - Closed)
2. Issue [#61](https://github.com/casbin/Casbin.NET/issues/61) - PR [#62](https://github.com/casbin/Casbin.NET/pull/62) - Add KeyMatch4 function support. (Changes +150 -10) (Status - Closed)
3. PR [#57](https://github.com/casbin/Casbin.NET/pull/57) - Improve KeyMatch4 function performence. (Changes +34 -7) (Status - Merged)
4. Issue [#64](https://github.com/casbin/Casbin.NET/issues/64) - PR [#67](https://github.com/casbin/Casbin.NET/pull/67) - Run benchmark on Github Actions. (Changes +60 -15) (Status - Closed)
5. Issue [#65](https://github.com/casbin/Casbin.NET/issues/65) - PR [#68](https://github.com/casbin/Casbin.NET/pull/68) - Auto release github packages on Github Actions. (Changes +45 -4) (Status - Closed)
6. (9 Commit) From [Change test project name](https://github.com/casbin-net/Casbin.AspNetCore/commit/f858c4daa64a96dd443ecb0012bb624403654b11) to [Remove retry to push github package at build github action](https://github.com/casbin-net/Casbin.AspNetCore/commit/ec34b278b8d95a42c03af08149d83ced35d73151).

## 下周计划：
1. 提供Casbin.AspNetCore的项目的集成，标注和中间实现。
2. 完善Casbin Sam的Management项目的基础设计。


# 第六周（August 7 - August 14）

## 本周总结：
1. 完善Casbin.AspNetCore的中间件和标注的实现，并增加了对应的单元测试，此时Casbin.AspNetCore已达到测试发布要求。
2. 增加Casbin.NET的watcher的单元测试。
3. 开发Casbin.Sam的Management项目。

## 贡献：
1. Issue [#71](https://github.com/casbin/Casbin.NET/issues/71) - PR [#72](https://github.com/casbin/Casbin.NET/pull/72) - Add watcher unit test. (Changes +60 -15) (Status - Closed)
2. Issue [#3](https://github.com/casbin-net/Casbin.AspNetCore/issues/3) - PR [#9](https://github.com/casbin-net/Casbin.AspNetCore/pull/9) - Provide casbin authorization middleware. (Changes +798 -326) (Status - Closed) (6 Commit)
3. PR [#1](https://github.com/casbin-net/casbin-sam/pull/1) - Initial the core and management design. (Changes +661 -12) (Status - Closed)
4. (5 Commit) From [Add authentication schemes support](https://github.com/casbin-net/Casbin.AspNetCore/commit/d5d753e14551551ad5012cab27b7f24227b8f945) to [Change try add CasbinAuthorizationHandler to add](https://github.com/casbin-net/Casbin.AspNetCore/commit/02bc0fb12e173c652ca1ab8013e5514c03f44252).

## 下周计划：
1. 为Casbin.AspNetCore编写README和介绍文章。
2. 继续开发Casbin.Sam的Management项目。