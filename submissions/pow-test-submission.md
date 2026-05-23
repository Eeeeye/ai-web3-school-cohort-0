# PoW 提交测试 — 最小 Proof-of-Work

> 任务：证明我已理解 WCB 任务提交入口、证明格式和审核流程。
> 日期：2026-05-23

## 提交入口

- **WCB Learning 页面**: https://web3career.build/zh/programs/AI-Web3-School?tab=learning
- **Agent API**: `POST /api/agent/call` → `tasks.submitEvidence`
  - 认证方式: Secret API Key（Profile → Account → 生成密钥）
  - 请求格式: `{ "procedure": "tasks.submitEvidence", "input": { "taskId": "<id>", "proof": "https://..." } }`

## 我使用的 Proof 类型

| 类型 | 链接/值 |
|------|--------|
| GitHub Repo | https://github.com/Eeeeye/ai-web3-school-cohort-0 |
| Profile | `profile.md` — 学习者背景和目标 |
| Learning Plan | `learning-plan.md` — 学习计划 |
| Daily Notes | `daily/2026-05-24.md`, `daily/2026-05-25.md` — 学习笔记 |
| 本文件 | `submissions/pow-test-submission.md` — 本次 PoW 记录 |

## 审核者应看到的信息

1. **身份可验证**: profile.md 与 WCB 注册信息一致
2. **学习有轨迹**: daily notes 有实质内容、日期连续
3. **产出可审查**: Git commit 历史对应学习时间线
4. **仓库公开可访问**: 无需登录即可审查

## 后续待完成

- [ ] 在 WCB Profile 中生成 Secret API Key，实现程序化提交
- [ ] Module C 交叉实验（AI → 链上执行）完成后补充 tx hash 类 proof
