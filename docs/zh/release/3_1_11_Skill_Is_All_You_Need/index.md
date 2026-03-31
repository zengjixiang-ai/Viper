# 3.1.11 Skill is all you need

## 优化

- 更新MCP服务器,压缩docstring,占用更少上下文,修复BUG [MCP服务器](../../guide/mcpserver.md)

## 新功能

- 新增 [Claude Code Plugin](../../training/use_viper_with_skills/),通过Claude Code插件市场安装后,可以在Claude Code中使用Viper的MCP Tools,实现无缝衔接的AI辅助红队操作.

## 开发者笔记

Claude 提出的 MCP 和 Skill 的两个核心概念,在Viper中得到了很好的实现.通过MCP服务器,我们将Viper的功能以API的形式暴露出来,而Skill则是对这些功能的封装和组合,使得用户可以更高效地使用这些功能.
使用Viper进行内网渗透,或者说使用任何工具进行内网渗透,都是有"套路"的,但是这个"套路"更多的是在思维层面上的,而不是在具体的操作步骤上.
每个内网环境都是独特的,需要根据实际情况进行调整和适应. 而Viper的Skill则是对这些"套路"的一种抽象和封装,使得用户可以更高效地使用这些"套路",而不需要关心具体的操作细节.
而所有的这些动作动作基本都需要 Session 这个桥梁在内网主机中执行,所以将 Session 的功能都通过MCP开放出来让 skill 可以调用,是 AI 驱动内网渗透的基础.
未来我们还会继续增加更多的 MCP API,让 Skill 可以调用更多的功能,从而实现更加强大和智能的内网渗透能力.
