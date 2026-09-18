# 25 AI Productivity Skills

Portable [Agent Skills](https://agentskills.io) (`SKILL.md`) for Claude, Claude Code, ChatGPT, and Gemini.

Inspired by the catalog Nico ([@nicos_ai](https://x.com/nicos_ai/status/2053870934965043354)) published on 11 May 2026. His X Article described 25 skills in `.md` form; the original embedded files were not released as a public repo. This repository is a **spec-compliant reconstruction** of those 25 skills so you can install them.

## Skills

### Students
| Skill | Folder |
|-------|--------|
| Structured Notes Generator | [`structured-notes-generator`](structured-notes-generator/SKILL.md) |
| Exam Preparer | [`exam-preparer`](exam-preparer/SKILL.md) |
| Learning Roadmap Generator | [`learning-roadmap-generator`](learning-roadmap-generator/SKILL.md) |
| Complex Concepts Explainer | [`complex-concepts-explainer`](complex-concepts-explainer/SKILL.md) |
| Academic Paper Writer | [`academic-paper-writer`](academic-paper-writer/SKILL.md) |
| Flashcards Creator | [`flashcards-creator`](flashcards-creator/SKILL.md) |
| Study Session Planner | [`study-session-planner`](study-session-planner/SKILL.md) |

### Work productivity
| Skill | Folder |
|-------|--------|
| Professional Email Writer | [`professional-email-writer`](professional-email-writer/SKILL.md) |
| Meetings and Minutes Organizer | [`meetings-minutes-organizer`](meetings-minutes-organizer/SKILL.md) |
| CV and LinkedIn Optimizer | [`cv-linkedin-optimizer`](cv-linkedin-optimizer/SKILL.md) |
| Presentation Preparer | [`presentation-preparer`](presentation-preparer/SKILL.md) |

### Research and analysis
| Skill | Folder |
|-------|--------|
| Deep Research Synthesizer | [`deep-research-synthesizer`](deep-research-synthesizer/SKILL.md) |
| Source Validation | [`source-validation`](source-validation/SKILL.md) |
| Knowledge Structuring | [`knowledge-structuring`](knowledge-structuring/SKILL.md) |
| Competitive Intelligence | [`competitive-intelligence`](competitive-intelligence/SKILL.md) |

### Video and visual content
| Skill | Folder |
|-------|--------|
| Video Script Generator | [`video-script-generator`](video-script-generator/SKILL.md) |
| Hooks Generator | [`hooks-generator`](hooks-generator/SKILL.md) |
| Flowchart Builder | [`flowchart-builder`](flowchart-builder/SKILL.md) |

### Code and automation
| Skill | Folder |
|-------|--------|
| Code Documenter | [`code-documenter`](code-documenter/SKILL.md) |
| Unit Test Generator | [`unit-test-generator`](unit-test-generator/SKILL.md) |
| Debugger Assistant | [`debugger-assistant`](debugger-assistant/SKILL.md) |
| Regex Builder | [`regex-builder`](regex-builder/SKILL.md) |
| Conventional Commits Generator | [`conventional-commits-generator`](conventional-commits-generator/SKILL.md) |
| Code Review | [`code-review-skill`](code-review-skill/SKILL.md) |
| Workflow Automation Agent | [`workflow-automation-agent`](workflow-automation-agent/SKILL.md) |

## Install

Each skill is a folder with a `SKILL.md`:

```
skill-name/
  SKILL.md
```

### Claude Code

```bash
git clone https://github.com/KRoshanK/ai-productivity-skills.git
mkdir -p ~/.claude/skills
cp -R ai-productivity-skills/structured-notes-generator ~/.claude/skills/
```

Or copy any subset of folders into `.claude/skills/` inside a project.

If you use the skills CLI:

```bash
npx skills add KRoshanK/ai-productivity-skills
```

### Claude.ai

Zip one skill folder and upload via **Customize → Skills**.

### ChatGPT / Gemini

Open the `SKILL.md` you need and paste it as custom instructions or system context at the start of the chat.

## Format

Skills follow the Agent Skills standard:

```markdown
---
name: skill-name
description: What it does and when to use it.
---

# Skill Name
Instructions the model follows when the skill is active.
```

## License

MIT. See [LICENSE](LICENSE).
