Life
====
这是我长期以来一直想构建的东西。它是我生命中重要事件的**时间线**，以一种我脑海中总是想象的方式呈现。曾经有个叫做[**Lifepath.me**](http://dcurt.is/facebook-timelines-and-lifepath-me-4)的东西，但现在它已经消失了。Facebook的时间线呢？呃。
所以，就是这样。来看看 [cheeaun的Life](http://cheeaun.life/)。

特性
--------
- 极其简单
- 没有花哨的格式
- 没有复杂的设置
- 没有花哨的效果
- 灵活的日期时间，因为有时你并不记得一个事件的确切日期

如何贡献
-----------------
1. Fork 这个项目。
2. 编写代码。
3. 提交 pull 请求。

如何搭建你自己的 *Life*
----------------------------
1. Fork 这个项目。
2. `git checkout -b gh-pages`（或者任何你喜欢的分支名称）
3. 复制一份 `life.example.md`，将其重命名为 `life.md`。
4. 在 `life.md` 中添加你的生活事件。
5. 在本地服务器上预览。使用 [`python -m http.server`](https://docs.python.org/3/library/http.server.html) 或者 [`http-server`](https://github.com/nodeapps/http-server)。
6. 提交 `life.md`（不在 `master` 分支中）。
7. `git push origin gh-pages -f` 并发布到 [GitHub Pages](http://pages.github.com/)。
8. 在你的 GitHub 仓库描述中更新网站链接。
9. 告诉世界关于你的Life。
10. 将你的Life添加到 [Life集合](https://github.com/cheeaun/life/wiki/Lives) 页面。

如何升级你的 *Life*
--------------------------
1. `git checkout master`
2. `git remote add cheeaun https://github.com/cheeaun/life.git`
3. `git fetch cheeaun` 然后 `git merge cheeaun/master` 以升级到最新的Life。
4. `git checkout gh-pages` 然后 `git merge master` 以将更改同步回 GitHub Pages。
[了解更多](https://help.github.com/articles/fork-a-repo)。
对于那些 fork 了早期版本Life的用户，以下是我推荐的步骤（需要一些 Git 技能）：
1. 备份你的 `life.md`。
2. 将你的 fork 硬重置到这个仓库的 `master` 分支。
3. 清理你的 `gh-pages`。
4. 在那里重新提交你的 `life.md`。
5. 确保你的 `master` 分支未被修改，以便未来的更新可以正常工作。

如何配置你的 *Life*
----------------------------
1. 复制一份 `config.example.json`，将其重命名为 `config.json`。
2. 只在 `gh-pages` 分支中提交它。
配置项：
- `customStylesheetURL` - (*字符串*, 默认为 `null`) 自定义样式表的路径，适用于那些不喜欢默认 *主题* 的人。
- `yearLength` - (*数字*, 默认为 `120`) 年份格子的宽度，以像素为单位。
- `hideAge` - (*布尔值*, 默认为 `false`) 选择隐藏年份轴上的年龄。

日期时间 "语法"
-----------------
- `2000` - 发生在那一年的事件
- `01/2000` - 发生在那个月/年的事件
- `01/01/2000` - 精确发生在那一天/月/年的事件
- `2001-2005`, `10/2001-02/03/2005` - 在两个日期之间发生的事件
- `~2005` - 大约在那一年发生的事件
- `2005-~` - 从那一年开始并且持续到现在的事件。

其他人的Life
--------------------
这里有一份来自那些已经 fork 了Life的用户的[Life汇编](https://github.com/cheeaun/life/wiki/Lives)。

许可
-------
[MIT](http://cheeaun.mit-license.org/)
