# Earnings Signal Reviewer：AI 财报分析与盈利质量审阅 Skill

收入增长并不自动等于经营变好，利润超预期也可能来自一次性项目。真正有价值的财报分析，要把报告事实、管理层叙事和分析推断分开。

`earnings-signal-reviewer` 是一个面向投资研究、战略和经营分析的开源 AI 财报分析 Agent Skill。它生成来源可追溯的季度财报简报，重点检查业绩预期差、盈利质量、现金流、一次性项目、管理层指引和研究论点变化。兼容支持 `SKILL.md` 的 Codex、Claude Code、Cursor 和 OpenCode。

## 默认输出

- 一句话变化判断
- 关键指标与预期差
- 盈利质量和现金流检查
- 管理层解释与证据强度
- 指引变化和隐含假设
- 风险、反证与下一次验证点

## 使用示例

```text
用 $earnings-signal-reviewer 分析这家公司最新季度财报。
请把事实、管理层说法和你的推断分开，并附原始来源。
```

## 安装

```bash
cp -R skills/earnings-signal-reviewer ~/.codex/skills/
```

## 适用场景

- 上市公司季度财报、年报和业绩电话会分析
- 收入、利润、现金流和经营指标的同比与环比变化
- Beat/Miss、公司指引和市场预期差分析
- 检查盈利质量、一次性收益、库存和应收变化
- 将财报事实、管理层解释和分析推断分开

## 常见问题

### 它会给出股票买卖建议吗？

不会。Skill 用于信息整理和研究，不提供个性化买入、卖出、仓位或收益承诺。

### 没有一致预期数据怎么办？

它不会滥用“超预期”一词，而会改用同比、环比或公司原指引作为比较基准，并标出数据缺口。

### 为什么要区分事实和管理层解释？

财报数字可以核验，管理层对原因和未来的说法则需要进一步验证。把两者分开能减少被叙事带着走的风险。

## 方法参考

本项目独立实现。财报研究问题域参考了 [anthropics/financial-services](https://github.com/anthropics/financial-services) 的公开金融 Skill，该项目采用 Apache-2.0 License。本项目不复制其报告格式、篇幅约束、图表模板、提示词或代码，也不代表 Anthropic 官方项目。

## 免责声明

输出仅用于信息整理和研究，不构成投资、会计、税务或法律建议。

## License

MIT License。

## 商业授权

个人学习、研究、测试和非商业使用可以。商业使用请先联系 **linxu.money@gmail.com** 获得授权，详见 [COMMERCIAL-LICENSING.md](COMMERCIAL-LICENSING.md)。

