# kiroween-credits

一个给 AI 助手用的技能:带零基础的人走完 Kiroween 2026 黑客松领 Kiro 额度的全流程(注册 Kiro、注册 Devpost、报名、填额度表、身份核验)。

## 一条命令安装(推荐,通用)

先装好 Node.js(自带 npx)。然后在终端运行:

```bash
npx -y skills add https://github.com/alex4524/kiroween-credits -g -y
```

- `npx` 会自动下载安装工具 `skills`,不用先 `npm install`。
- `-g` 装到你的用户目录,所有项目都能用。不加 `-g` 只装到当前文件夹。
- 不加 `-y` 时,它会让你选要装给哪个工具(Claude Code、Codex 等)。
- 想指定工具:加 `-a claude-code` 或 `-a codex`。

装完对助手说:「帮我领 Kiroween 的 Kiro 额度」。

实测(2026-11-14,macOS):完整链接和 `alex4524/kiroween-credits` 简写都能装,技能文件落到了 `.claude/skills` 和 `.agents/skills`。在真实的 Claude Code、Codex 里能否被调用,未验证。

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
- 中国身份证可以通过身份核验(2026-11-16 本人实测)。
- 技能不含任何个人信息。证件照和人脸只在核验页面里拍,不发给 AI。
