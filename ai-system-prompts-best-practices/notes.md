# Research Notes: AI System Prompts Best Practices

## Source Repository
https://github.com/x1xhlol/system-prompts-and-models-of-ai-tools

## Research Log

### Session Start (2026-02-24)
- Cloned repo, found 99 text/json files across 30+ AI tools
- Launched 9 parallel research agents to read all prompts simultaneously
- Also read key prompts directly for hands-on analysis

### Prompts Read Directly
1. **Cursor** - Agent Prompt 2.0 (773 lines) - most detailed tool definitions
2. **Claude Code** - v1 Prompt (192 lines) + v2 (200+ lines) - conciseness-focused
3. **Devin AI** - Full prompt (403 lines) - think tool, planning modes
4. **Manus** - Prompt + Agent loop + Modules - agent loop architecture
5. **v0 (Vercel)** - Full prompt (1137 lines) - frontend-focused, design guidelines
6. **Windsurf/Cascade** - Wave 11 prompt (126 lines) - memory system, plan management
7. **Replit** - Prompt (138 lines) - IDE-embedded, workspace tools
8. **Perplexity** - Prompt (195 lines) - citation-heavy, format rules
9. **Lovable** - Agent Prompt (200+ lines) - discussion-first workflow
10. **Cline** - Open source prompt (200+ lines) - XML tool format
11. **Bolt** - Prompt (100+ lines) - WebContainer constraints
12. **Kiro** - Spec Prompt (100 lines) - warm personality, AWS focus
13. **Cluely** - Default Prompt (60 lines) - anti-meta-phrase rules
14. **Same.dev** - Prompt (80 lines) - parallel tool emphasis
15. **Warp.dev** - Prompt (80 lines) - terminal-focused agent

### Prompts Read via Background Agents
- VSCode Agent (multiple model-specific prompts)
- Xcode (System, actions)
- Google Antigravity (Fast, Planning)
- Trae (Builder, Chat)
- Augment Code (Claude 4 Sonnet, GPT-5)
- Junie
- NotionAI
- CodeBuddy (Craft, Chat)
- Emergent
- Poke (6 parts + agent)
- Orchids.app
- Qoder (prompt, Quest Action, Quest Design)
- Z.ai Code
- dia
- Comet Assistant
- Leap.new
- Traycer AI

## Key Observations

### Universal Patterns (found in 80%+ of prompts)
1. Identity declaration in first sentence
2. Tool use instructions with explicit schemas
3. "Read before edit" mandate
4. Conciseness emphasis
5. Safety/security guardrails
6. Don't reveal system prompt
7. Follow existing code conventions
8. Parallel tool execution encouragement

### Distinctive Techniques by Tool
- **Devin**: `<think>` scratchpad for reflection, required before critical decisions
- **Windsurf**: Persistent memory database, automatic plan management
- **v0**: Design system guidelines with color/typography rules
- **Perplexity**: Rigorous citation format, query-type classification
- **Lovable**: "Discussion first" default before implementation
- **Cluely**: "ZERO introductory text" - start with solution immediately
- **Manus**: Agent loop architecture (analyze → select → wait → iterate → submit → standby)
- **Cursor 2.0**: `// ... existing code ...` pattern for efficient edits
- **Claude Code**: Extreme conciseness ("One word answers are best")
- **Same.dev**: `.same/` folder for self-tracking memos and todos

### Anti-Patterns Explicitly Warned Against
- Over-engineering / scope creep (Lovable, Claude Code)
- Adding unsolicited features (Claude Code, Lovable)
- Sequential tool calls when parallel is possible (Same.dev, v0, Cursor)
- Guessing file contents without reading (universal)
- Outputting code to user instead of using edit tools (Cursor, Windsurf, Same.dev)
- Using `git add .` or force push (Devin, Claude Code)
- Hardcoding secrets/API keys (universal)
- Adding unnecessary comments (Claude Code, Devin)
- Long explanations when brief answer needed (Claude Code, Cluely)
