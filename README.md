# SimEx Skills: Install and Use Guide

This guide covers the two SimEx skills the team uses to draft simulation exercises for design sprints: **simex-prototype** (for exercises that test a built dashboard, alert system, or other information product) and **simex-scenario** (for purely theoretical, narrative exercises with no prototype involved). Use whichever matches the exercise you're building.

## 1. Installing a skill

Each person adds the skill to their own Claude account. There are two ways to get it, depending on how your team's account is set up.

**If your organisation has added the skill centrally** (Team/Enterprise plans, set up by an org owner): it will already appear in your available skills automatically. Nothing to install, skip to section 2.

**Otherwise, install it yourself from the shared file:**

1. Get the SKILL.md file for the skill you need (shared by whoever set this up, or downloaded from the review card in claude.ai).
2. In claude.ai, go to Settings > Capabilities > Skills.
3. Click Create skill (or Upload), and upload the SKILL.md file.
4. Save. The skill now appears in your account and triggers automatically when relevant.

Note: creating or uploading custom skills requires code execution to be enabled on your account, and is available on Pro, Max, Team, and Enterprise plans.

If you're on a Team or Enterprise plan and want this available to the whole team at once rather than person by person, ask your organisation owner to add it under the organisation's admin settings instead.

## 2. Which skill to use

| Your exercise... | Use |
| --- | --- |
| Tests an actual dashboard, alert, report, or other prototype built in the sprint | simex-prototype |
| Is a theoretical situation or decision-making trade-off, with no built tool involved | simex-scenario |

You don't need to invoke the skill by name, just ask Claude to draft a simex and describe what you have (a prototype to test, or a decision-making situation to explore), and the right skill triggers on its own. Naming it directly also works, e.g. "use simex-prototype to draft an exercise for the malaria dashboard sprint."

## 3. Using simex-prototype

Start by telling Claude you need a simex for a prototype, and give it what you already know. Claude asks for anything missing before drafting. Have this ready:

- Sprint/programme name and topic, e.g. "PHISMS Design Sprint, malaria"
- Target role and persona: who the participant plays (e.g. "district surveillance officer in District A"), and any constraint on their authority or access worth building in (no channel to a superior, not a clinician, etc.)
- The decision-making need or sprint challenge: the "how might we" question the prototype is meant to answer
- The prototype content itself: screenshots, mock data, alert text, or a description of what the dashboard shows, in the order a user would encounter it
- Roughly how many steps you want, given a 60-90 minute target (there's no fixed number)

Claude drafts the full exercise directly in the chat: header, instructions, the decision-making need, scene-setting, each step with its prototype content and questions, and a closing debrief step. Review it there and ask for changes (add a step, adjust the role, change the tone) before it's final.

## 4. Using simex-scenario

Start by telling Claude you need a theoretical/scenario-based simex, and describe the judgement call you want to explore. Have this ready:

- Sprint/programme name and topic, if the exercise sits under a named sprint (not required, some scenario exercises stand alone)
- The judgement call or trade-off each scenario should force, e.g. act now vs. wait for confirmation, how to communicate uncertainty to leadership, how to prioritise across competing needs. This is the core of the exercise, so be specific.
- Whether there's a defined role and persona, or whether it should stay in plain "you" framing
- How many separate scenarios you want (three to six is typical), and whether they share a throughline or are unrelated
- Roughly how many prompts per scenario, given a 60-90 minute target overall

Claude drafts each scenario as a short narrative followed by a sequence of building prompts, plus a shared debrief at the end. Review and ask for changes in chat before it's final.

## 5. Getting a Word file

Both skills draft in the chat by default, so you can review and edit conversationally first. Once the content is finalised, just ask for a Word version ("turn this into a Word doc") and Claude exports it as a .docx matching the team's existing formatting conventions.

## 6. Updating the skills

If the standard changes, whoever maintains the skills updates the SKILL.md and re-shares it. Re-uploading a skill with the same name under Settings > Capabilities > Skills replaces the old version on your account.
