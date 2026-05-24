# Task 3: 用 Agent 生成可交互学习产物

## Source

WCB Week 1 Task 3 — 选择一个 Week 1 概念，让 Agent 生成可交互产物

## Objective

选择一个概念（链上交易生命周期），用 AI Agent 生成一个可交互的 HTML 可视化页面。

---

## Agent 做了什么

**Agent**: Claude Code (GLM-5.1 via 火山引擎 ARK)

**Prompt**: 要求生成一个展示链上交易 5 个阶段（RPC → Mempool → Builder → Validator → Finalize）的交互式 HTML 页面，包含：
- 深色 Web3 风格
- 水平流程图 + 动画连接线
- 可展开阶段卡片（中文 + 英文关键词 + 现实类比）
- "播放动画"按钮自动推进
- 移动端响应式

**执行过程**:
- 4 轮对话
- 耗时 113 秒
- 成本 $0.31
- 生成了 415 行、17KB 的单文件 HTML

---

## 人工修改了什么

- [ ] 待审查：验证所有技术细节准确性（Gas base fee / tip fee、Slashing 机制、12 分钟确认时间）
- [ ] 待审查：中文翻译是否自然
- [ ] 待修改：可能需要在 README 中添加截图预览
- [ ] 待测试：在移动端浏览器验证响应式效果

---

## 哪些输出不可靠

1. **Gas 机制细节**: Agent 可能简化了 EIP-1559 的 base fee 销毁和 priority fee 机制，需要人工对照文档验证
2. **12 分钟确认时间**: 以太坊的 finality 大约 2 个 epoch（~12.8 分钟），Agent 可能简化表述
3. **Builder 角色**: 在 PBS（Proposer-Builder Separation）架构下 Builder 和 Proposer 是分开的，Agent 可能合并了这两个角色
4. **MEV 说明**: 可能不够准确，需要对照 Flashbots 文档

---

## 下一步改进

- [ ] 人工审核后修正技术细节
- [ ] 添加英文版本切换
- [ ] 补充更多交互：hover 显示 Gas 计算器、自定义 Gas 看排队优先级
- [ ] 考虑添加"模拟一笔交易"功能 — 用户输入地址和金额，页面模拟走一遍流程
- [ ] 部署到 GitHub Pages 方便分享

---

## Proof-of-Work

- 产物: `experiments/tx-lifecycle/index.html`
- Claude Code session: `4e2c7916-1595-43a7-8b14-3e880dd1924c`
- Commit: [本次提交]
