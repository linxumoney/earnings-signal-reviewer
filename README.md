# Earnings Signal Reviewer：财报不是数字复述，而是判断什么变了

收入增长并不自动等于经营变好，利润超预期也可能来自一次性项目。真正有价值的财报分析，要把报告事实、管理层叙事和分析推断分开。

`earnings-signal-reviewer` 是一个面向投资研究、战略和经营分析的开源 Agent Skill。它生成来源可追溯的财报信号简报，重点检查预期差、盈利质量、指引变化和论点影响。

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

## 方法参考

本项目独立实现。财报研究问题域参考了 [anthropics/financial-services](https://github.com/anthropics/financial-services) 的公开金融 Skill，该项目采用 Apache-2.0 License。本项目不复制其报告格式、篇幅约束、图表模板、提示词或代码，也不代表 Anthropic 官方项目。

## 免责声明

输出仅用于信息整理和研究，不构成投资、会计、税务或法律建议。

## License

MIT License。
