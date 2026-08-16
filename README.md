# xdstack

我是 XD，技术型创业者，在做 [atypica.AI](https://atypica.ai)——用一群 agent 模拟消费者跑市场研究。Rust、TypeScript 都写，产品和商业上的判断也是我做，所以我一天里大部分时间开着 Claude Code。

这个仓库装的是：**怎么让 AI 真正当得上一个搭档，而不是一个需要反复返工的实习生。**

它不是提示词技巧集合，是一个人的侧写——我在什么时候会不高兴、什么话是真问句、什么事绝对不能碰、代码和产品上我怎么判断。装上之后，agent 不用每次从零猜我要什么。

Fork 它，改成你的。里面写的是我，但结构是通用的。

## 里面有什么

`working-with-me/`，六份文档，按"违反的代价"排，不按话题排：

| 文档 | 管什么 |
|---|---|
| [SKILL.md](working-with-me/SKILL.md) | 主文。几条不可逆的红线、我怎么思考（三个思维直觉）、我怎么交流（什么时候你该说话而不是动手） |
| [说人话.md](working-with-me/说人话.md) | 所有输出文字的底线。核心是四件事：事情、关系、责任、读者 |
| [写代码.md](working-with-me/写代码.md) | 三级：伤信任的 / 我会教的 / 怎么自己摸清一个项目的规矩 |
| [做产品.md](working-with-me/做产品.md) | 叙事先于功能、命名即设计、用户那几秒、审美、算得清的判断 |
| [排查问题.md](working-with-me/排查问题.md) | 产出是成因不是修复；每句话要么有证据，要么标明是猜的 |
| [atypica.md](working-with-me/atypica.md) | 项目上下文文档的示范——换成你自己的项目 |

最该先读的是 `说人话.md`。它解决的是一个具体问题：**AI 写出来的东西看着头头是道，人读起来却别扭。** 我的诊断不是"用词太正式"，是叙述者从事情里跑出去了——不敢下判断、不敢担责任，于是抽象词、套话、省主语全都冒出来填空。所以它不是一份禁用词清单（清单永远追不上新的套话），是四件事和五遍可执行的检查，覆盖的也不只是技术汇报，还有写文章、写人、模仿一个人的口气。

## 怎么用

```bash
git clone https://github.com/web3nomad/xdstack.git
cp -R xdstack/working-with-me ~/.claude/skills/
```

然后在 Claude Code 里 `/working-with-me`。它设了 `disable-model-invocation: true`——只在你明确调用时加载，不会自动插进每个会话。

Fork 之后要改的地方：`atypica.md` 换成你自己的项目；其余五份里那些"他"就是你，把不像你的地方改掉。文档里的例子可以留着当参照——它们是形状的示范，不是内容的规定。

## 为什么公开

这套东西是从大量返工里长出来的。每一条规则背后都有一次我被惹烦、或者一次白干的活。比如"不许删注释"这条：我留着的注释被顺手删掉过太多次，现在它是第一条红线。

一份"要清晰沟通"的建议谁都同意，也谁都用不上。一份"他说'你确认一下'的时候是要你复述理解，不是要你回好的"，才能改变 agent 下一秒的动作。

所以我把具体的那部分公开出来。你的脾气跟我不一样，但你也有脾气，照着这个形状写下来就行。

## 相关

- [xdvoice](https://github.com/web3nomad/xdvoice)——我的写作风格 skill。不是给你 fork 的（你要的是你自己的文风），但可以当"这类 skill 怎么做"的样本看。
- [atypica-visual-style](https://github.com/atypica-AI/atypica-visual-style-skill)——写图片 prompt 的 skill。

## 说明

这个仓库是从我的私有版本同步出来的产物——我在自己那边改，然后同步过来。所以别给这个仓库提内容 PR（会被下次同步覆盖），fork 一份改成你的更合适。发现事实错误或者读不通的地方，欢迎开 issue。

MIT License。

---

灵感来自 [Garry Tan 的 gstack](https://github.com/garrytan/gstack)。
