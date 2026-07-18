# Anti-AI Writing Style Skill for Claude

A Claude skill that strips the most common AI tells out of your writing. The kind of tells that make a reader stop mid-paragraph and think "a robot wrote this."

## Why this exists

In 2025, researchers at UMD and UMass ran a study called "People who frequently use ChatGPT for writing tasks are accurate and robust detectors of AI-generated text" (Russell, Karpinska & Iyyer, arXiv:2501.15654). They paid five experienced LLM users to read 300 articles and label each one as human or AI. The group got 299 out of 300 right. Zero false positives. They beat almost every commercial AI detector on the market, including on text that had been paraphrased and "humanized" specifically to fool them.

The researchers also documented exactly what gave the AI text away. This skill turns those findings into rules Claude follows when it writes for you.

The first 10 rules came from years of hands-on content work and pattern spotting. Rules 11 through 18 were added straight from the study's published findings, including the full "AI vocabulary" list the expert detectors kept flagging.

## What it covers

Structural habits like the rule of three, formulaic transitions, and hypophora. Banned vocabulary (delve, tapestry, crucial, testament, and about 80 friends). Attribution verbs, because humans just write "says" and AI can't stop writing "notes" and "emphasizes." Quote homogeneity, too-perfect grammar, safe and opinion-free content, relentlessly positive tone, generic intros, invented experts named Dr. Sarah Thompson, and yes, em dashes.

## Install in Claude.ai

You need a Pro plan or above with code execution turned on (Settings > Capabilities).

1. Download `anti-ai-writing-style.zip` from this repo
2. In Claude, go to Customize > Skills
3. Click the + button and choose Upload a Skill
4. Upload the zip and toggle it on

Claude will apply it automatically when you ask for written content. If it doesn't trigger, say "use my anti-ai-writing-style skill for this."

## Install in Claude Code

Copy the `anti-ai-writing-style` folder into `~/.claude/skills/` for use across all projects, or into `.claude/skills/` inside a specific repo to share it with everyone working in that codebase. No zip needed.

## Repo contents

```
anti-ai-writing-style/
  SKILL.md               The skill itself
anti-ai-writing-style.zip  Ready to upload to Claude.ai
README.md                  You are here
```

## Who made this

Hi, I'm AMA (Ann Marie Almariei). Partner & Creative Orchestrator at [Sageworx](https://www.sageworx.com/members/ann-marie-almariei), 20+ years in creative and content strategy, currently building with AI every day. I made this skill because I write a lot of content for myself and clients and refuse to ship copy that sounds like a robot.

- Website: [workwithAMA.io](https://www.workwithama.io)
- X: [@amalmariei](https://x.com/amalmariei)
- LinkedIn: [Ann Marie Almariei](https://www.linkedin.com/in/annmariealmariei/)

## Credit

Research basis: Jenna Russell, Marzena Karpinska, and Mohit Iyyer (2025), arXiv:2501.15654. Their annotated dataset and detection guide are at github.com/jenna-russell/human_detectors.

Feel free to fork it, adapt it, or add your own rules. If you find a new AI tell in the wild, that's rule 19 waiting to happen.
