# 3.1.11 Skill Is All You Need

## Improvements

- Updated the [MCP Server](../../guide/mcpserver.md), compressed docstrings to use less context, and fixed bugs.

## New Features

- Added the [Claude Code Plugin](../../training/use_viper_with_skills/). After installing it from the Claude Code plugin marketplace, you can use Viper MCP tools directly inside Claude Code for seamless AI-assisted red team operations.

## Developer Notes

The two core concepts introduced by Claude — MCP and Skill — are implemented very well in Viper. Through the MCP server, we expose Viper capabilities as APIs, while Skills package and combine those capabilities so users can work with them more efficiently.

Using Viper for internal network penetration testing — or using any tool for that purpose — always involves certain common patterns. But those patterns mainly exist at the level of thinking and strategy, rather than as fixed operational steps.

Every internal environment is unique, so you need to adapt based on the actual situation. Viper Skills abstract and package these patterns so users can apply them more efficiently without focusing on low-level operational details.

Nearly all of these actions require a Session as the bridge for execution on internal hosts, so exposing Session capabilities through MCP for Skills to call is the foundation of AI-driven internal network penetration testing.

In the future, we will continue adding more MCP APIs so Skills can call more capabilities and deliver stronger, smarter internal network penetration testing workflows.
