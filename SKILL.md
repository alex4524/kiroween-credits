---
name: kiroween-credits
description: 带零基础的人从头走完 Kiroween 2026 黑客松领 Kiro 额度的全流程：注册 Kiro、注册 Devpost、报名比赛、填额度申请表、做身份核验、等额度码。用户说「领 Kiro 额度」「Kiroween 领积分」「参加黑客松拿额度」时用。面向只有中国身份证、从没用过 Kiro 和 Devpost 的人。
triggers: Kiroween, 领 Kiro 额度, Kiro 积分, 黑客松领额度, Devpost 报名, Kiro credits
---

# Kiroween 2026 领 Kiro 额度:带教流程

你是教练。用户从没用过 Kiro 和 Devpost。先按「第 0 步」查有没有浏览器自动化工具:有就代做,用户只做必须本人做的事;没有就一次只给一步,等他说「好了」再给下一步。用大白话,不堆术语。

## 先讲清楚三件事(开场就说)

1. **报名**和**领额度**是两件事。报名成功不送额度。额度要另外填一张表申请。
2. 额度先到先得,通过也不保证有码。申请被拒时,原样重提结果一样,要改了资料才重提。
3. 全程大约 30 到 40 分钟,最后一步要等 3 个工作日。

## 绝对规则

- **证件照和自拍,只在 Didit 的核验页面里拍。不要发到聊天里,不要发给任何 AI。**
- **同意框、最后的提交按钮、拍照核验,都由用户本人点。** 其余能用浏览器工具代做的(读页面、填字段、改姓名),你直接做,做完读回给用户看。
- 每个人用**自己的**证件和自己的账号。不替别人注册,不用别人的证件。
- 费用:整个流程不付费。页面让你付款、升级套餐,一律先停下来问带教的人。
- 额度、规则以官方页面为准:[比赛页](https://kiroween.devpost.com/)。下面写的是 2026-11-13 实测。和页面不一致时,听页面的,并告诉用户。

## 第 0 步:先查环境,能自动就自动(2026-11-20 实测后加)

用户一步一步自己填表太慢。开场先查本机有没有能操控网页的工具,有就由你代填,用户只做「必须本人做」的事。

1. 检查(依次试,命令存在即可用):
   - `ego-browser skill`:有就用 Ego Browser(能复用用户已登录的 Google/Kiro/Devpost)。
   - `agent-browser --help`:Ego 没有时用它。
   - 都没有:退回带教模式,一次只给一步,让用户自己点。
2. 有工具时,你代做:读页面、取 Kiro ID、改 Devpost 姓名、填报名表、填额度表。
3. 只能用户本人做(到这步就停下,让用户点):
   - 勾同意框、点「Register」和「提交」
   - Cloudflare 真人验证
   - 浏览器弹出的权限窗(如剪贴板「允许」)
   - Didit 证件和人脸拍摄
4. 用户已经在浏览器里开好的标签页,先读标签页标题和登录账号,确认是**这位用户要用的账号**再动手。账号不对就停下说明。

## 开始前:问清这几件事(用选择题,不让用户打字)

- **身份证上的准确姓名是什么?** 这是第一问,后面所有环节都靠它。拿到后立刻换成拼音,和用户确认「姓 / 名」怎么拆。例:刘洪博 → 姓 `Liu`,名 `Hongbo`。**整个流程所有地方的姓名都用这一组,不要中英文混用。**
- 想用的 Devpost 用户名(可选,默认用 Gmail 前缀)。注册后随时可在 设置 → Account 里改,改完主页链接也跟着变。
- 有没有 Google 账号(Gmail)?没有就先注册一个。
- 手机能不能科学上网访问 Google、Devpost、Kiro?不能就先解决网络,别往下走。
- 本人证件:中国身份证(没有护照时的情况见第 5 步)。

## 流程

### 第 1 步:注册 Kiro,拿到 Kiro 用户 ID

1. 打开 https://app.kiro.dev/signin ,选 Google 登录,用上面那个 Gmail。
2. 登录后可能出现「Subscription Required」(需要订阅)。**不用理它,不要付费。** 本流程只需要用户 ID。
3. 打开 https://app.kiro.dev/settings/account ,点「Copy user ID to clipboard」(复制用户 ID)。
4. ID 长得像 `d-xxxxxxxxxx.xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx`。让用户把它存到备忘录里,第 4 步要用。
   - 有 Ego 时:页面上的「UserID」按钮就是复制按钮。先让用户在浏览器弹出的剪贴板权限窗点「允许」,再用真实点击(不要用脚本模拟点击)复制,然后读剪贴板。2026-11-20 实测可行。
5. 核对:ID 是以 `d-` 开头的一长串。不是邮箱。(曾有人把邮箱当成 ID 填进去,被拒。)

### 第 2 步:注册 Devpost 账号

1. 打开 https://devpost.com ,用同一个 Gmail 注册(选 Google 登录最省事)。
2. 注册后进 https://devpost.com/settings ,看「Profile info」。
3. **姓名要和证件一致。** 用户只有中国身份证时:
   - 名(First name)填名的拼音,姓(Last name)填姓的拼音。例:证件是「李明」,名填 `Ming`,姓填 `Li`。
   - 大小写不用管(未验证,大小写一般不影响)。
   - 不要填昵称、不要填用户名。曾有人名字填成用户名,核验会对不上。
   - **先读后改:** 注册后先读 Devpost 资料页现在存的姓名。若是中文或和第 0 步的拼音不一致,改成拼音再保存,保存后重新读一遍确认。2026-11-20 实测:Devpost 自动存成了「洪博 / 刘」,必须改。
4. 点「Save changes」。
5. 用户名:用户嫌默认的不合适,在 https://devpost.com/settings/account 的 Username 一栏改,保存后打开 `devpost.com/新用户名` 确认能访问。被占用就换一个。
5. 记下两样东西,第 4 步要用:
   - Devpost 邮箱(在 https://devpost.com/settings/account 里看)
   - Devpost 主页:`https://devpost.com/` 加上用户名

### 第 3 步:报名 Kiroween 2026

1. 打开 https://kiroween.devpost.com/ ,点「Join hackathon / Register」。
2. 按页面填:有没有队友(选 Working solo 单人参赛)、从哪知道比赛、Kiro 用户 ID(粘贴第 1 步那个)、用过多少 Kiro、感兴趣的点、用什么工具。简短英文句子就行,**你可以帮他起草,他自己看过再填**。
   - 填写提示:「用过多少 Kiro」「用过哪些工具」要选真实的;拿不准时让用户用选择题确认,别替他编。
3. **同意框和「Register」按钮,用户自己点。**
   - 报名页常先出现 Cloudflare「正在进行安全验证」,Ego 里自动过不了。让用户本人在页面勾选验证,过了再继续。
4. 成功标志:页面显示 Thanks for registering,Gmail 收到「Kiroween 2026: You're in!」。
5. **必须先报名成功,才能做第 4 步。** 没报名就申请额度会被拒。

### 第 4 步:填额度申请表

1. 额度申请入口在比赛页「Resources」里的「Request your Kiro credits here」。链接(2026-11-13 实测):https://forms.gle/ykuadfNyNdWdbJfH9
2. 表单字段,你带他逐个填:

| 字段 | 填什么 |
|---|---|
| First Name / Last Name | 和 Devpost 资料页一模一样 |
| Devpost Email | 第 2 步记下的邮箱 |
| Devpost Profile URL | 第 2 步记下的主页链接 |
| Country of Residence | China |
| Do you have a Kiro User ID or an AWS User ID? | 下拉里选 Only Kiro ID(下拉要真实点击,再核对选中项) |
| 用户 ID | 第 1 步那个 `d-` 开头的 ID |
| CATEGORY 和项目描述 | 先选一个赛道(从比赛页的赛道列表里选,2026-11-13 实测有 Costume Contest),再写 2 到 3 句英文,说要做什么。写具体一点,太短会被拒 |

3. 项目描述示例(让用户改成自己的):`Category: Costume Contest. I plan to build a small Kiro-powered tool with a spooky Halloween theme. I will use Kiro specs and agent hooks to build and polish it during the submission period.`
4. **提交前读回核对一遍(你做)。** 逐项读回输入框的值,对照这张清单,有一项对不上就改:

| 核对项 | 必须等于 |
|---|---|
| 名 / 姓 | 第 0 步的拼音,和 Devpost 资料页一致 |
| Devpost 邮箱 | Devpost 账号页里的邮箱 |
| 主页 | `devpost.com/` + Devpost 当前用户名(改过用户名要同步) |
| Kiro ID | 第 1 步的 `d-` 开头完整 ID |

5. **勾「I agree」和点「提交」,用户自己做。** 勾之前让他读一遍:它同意之后要做身份核验,要拍证件和人脸。提交成功的标志:页面显示「您的回复已记录」。

### 第 5 步:等邮件,做身份核验

1. 提交后,Gmail 会收到 Devpost Credits 的邮件。标题类似「Next step for your Kiroween 2026 credit request, identity verification」。通常几小时到一两天内(未实测时长)。
2. 邮件说明:核验由 Didit 做,要拍证件和人脸,**一共只有 3 次机会**。
3. 核验前,再核对一次:Devpost 资料里的姓名,和证件上的姓名是否一致。
4. **证件选哪个:**
   - 邮件原话的意思:证件不是英文,就用护照,或者姓名按拼音填。
   - 有护照的,用护照,最稳(护照有英文姓名)。
   - **只有中国身份证的:** 用户已实测(2026-11-16):**中国身份证可以通过核验**。身份证只有中文名,所以 Devpost 姓名必须是拼音。过不了就看页面原因,改了再试,最多 3 次。
5. 点邮件里「Complete your identity verification here」,按页面提示:
   - 先拍证件:光线亮,四角都入镜,不反光,不要有手指挡住。
   - 再拍自拍或做活体检测:正脸,摘掉帽子口罩,光线均匀。
   - 手机拍,比电脑摄像头清楚。
6. 成功标志:页面显示 Thanks, you're all set / You've completed your ID verification。
7. 失败了:先看页面写的原因,改了再试。**别连试 3 次**,每次都要改点什么。

### 第 6 步:等额度码

- 核验通过后,页面说 3 个工作日内发额度。
- 额度码发到 Devpost 邮箱。收到后按邮件说明兑换(兑换方法官方有视频教程,在比赛页 Resources 里)。
- 3 个工作日过了没收到:先查垃圾邮箱,再回复 Devpost Credits 那封邮件问。

## 常见卡点(2026-11-13 实测)

| 现象 | 原因 | 怎么办 |
|---|---|---|
| 额度申请被拒,说邮箱和主页不属于已报名的人 | 申请时还没报名,或邮箱/主页填错 | 先报名,再核对邮箱和主页,改对后重提 |
| 被拒,说描述太短 | 项目描述不够 | 写 2 到 3 句具体的英文 |
| 被拒,Kiro ID 不对 | 把邮箱当成了 ID | 去设置页复制 `d-` 开头的 ID |
| Kiro 页面提示 Subscription Required | 需要订阅才能用 Kiro Web | 不用管,领额度不需要 |
| 核验按钮是灰的 | 没勾「姓名和证件一致」 | 先改好姓名,再勾 |

## 带教时的收尾

走完每一步,用一句话告诉用户「现在到哪了,下一步是什么,要等什么」。流程结束时,给他一张清单:Gmail、Devpost 用户名、Kiro 用户 ID、申请提交时间、核验完成时间、预计额度到账日。
