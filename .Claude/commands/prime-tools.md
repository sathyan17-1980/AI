
## Context

You are about to work on building or modifying agent tools that will be used by Pydantic AI agents. Load tool development patterns from C:\Users\sathy\Downloads\AI Mastery\AI Agentic Coding course\agentic-coding-course\module_4\4_exercise\exercise_1\adding_tools_guide.md . This will help the agent understand the tool docstring patterns and best practices to follow when building tools. 

## Read

Read the tool docstring patterns: C:\Users\sathy\Downloads\AI Mastery\AI Agentic Coding course\agentic-coding-course\module_4\4_exercise\exercise_1\adding_tools_guide.md

## Process

Understand and internalize:

1. **Core Philosophy** - How agent tool docstrings differ from standard docstrings
2. **7 Required Elements** - One-line summary, "Use this when", "Do NOT use", Args with guidance, Returns, Performance Notes, Examples
3. **Agent Perspective** - Writing for LLM comprehension and tool selection
4. **Token Efficiency** - Documenting token costs and optimization strategies
5. **Anti-patterns** - Common mistakes that confuse agents
6. **Template Structure** - The exact format to follow

Pay special attention to:

- "Use this when" (affirmative guidance for tool selection)
- "Do NOT use" (negative guidance to prevent tool confusion)
- Performance Notes (token costs, execution time, limits)
- Realistic examples (not "foo", "bar", "test.md")

## Report Back

### Key Principles (5 bullets max)
What are the core principles you understood?

- Write for AI agents, not humans - focus on behavioral instructions and constraints
- Be explicit about what NOT to do, as agents lack human intuition about misuse
- Front-load critical information - agents process sequentially and may miss buried details
- Use imperative commands ("Use X for Y") rather than descriptive statements
- Include concrete examples inline - agents learn better from示例 than abstract descriptions

### Critical Distinctions
What makes agent tool docstrings different from standard docstrings?

- Agent docstrings focus on when and how to use the tool, not just what it does
- They include explicit negative constraints ("Do NOT use for X") that human docs omit
- They embed decision trees and conditional logic directly in the description
- They prioritize behavioral guardrails over technical specifications

Why does "Do NOT use" matter?

- Agents explore the solution space broadly and may misapply tools creatively
- Without explicit boundaries, agents lack the contextual judgment humans have
- Prevents wasted tokens on inappropriate tool calls and error recovery
- Clarifies tool scope when multiple similar tools exist

### Template Internalized
Confirm you understand the structure you'll follow

- Start with one-line purpose, then "When to use" conditions
- Add "Do NOT use" constraints immediately after
- Include parameter guidance with examples inline
- End with usage pattern or expected workflow
- Keep total under 150 words unless complexity demands more

### Ready to Apply
One sentence confirming you're ready to write agent-optimized tool docstrings
- Keep it scannable - I want to verify understanding in 30 seconds.
- Ready to write agent-first docstrings that prioritize behavioral clarity, explicit constraints, and decision-making guidance over technical documentation.

---