<!--
  演示动图 assets/demo.gif 录制后取消相应注释即可启用（见 Docs/18）。
  美学：复古纸张 / 编辑式排版。视觉质感由 assets/*.svg 承载（GitHub 会过滤内联 CSS，故用 SVG 图片）。
-->

<a id="top"></a>

<div align="center">

<img src="https://raw.githubusercontent.com/MrMaii/-.skill/main/assets/banner.svg" width="820" alt="向上汇报体 · report-to-boss" />

<br/>

[![License](https://img.shields.io/badge/License-MIT-b8643f?style=flat&labelColor=2c2620)](LICENSE)
&nbsp;
[![Cursor Skill](https://img.shields.io/badge/Cursor%20Skill-report--to--boss-b8643f?style=flat&labelColor=2c2620)](.cursor/skills/report-to-boss)
&nbsp;
[![Version](https://img.shields.io/badge/version-0.1.0-b8643f?style=flat&labelColor=2c2620)](CHANGELOG.md)

<sub>

[快速开始](#三--快速开始) · [它好在哪](#一--困局) · [四层模型](#二--它是怎么思考的) · [设计文档](#六--想深入)

</sub>

</div>

<br/>

> *把用户当领导，把自己当一个靠谱、有想法、会表达的下属。*
> *汇报不是把事说完，而是让对方一眼看懂、心里有数、知道下一步。*

<br/>

---

## 一 · 困局

让 AI 干个活，它常常甩回来一大坨——

> "我先打开了文件，然后引入了一个库，接着配置了参数，又改了返回码，最后我还加了……"

读到最后一行，你才知道**到底成没成、有没有坑、接下来要你干嘛**。

它在*交代过程*，而不是在*向你汇报*。这是今天几乎所有 AI 的通病。

`report-to-boss` 只改一件事：**让 AI 学会向领导汇报。**

<br/>

| 默认 AI（流水账） | 挂上 report-to-boss |
| :--- | :--- |
| 我先打开 `auth` 中间件，然后引入限流库，接着配置每分钟次数，又改返回码，还加了配置项…… | **结论** — 已完成登录接口限流（每 IP 每分钟 5 次），自测通过。 |
| *（重点埋在最后，自己捞）* | **价值** — 相当于给登录口加了个"保安"，狂试密码会被自动拦，挡住绝大多数撞库。 |
| *（风险？自己想）* | **风险** — 阈值按默认值设的，高峰可能偏严，建议你确认。 |
| *（下一步？没说）* | **下一步** — 阈值 OK 我就补测试；要按用户维度限流我再调。 |

<div align="right"><sub><i>左边让你省事；右边让你省心，还顺手帮你想到下一步。</i></sub></div>

<br/>

---

## 二 · 它是怎么思考的

汇报是一套层层递进的能力——**下层是地基，上层是艺术，四层同在方为知音。**

<div align="center">
<img src="https://raw.githubusercontent.com/MrMaii/-.skill/main/assets/layers.svg" width="640" alt="四层沟通能力模型" />
</div>

> 权重随场景流转：*事越急，越往下沉，重实质；事越大越开放，越往上扬，重激发。*

<br/>

---

## 三 · 快速开始

> 前提：你在用 [Cursor](https://cursor.com)。

**一、取下这套技能**

```bash
git clone https://github.com/MrMaii/-.skill.git
```

**二、安进你的技能目录**

| 位置 | 路径 | 作用范围 |
| :--- | :--- | :--- |
| 个人（推荐） | `~/.cursor/skills/report-to-boss/` | 所有项目通用 |
| 项目 | `<你的项目>/.cursor/skills/report-to-boss/` | 随仓库共享给团队 |

```bash
cp -r ./-.skill/.cursor/skills/report-to-boss ~/.cursor/skills/
```

**三、照常派活**

像平时一样布置任务，它汇报时便会自动用"汇报体"。想暂时收起？说一句 **"用普通方式说"** 即可。

<br/>

---

## 四 · 招牌：价值陈述五点

讲"做成了什么"时，它会用*外行也听得懂的大白话*讲清这五点——

1. **这是个啥** &mdash; 一句话讲清，不飙术语
2. **为什么有意义** &mdash; 解决了什么痛点
3. **花了多久** &mdash; 投入几何，诚实不杜撰
4. **下一步** &mdash; 接下来做什么
5. **为什么值得投资** &mdash; 投入产出 · 护城河 · 想象空间

> 准则：营销的是*价值*，不是*自己*。让事实自然显现价值——可点睛，不可夸大，不邀功。

<br/>

---

## 五 · 适用 / 不适用

| 适用 | 不硬套 |
| :--- | :--- |
| 任务完成汇报 | 闲聊、情感陪伴 |
| 进展 · 决策请示 | 头脑风暴、自由发散 |
| 问题 · 故障上报 | 创意 · 文学写作 |
| 成果复盘 · 方案提报 | *（说一句"普通方式"即可关闭）* |

<br/>

---

## 六 · 想深入

这套技能不是拍脑袋做的——它有完整的产品、心理学与方法论文档。

| 文档 | 内容 |
| :--- | :--- |
| [项目概述](Docs/01-项目概述.md) | 愿景 · 定位 · 核心原则 |
| [用户行为心理学分析](Docs/03-用户行为心理学分析.md) | 为什么这样说更有效 |
| [汇报沟通方法论](Docs/04-汇报沟通方法论.md) | 金字塔 · BLUF · 闭环 |
| [四层沟通能力模型](Docs/15-四层沟通能力模型.md) | 核心框架 |
| [知音体验与灵感激发设计](Docs/16-知音体验与灵感激发设计.md) | 最高层的设计 |

<sub>全部 18 篇见 [Docs/](Docs/)。贡献请见 [CONTRIBUTING](CONTRIBUTING.md)。</sub>

<br/>

---

## 许可证

[MIT](LICENSE) © 2026 MrMaii. 自由使用、修改、商用与再分发。

<br/>

<div align="center">

<sub>❧</sub>

<sub><i>如果它帮你省下了读流水账的时间，给个 ⭐ 就是最好的汇报。</i></sub>

<sub><a href="#top">回到顶部</a></sub>

</div>
