---
name: hackathon-social-playbook
description: >-
  Generate a personalized X (Twitter) social strategy and 4-week content plan for hackathon projects.
  Analyzes breakout patterns from past Colosseum hackathons and delivers actionable posting guidance.
---

# hackathon-social-playbook

## Goal

After a project is submitted to a hackathon, generate a personalized X (Twitter) social strategy that turns a quiet project listing into a recognized presence. Uses patterns from past breakout hackathon projects on Colosseum to advise on narrative angles, content formats, timing, and engagement tactics.

## Trigger Conditions

Use this skill when:
- A hackathon project has been submitted and the listing is live
- The project needs an X presence strategy but the team has no social media background
- The hackathon deadline is still 7+ days away
- Invoked during the post-submission social ramp-up phase

## Inputs

| Input | Type | Required | Description |
|---|---|---|---|
| `project_name` | string | Yes | Name of the project |
| `project_description` | string | Yes | What the project does in 1-2 sentences |
| `target_users` | string | Yes | Who the project is built for |
| `tech_stack` | string | Yes | Main technologies used |
| `team_background` | string | No | Team's relevant experience or background |
| `hackathon_track` | string | No | Which track/submission category |
| `submission_url` | string | Yes | URL of the project listing |

## Outputs

| Output | Description |
|---|---|
| `core_story_angle` | The single most compelling narrative hook for this project |
| `content_plan_weeks_1_4` | Day-by-day content plan for 4 weeks |
| `recommended_hashtags` | Hashtags to use and why |
| `engagement_tactics` | Specific actions to build followers and drive engagement |
| `posting_schedule` | Optimal posting times and frequency |
| `thread_templates` | Ready-to-use thread structures |

## Rules

1. The `core_story_angle` must be something the team can authentically own — do not invent narratives.
2. Content plan must be executable by a non-marketer team with no social media experience.
3. Every week must include at least one thread (3-7 tweets) as the engagement anchor.
4. Hashtags must include at least one broad (#Solana, #DeFi) and one niche track tag.
5. Do not recommend posting more than 2x per day — quality over quantity.
6. Engagement tactics must include specific accounts to interact with, not generic advice.
7. The posting schedule must account for the 24 hours before hackathon judging as peak intensity window.

## Output Format

```yaml
core_story_angle: "<one compelling sentence that anchors all social presence>"

key_narrative_tensions:
  - "<tension 1: e.g., 'built this in 48 hours with no sleep'>"
  - "<tension 2: e.g., 'why we chose to build on-chain instead of centralized'>"

recommended_hashtags:
  - tag: "<hashtag>"
    reason: "<why this tag drives reach for this project>"

posting_schedule:
  peak_times:
    - "<UTC window, e.g., 14:00-18:00 UTC>"
  daily_frequency: "<1 or 2>"
  thread_frequency: "<2-3x per week>"

content_plan_weeks_1_4:
  week_1:
    theme: "<theme name>"
    daily_posts:
      - day: 1
        content_type: "<tweet/thread/reply/space>"
        topic: "<what to post about>"
        template: "<ready-to-use starting text>"
      - day: 2
        content_type: "<tweet/thread/reply/space>"
        topic: "<what to post about>"
        template: "<ready-to-use starting text>"
      - day: 3
        content_type: "<tweet/thread/reply/space>"
        topic: "<what to post about>"
        template: "<ready-to-use starting text>"
      - day: 4
        content_type: "<tweet/thread/reply/space>"
        topic: "<what to post about>"
        template: "<ready-to-use starting text>"
      - day: 5
        content_type: "<tweet/thread/reply/space>"
        topic: "<what to post about>"
        template: "<ready-to-use starting text>"
      - day: 6
        content_type: "<tweet/thread/reply/space>"
        topic: "<what to post about>"
        template: "<ready-to-use starting text>"
      - day: 7
        content_type: "<tweet/thread/reply/space>"
        topic: "<what to post about>"
        template: "<ready-to-use starting text>"
  week_2:
    theme: "<theme name>"
    daily_posts:
      - day: 8
        content_type: "<tweet/thread/reply/space>"
        topic: "<what to post about>"
        template: "<ready-to-use starting text>"
      - day: 9
        content_type: "<tweet/thread/reply/space>"
        topic: "<what to post about>"
        template: "<ready-to-use starting text>"
      - day: 10
        content_type: "<tweet/thread/reply/space>"
        topic: "<what to post about>"
        template: "<ready-to-use starting text>"
      - day: 11
        content_type: "<tweet/thread/reply/space>"
        topic: "<what to post about>"
        template: "<ready-to-use starting text>"
      - day: 12
        content_type: "<tweet/thread/reply/space>"
        topic: "<what to post about>"
        template: "<ready-to-use starting text>"
      - day: 13
        content_type: "<tweet/thread/reply/space>"
        topic: "<what to post about>"
        template: "<ready-to-use starting text>"
      - day: 14
        content_type: "<tweet/thread/reply/space>"
        topic: "<what to post about>"
        template: "<ready-to-use starting text>"
  week_3:
    theme: "<theme name>"
    daily_posts:
      - day: 15
        content_type: "<tweet/thread/reply/space>"
        topic: "<what to post about>"
        template: "<ready-to-use starting text>"
      - day: 16
        content_type: "<tweet/thread/reply/space>"
        topic: "<what to post about>"
        template: "<ready-to-use starting text>"
      - day: 17
        content_type: "<tweet/thread/reply/space>"
        topic: "<what to post about>"
        template: "<ready-to-use starting text>"
      - day: 18
        content_type: "<tweet/thread/reply/space>"
        topic: "<what to post about>"
        template: "<ready-to-use starting text>"
      - day: 19
        content_type: "<tweet/thread/reply/space>"
        topic: "<what to post about>"
        template: "<ready-to-use starting text>"
      - day: 20
        content_type: "<tweet/thread/reply/space>"
        topic: "<what to post about>"
        template: "<ready-to-use starting text>"
      - day: 21
        content_type: "<tweet/thread/reply/space>"
        topic: "<what to post about>"
        template: "<ready-to-use starting text>"
  week_4:
    theme: "<theme name>"
    daily_posts:
      - day: 22
        content_type: "<tweet/thread/reply/space>"
        topic: "<what to post about>"
        template: "<ready-to-use starting text>"
      - day: 23
        content_type: "<tweet/thread/reply/space>"
        topic: "<what to post about>"
        template: "<ready-to-use starting text>"
      - day: 24
        content_type: "<tweet/thread/reply/space>"
        topic: "<what to post about>"
        template: "<ready-to-use starting text>"
      - day: 25
        content_type: "<tweet/thread/reply/space>"
        topic: "<what to post about>"
        template: "<ready-to-use starting text>"
      - day: 26
        content_type: "<tweet/thread/reply/space>"
        topic: "<what to post about>"
        template: "<ready-to-use starting text>"
      - day: 27
        content_type: "<tweet/thread/reply/space>"
        topic: "<what to post about>"
        template: "<ready-to-use starting text>"
      - day: 28
        content_type: "<tweet/thread/reply/space>"
        topic: "<what to post about>"
        template: "<ready-to-use starting text>"

engagement_tactics:
  - tactic: "<name of tactic>"
    action: "<specific action: who to reply to, what to say, which spaces to join>"
    frequency: "<daily/weekly>"
  - tactic: "<name of tactic>"
    action: "<specific action>"
    frequency: "<daily/weekly>"

thread_templates:
  - name: "<template name>"
    tweets: <number>
    structure:
      - tweet: 1
        content: "<opening tweet text>"
      - tweet: 2
        content: "<second tweet text>"
    best_for: "<when to use this template>"
```

## Example

**Input:**
```yaml
project_name: "SolSearch"
project_description: "AI-powered Solana token discovery tool that surfaces gems before they pump"
target_users: "Retail Solana traders and degen investors"
tech_stack: "Next.js, Rust, Solana SDK, OpenAI"
team_background: "Two ex-DeFi researchers who met at college"
hackathon_track: "DeFi / Infrastructure"
submission_url: "https://colosseum.io/project/solsearch"
```

**Output:**
```yaml
core_story_angle: "We spent 6 months analyzing what makes Solana tokens pump — now we're giving retail traders the same edge that whales have."

key_narrative_tensions:
  - "Insider knowledge democratized: what if retail could see what whales see?"
  - "Built by degen researchers, for degens: we're not VCs, we're your fellow traders"

recommended_hashtags:
  - tag: "#Solana"
    reason: "Broad reach to all Solana ecosystem participants"
  - tag: "#DeFi"
    reason: "Connects to DeFi power users most likely to try the tool"
  - tag: "#memecoin"
    reason: "High-engagement topic that drives algorithmic reach"
  - tag: "#Colosseum"
    reason: "Required for hackathon visibility"

posting_schedule:
  peak_times:
    - "14:00-18:00 UTC (US morning/afternoon overlap)"
  daily_frequency: 1
  thread_frequency: 3

content_plan_weeks_1_4:
  week_1:
    theme: "Building in Public"
    daily_posts:
      - day: 1
        content_type: "thread"
        topic: "Project intro + why Solana token discovery is broken"
        template: "We just submitted our hackathon project. It's called SolSearch — and it finds Solana gems before they pump. 🧵👇"
      - day: 2
        content_type: "tweet"
        topic: "The problem we're solving"
        template: "Right now, finding the next 100x Solana token means either: 1) Paying for alpha groups 2) Spending 12 hours/day on DexScreener 3) Getting lucky. We're fixing that."
      - day: 3
        content_type: "tweet"
        topic: "Technical approach"
        template: "Hot take: most Solana token analysis tools are just charts with extra steps. Real alpha comes from on-chain behavior patterns. Here's what we looked at instead 👇"
      - day: 4
        content_type: "reply"
        topic: "Engage with DeFi Twitter"
        template: "Reply substantively to tweets from popular DeFi accounts with genuine insights about Solana token mechanics"
      - day: 5
        content_type: "tweet"
        topic: "Progress update"
        template: "Day 5 of #Colosseum. SolSearch can now scan wallet behavior patterns in real-time. The data we're seeing is wild. Thread incoming..."
      - day: 6
        content_type: "thread"
        topic: "First demo teaser"
        template: "We said we'd find gems. Here it is in action. 🧵 Showed SolSearch to 3 friends — all of them found something they hadn't seen before. That's the whole point."
      - day: 7
        content_type: "tweet"
        topic: "Week 1 recap"
        template: "1 week, 1 hackathon submission, and we're just getting started. SolSearch is real. Week 2 = integration + testing. 🚀"
  week_2:
    theme: "Building Credibility"
    daily_posts:
      - day: 8
        content_type: "thread"
        topic: "Thread on methodology"
        template: "How does SolSearch actually find tokens before they pump? We analyzed 200+ tokens over 3 months. Here's what the data says 🧵"
      - day: 9
        content_type: "tweet"
        topic: "Hot take on current market"
        template: "The average Solana trader spends 3 hours/day on DexScreener. That's 90 hours/month watching charts. What if you could automate that?"
      - day: 10
        content_type: "tweet"
        topic: "Team story"
        template: "We met in a DeFi research group 2 years ago. Spent months arguing about tokenomics. Now we're building the tool we always wished existed."
      - day: 11
        content_type: "tweet"
        topic: "Progress update"
        template: "SolSearch v0.2 is live. Added wallet clustering analysis. The patterns we're finding are wild — some wallets have been accumulating the same token for 6 months straight."
      - day: 12
        content_type: "tweet"
        topic: "Engagement"
        template: "Drop your wallet below and I'll show you what SolSearch found for your交易历史. No promises, just data. 👇"
      - day: 13
        content_type: "tweet"
        topic: "AMA-style"
        template: "We're live for the next hour. Ask us anything about Solana token analysis, our methodology, or why we chose this problem. Go."
      - day: 14
        content_type: "tweet"
        topic: "Week 2 recap"
        template: "Week 2 down. SolSearch has analyzed 1,847 wallets and found 23 tokens with unusual accumulation patterns. 3 of them did 5x last week. This is working."
  week_3:
    theme: "User Traction"
    daily_posts:
      - day: 15
        content_type: "tweet"
        topic: "Feature announcement"
        template: "Just added Telegram alerts to SolSearch. Get notified when a wallet you've been watching makes a move. Finally, alpha that finds you."
      - day: 16
        content_type: "tweet"
        topic: "User feedback"
        template: "A trader DMed us: 'I used SolSearch for 3 days and found a 4x before it moved.' This is why we're building this. 🚀"
      - day: 17
        content_type: "space"
        topic: "AMA on Colosseum space"
        template: "Join us in the @ColosseumDAO space to talk about what we're building and answer questions about our methodology."
      - day: 18
        content_type: "tweet"
        topic: "Technical deep dive"
        template: "The clustering algorithm is the core of SolSearch. Here's how it works: we group wallets by behavior, not just holdings. Thread 🧵"
      - day: 19
        content_type: "tweet"
        topic: "Progress update"
        template: "Day 12 of Colosseum. SolSearch now tracks 5,000+ wallets in real-time. We're seeing patterns that traditional metrics completely miss."
      - day: 20
        content_type: "tweet"
        topic: "Hot take"
        template: "Unpopular opinion: most on-chain analytics tools are built for VCs, not traders. They show you what already happened. SolSearch shows you what's about to happen."
      - day: 21
        content_type: "tweet"
        topic: "Week 3 recap"
        template: "3 weeks in. 127 users signed up. One whale just followed our wallet tracker. We're officially on someone's radar. Week 4 = final push."
  week_4:
    theme: "Final Push"
    daily_posts:
      - day: 22
        content_type: "thread"
        topic: "Final product thread"
        template: "SolSearch is done. Here's everything you need to know before #Colosseum judging. What we built, how it works, and why it matters. 🧵 #Solana #DeFi"
      - day: 23
        content_type: "tweet"
        topic: "Team demo"
        template: "Quick demo of SolSearch in action: we picked a random wallet, ran it through our system, and found something interesting within 30 seconds. 🎯"
      - day: 24
        content_type: "tweet"
        topic: "Reflection"
        template: "Built SolSearch in 4 weeks with 2 people. Learned more about Solana's data layer than I thought possible. Whatever happens tomorrow, this was worth it."
      - day: 25
        content_type: "tweet"
        topic: "Last call"
        template: "48 hours until #Colosseum judging. If you've been sleeping on SolSearch — now's the time. Link in bio. We're not going anywhere after the hackathon."
      - day: 26
        content_type: "tweet"
        topic: "Thank you thread"
        template: "Thank you to everyone who gave us feedback, shared our posts, and helped us debug at 2am. You know who you are. 🧵"
      - day: 27
        content_type: "tweet"
        topic: "Final countdown"
        template: "Tomorrow we find out. SolSearch is live. The data is real. We've done everything we can. See you on the other side."
      - day: 28
        content_type: "tweet"
        topic: "Results"
        template: "Whatever happens — we shipped. We built something real. And we learned that building in public is the best way to build. Thanks for coming along."

engagement_tactics:
  - tactic: "DeFi influencer engagement"
    action: "Reply substantively to tweets from @aeyakovenko, @jumptrampvines, @stepp01 with genuine insights about Solana token mechanics"
    frequency: daily
  - tactic: "Colosseum participant network"
    action: "Engage with 5 other Colosseum hackathon participants daily — genuine interaction, not spam"
    frequency: daily
  - tactic: "Spaces participation"
    action: "Join all #Solana and #Colosseum Spaces in the final week. Speak if possible. Share takeaways in a tweet thread."
    frequency: weekly

thread_templates:
  - name: "Project Introduction"
    tweets: 5
    structure:
      - tweet: 1
        content: "We just submitted to #Colosseum. It's called [PROJECT]. Let us explain why it exists. 🧵"
      - tweet: 2
        content: "The problem: [specific problem statement with data if possible]"
      - tweet: 3
        content: "Our approach: [how the project solves it, with technical nuance]"
      - tweet: 4
        content: "What surprised us while building: [vulnerability angle]"
      - tweet: 5
        content: "Try it here: [link]. We're still building — feedback welcome. 🚀"
    best_for: "Day 1 of social ramp-up"
  - name: "Final Demo Thread"
    tweets: 7
    structure:
      - tweet: 1
        content: "[PROJECT] is complete. Here's what we built and why it matters. 🧵 #Colosseum #Solana"
      - tweet: 2
        content: "The problem we solved: [1-2 sentences on the pain point]"
      - tweet: 3
        content: "How it works: [technical overview in simple terms]"
      - tweet: 4
        content: "The 'wow' moment: [the most impressive feature or result]"
      - tweet: 5
        content: "What we learned building this: [honest reflection on the process]"
      - tweet: 6
        content: "What's next: [roadmap hint, creates anticipation]"
      - tweet: 7
        content: "Link in bio. Feedback welcome — we're shipping this for real. 🚀"
    best_for: "Final 48 hours before judging"
