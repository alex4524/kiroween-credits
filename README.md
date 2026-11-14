# kiroween-credits

一个给 AI 助手用的技能:带零基础的人走完 Kiroween 2026 黑客松领 Kiro 额度的全流程(注册 Kiro、注册 Devpost、报名、填额度表、身份核验)。

## 一条命令安装(推荐,通用)

```bash
npx skills add alex4524/kiroween-credits
```

按提示选你用的工具(Claude Code、Codex、Kiro 等),它会装到对应目录。需要先装 Node.js。
我只测过「列出技能」,能识别到 kiroween-credits。实际装进各个工具,未验证。

装完对助手说:「帮我领 Kiroween 的 Kiro 额度」。

## 手动安装:按工具选一种

先下载文件:[SKILL.md](https://raw.githubusercontent.com/alex4524/kiroween-credits/main/SKILL.md)

| 工具 | 放到哪个目录 |
|---|---|
| Claude Code | `~/.claude/skills/kiroween-credits/SKILL.md` |
| Codex | `~/.agents/skills/kiroween-credits/SKILL.md`(也有文章写 `~/.codex/skills`,不生效就换) |
| Kiro | `~/.kiro/skills/kiroween-credits/SKILL.md` |

例(Claude Code):

```bash
mkdir -p ~/.claude/skills/kiroween-credits
curl -fsSL https://raw.githubusercontent.com/alex4524/kiroween-credits/main/SKILL.md -o ~/.claude/skills/kiroween-credits/SKILL.md
```

## DeepSeek 或其他没有技能功能的聊天工具

1. 打开上面的 SKILL.md,全选复制。
2. 新开对话,粘贴进去,最前面加一句:
   「你是教练。请严格按下面的流程,一步一步带我领 Kiroween 的 Kiro 额度。每次只给一步,我说"好了"再给下一步。」
3. 每做完一步,告诉它「好了」。

## 说明

- 流程和网址按 2026-11-13 实测写成,以官方页面为准:https://kiroween.devpost.com/
- 中国身份证能否通过身份核验,未验证。
- 技能不含任何个人信息。证件照和人脸只在核验页面里拍,不发给 AI。
