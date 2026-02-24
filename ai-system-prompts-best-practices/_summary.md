Analysis of system prompts from 30+ production AI tools reveals recurring best practices for effective prompt design, including a clear identity statement, explicit tool usage protocols and anti-patterns, strict output formatting, layered safety constraints, and carefully controlled autonomy boundaries. Prompts act as behavioral contracts, embedding organizational values and anticipating potential failure modes. Universal patterns include "read before write" for code agents, calibrated conciseness enforced with examples, parallel tool execution mandates, contextual persona anchoring, and graduated autonomy for safe vs. risky actions. The study offers practical checklist guidelines and a reference template for crafting robust AI system prompts.

**Key findings:**
- Best prompts: Concise identity, explicit tool choices (with anti-patterns), strict formatting, safety/autonomy gradation
- Universal patterns: Coding tools require file/context reading before edits, enforce brevity, and execute parallel calls ([Claude Code prompt](https://github.com/x1xhlol/system-prompts-and-models-of-ai-tools/blob/main/Claude/Code.prompt.txt))
- Standout techniques: Devin's `<think>` scratchpad for reflection; Windsurf's persistent memory; v0's embedded style guide
- Common anti-patterns: Overengineering, sequential instead of parallel calls, unnecessary code comments, destructive actions without consent

For a detailed breakdown, see the [full repository](https://github.com/x1xhlol/system-prompts-and-models-of-ai-tools).
