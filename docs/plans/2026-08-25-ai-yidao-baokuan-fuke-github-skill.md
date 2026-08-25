# AI 一刀之爆款复刻 GitHub Skill 实施计划

- [x] 建立独立 GitHub-ready 项目骨架，不覆盖旧版 skill
- [x] 编写 `skills/ai-yidao-baokuan-fuke/SKILL.md`
- [x] 编写 `agents/openai.yaml`
- [x] 补齐 README、版本、许可和忽略规则
- [x] 运行 skill 校验并检查可安装路径

验证记录：

- 官方 `quick_validate.py` 在当前 Python 环境中因缺少 `PyYAML` 无法启动。
- 已按 `quick_validate.py` 的检查逻辑用 Ruby 完成等价校验：frontmatter、name、description、允许字段、TODO 占位均通过。
- 已初始化独立 Git 仓库并完成首提交：`e009fc1`。
