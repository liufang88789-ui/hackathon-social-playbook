# hackathon-social-playbook

AI agent skill that generates personalized X (Twitter) social strategies for hackathon projects.

## What it does

After you submit your hackathon project, this skill studies how breakout projects from past Colosseum hackathons built their X presence — what narrative angles worked, what content formats got traction, which spaces and AMAs drove real visibility — and turns those patterns into a personalized, actionable content plan for your project.

## Usage

```bash
npx skills add https://github.com/fang-liu62789/hackathon-social-playbook --skill hackathon-social-playbook
```

## Skill Structure

- `skills/hackathon-social-playbook/SKILL.md` — Core skill definition
- `knowledge/breakout-patterns.md` — Research on what worked
- `templates/content-plan.md` — Content plan template

## Inputs

- `project_name` — Name of the project
- `project_description` — What it does (1-2 sentences)
- `target_users` — Who it's built for
- `tech_stack` — Main technologies
- `team_background` — Team experience (optional)
- `submission_url` — URL of the project listing

## Outputs

- `core_story_angle` — The single most compelling narrative hook
- `content_plan_weeks_1_4` — Day-by-day 4-week content plan
- `recommended_hashtags` — Strategic hashtag recommendations
- `engagement_tactics` — Specific actions to build X presence
- `thread_templates` — Ready-to-use thread structures
