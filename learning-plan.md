# Learning Plan

Based on the [AI x Web3 School Handbook](https://aiweb3.school/zh/handbook/) and [WCB curriculum](https://web3career.build/zh/programs/AI-Web3-School?tab=learning).

## Week 1 | AI & Web3 Basics

Goal: Build shared language, complete AI tool practice, testnet interaction, and minimum AI x Web3 crossover experiment.

### Module A | AI Basics: LLM to Agent Workflow

- [ ] Understand LLM fundamentals (context, generation, limitations)
- [ ] Learn the 4 control layers: context window, system instruction, prompt, tool calling
- [ ] Call LLM API (try Anthropic Claude / OpenAI / Z.ai GLM)
- [ ] Understand Prompt → Workflow → Agent boundaries
- [ ] Try AI coding tools (Claude Code / Codex CLI)
- [ ] Learn AI output verification: fact errors, hallucinated refs, reasoning drift, execution overreach, tool misuse
- [ ] Understand Agent core components: state, memory, MCP, skills, tool calling, tracing, guardrails, handoff, error recovery
- [ ] Know when to use (and not use) an Agent

**Practice**: Set up a learning agent, create GitHub repo, generate a small demo with agent assistance.

### Module B | Web3 Basics: Account, Wallet, Signature & On-chain Execution

- [ ] Understand account, address, wallet relationship
- [ ] Mnemonic phrase, private key, address — what each is and why secrets must stay secret
- [ ] Signing ≠ login, authorization ≠ transfer — what each action actually means
- [ ] AI Agent should never touch private keys; human-in-the-loop for signing/transfer/contract writes
- [ ] Gas, L1/L2, testnets, block explorers, transaction receipts
- [ ] Account abstraction, smart accounts, multi-sig, Safe, ERC-4337, Session Key

**Practice**: Create test wallet, get testnet ETH, send test transaction, deploy minimal contract via Remix/Foundry, compare EOA vs smart account.

### Module C | Minimum Crossover Experiment: AI Output → On-chain Execution

- [ ] AI generates contract interaction script → human reviews → testnet execution
- [ ] AI generates transaction explanation → verify on block explorer
- [ ] Record the full chain: AI output → human review → wallet confirm → on-chain execution → verification

---

## Week 2 | AI x Web3 Intersection Topics

Goal: Enter real problem spaces, choose a direction, form a project proposal.

- [ ] Agentic Commerce / Payment
- [ ] Dev Tooling
- [ ] AI Security / Privacy
- [ ] AI x Governance / Coordination
- [ ] Open Track

---

## Week 3 | Practice Deepening & Hackathon Prep

- [ ] Agent workflow + wallet confirmation
- [ ] On-chain receipts, testnet payments
- [ ] Governance proposal summarization
- [ ] Risk control strategies
- [ ] Define Hackathon track, project topic, tech path, team roles, demo plan

---

## Week 4 | Hackathon & Demo

- [ ] Build core features
- [ ] Write tests, README, demo flow
- [ ] Submit: project name, track, demo link, repo, video, verification materials
