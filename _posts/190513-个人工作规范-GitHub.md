---
layout: post
title: 个人工作规范-GitHub
categories: [规范, GitHub]
description: 主要强调一些 GitHub 使用上的规范，提高使用效率，养成良好编程习惯
keywords: 规范, GitHub
---

# Git Commit Message 提交规范

简单搜了一下，已经有比较规范化的工具 [commitizen](https://github.com/commitizen/cz-cli)，考虑到个人维护的项目比较小，暂时还用不上这样的“牛刀”。

业界常用的规范是 [Angular团队的规范](https://github.com/angular/angular.js/blob/master/DEVELOPERS.md#-git-commit-guidelines)，然后主要参考了 [优雅的提交你的 Git Commit Message][1] 和 [git commit 代码提交规范][2]，感觉对于个人项目来说还是有点点复杂，准备只采用标题行中的 type 和 subject ，所以自己的提交规范如下：

标题行：主要描写修改类型和内容

```
<type>: <subject>
```

### type 类型：
- feat : 新功能
- fix : 修复bug
- docs : 文档改变
- style : 代码格式改变
- refactor : 某个已有功能重构
- perf : 性能优化
- test : 增加测试
- chore : 构建过程或辅助工具的变动
- build : 改变了build工具 如 grunt换成了 npm
- revert : 撤销上一次的 commit

### subject 描述：
[优雅的提交你的 Git Commit Message][1] 说是 subject 是概述，建议符合 [50/72 formatting][3]，即：第一行少于或等于 50 个字符；然后空行；一行超过 72 个字符就需要换行。

### 最终规范
考虑到上面说的情况，准备直接采用动宾格式，后面三个 type 一般的小项目应该也用不到，最后 Commit Message 模板如下，`()` 内的文字可选可换：

- feat: 添加xxx(功能)
- fix: 修复xxx(问题)
- docs: 撰写xxx(文档)
- style: 规范xxx(格式)
- refactor: 重构xxx(功能)
- perf: 优化xxx(性能)
- test: 测试xxx(模块)

[1]: https://juejin.im/post/5afc5242f265da0b7f44bee4
[2]: https://segmentfault.com/a/1190000017205604
[3]: https://stackoverflow.com/questions/2290016/git-commit-messages-50-72-formatting


