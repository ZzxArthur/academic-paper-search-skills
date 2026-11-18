# Academic Paper Search - Claude Code Instructions
# 复制本文件到你的项目根目录下的 CLAUDE.md 或 .claude/skills/paper-search.md

## Academic Literature Survey & Capability Matrix Protocol

When assisting the user with academic paper discovery, related work surveys, or topic ideation:

1. **Clarification on Broad Topics**:
   - Detect if the user query is broad (e.g. "具身智能", "强化学习大模型").
   - Ask first: "Do you want latest survey papers + representative milestone works, or focus on a specific sub-direction?"
   - Offer 3-5 mutually exclusive concrete sub-directions.
2. **Reading Order**:
   - Organize results in progressive reading sequence: Foundational -> Methodological Evolution -> Latest SOTA.
   - For each paper, detail: Publication/Acceptance date, official venue (e.g. CVPR/NeurIPS/RSS/ICML), official GitHub repo status (✓/△/✗/?) with link, core contribution, and why to read it at this specific order.
3. **Comparative Innovation Matrix**:
   - Build a comparison table (Rows: Papers; Columns: 6-8 core technical dimensions).
   - Use `✓`, `✗`, `△` to mark coverage.
4. **Synthesis & Gap Mining**:
   - Synthesize unaddressed combinations from empty/cross cells (`✗`).
   - Propose 2-3 novel, actionable research directions with potential technical bottlenecks and minimum viable evaluation setup.
