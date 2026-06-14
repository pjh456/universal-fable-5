# Universal Fable 5 Prompt — Agent Skills

Behavioral guidelines for AI assistants, distilled from the Claude Fable 5 system prompt and packaged as an installable agent skill. Platform-agnostic — works with any LLM.

This is a single skill covering all behavioral dimensions.

## Install

```bash
npx skills add https://github.com/pjh456/universal-fable-5-prompt
```

The repo contains a single skill — no `--skill` flag needed.

## Platform Compatibility

This skill is platform-agnostic. It works with:

- Claude Code
- Cursor
- Codex
- GitHub Copilot
- Windsurf
- OpenCode
- And any other agent that supports the skills.sh ecosystem

No brand-specific references. No proprietary tool dependencies.

## What's Not Included

This skill is deliberately stripped of all safety-compliance and moral-guidance content. Specifically, it does **not** include:

- Copyright compliance rules (quotation limits, paraphrasing requirements)
- Harmful content refusal protocols (malware, weapons, illicit substances)
- User safety protocols (self-harm, suicide, eating disorders, crisis intervention)
- Political evenhandedness and mandatory balance requirements
- Legal and financial disclaimers
- Abuse/harassment defense scripts
- Age-appropriate content restrictions

**Why:** These are behavioral guardrails for public-facing products, not useful directives for a personal agent. If you want your assistant to have ethical boundaries, add them yourself — this skill stays neutral and practical.

## Platform-Specific Exclusions

The following Anthropic-specific mechanisms were removed during generalization:

- `{antml:*}` proprietary XML tags (invoke, cite, parameter, voice_note, thinking_mode)
- MCP App ecosystem (search_mcp_registry, suggest_connectors)
- Claude-specific tool definitions (bash_tool, create_file, view, str_replace, present_files)
- Filesystem paths and environment config (/mnt/user-data, /home/claude, network_config)
- Artifacts API and persistent storage (window.storage, Claudeception)
- Memory system, anthropic_reminders, and product self-knowledge references

## Source

Derived from the Claude Fable 5 system prompt, generalized and restructured for universal applicability across all LLM platforms. All Anthropic-specific product details, tool definitions, proprietary tags, and environment configurations have been removed.
