# AI 一刀之爆款复刻

一个给 Codex 使用的流程型 skill，用来把一篇对标短视频口播文案拆成逐句结构，再按用户的行业、客户、产品和选题方向复刻成新文案。

它的核心纪律是：

> 对标有，我们才有；对标没有，我们就没有。

因此，对标没有 CTA，就不生成 CTA；对标没有评论、私信、领资料、下单指令，就不额外添加这些动作。

## 安装

在 Codex 里让对方输入：

```text
请从 GitHub 安装这个 skill：
https://github.com/<your-github-name>/ai-yidao-baokuan-fuke/tree/main/skills/ai-yidao-baokuan-fuke
```

或：

```text
安装 <your-github-name>/ai-yidao-baokuan-fuke 里的 skills/ai-yidao-baokuan-fuke
```

安装后下一轮对话可用：

```text
用 $ai-yidao-baokuan-fuke 帮我复刻这篇口播
```

## 使用流程

1. 用户先发送对标口播文案。
2. 首次使用时，skill 询问行业、客户、产品；同一对话里后续不重复问。
3. skill 拆解对标文案的模块、句式、情绪节奏和 CTA 状态。
4. 用户输入本次选题方向。
5. skill 输出左右两列逐句对照，让用户确认或修改。
6. 用户确认后，skill 再输出提词器版。

## 项目结构

```text
ai-yidao-baokuan-fuke/
  skills/
    ai-yidao-baokuan-fuke/
      SKILL.md
      agents/
        openai.yaml
```

## 校验

```bash
python3 ~/.codex/skills/.system/skill-creator/scripts/quick_validate.py skills/ai-yidao-baokuan-fuke
```

## 版本

当前版本：`0.1.0`
