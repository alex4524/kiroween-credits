# kiroween-credits

一个给 AI 助手用的技能:带零基础的人走完 Kiroween 2026 黑客松领 Kiro 额度的全流程(注册 Kiro、注册 Devpost、报名、填额度表、身份核验)。

## 安装

把 `SKILL.md` 放进你助手的技能目录,目录名用 `kiroween-credits`。例如:

```bash
mkdir -p ~/.kiro/skills/kiroween-credits
curl -fsSL https://raw.githubusercontent.com/alex4524/kiroween-credits/main/SKILL.md -o ~/.kiro/skills/kiroween-credits/SKILL.md
```

装好后对助手说:「帮我领 Kiroween 的 Kiro 额度」。

## 说明

- 流程和网址按 2026-11-13 实测写成,以官方页面为准:https://kiroween.devpost.com/
- 中国身份证能否通过身份核验,未验证。
- 本技能不含任何个人信息。证件照和人脸只在核验页面里拍,不发给助手。
