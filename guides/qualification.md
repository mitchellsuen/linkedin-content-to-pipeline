# Qualify the people engaging with your content

[Back to LinkedIn Content to Pipeline](../README.md) · [Next: conversations](dm-conversion.md)

The first useful output is a short list of people who fit your buyer criteria, with reasons you can inspect. Keep company fit and the person's current remit separate. A highly engaged person at the wrong company should not pass.

## 1. Collect the engagers

Export the people who reacted to or commented on your recent posts from the LinkedIn tool you already use, into a spreadsheet or table. Start with your own profile. Add other relevant public profiles only when that audience is useful to your ICP.

Keep one row per person, with:

| Evidence | What it holds |
|---|---|
| Person | Name, LinkedIn URL, headline, current role |
| Current company | Employer name, LinkedIn/company URL, industry, size, location |
| Source profiles | The profile(s) whose posts they engaged with |
| Source posts | The post URL(s) they engaged with |
| Engagement types | Reaction, comment (and the comment text, if available) |

Keep the profile and source-post evidence on the same person. Do not transfer one employee's engagement to another employee at their company. A like is an observed signal, not proof of buying intent. Missing employer data stays unknown.

## 2. Write your rubric

Copy [the blank rubric](../templates/icp-rubric.md) into `company/private/` and fill it using your own ICP, offer and exclusions. Define company criteria, person criteria, pass thresholds and evidence you consider mandatory. Make the points add to 100 independently for company and person.

The kit's [company example](../company/icp.example.md) and [persona example](../company/persona.example.md) show the level of detail. They are synthetic examples, not recommended criteria for every reader.

## 3. Map your columns to the prompt

Copy [the prompt](../templates/qualification-prompt.md) into `company/private/linkedin-qualification.md` and replace its rubric block with the criteria from step 2. The prompt has four evidence placeholders: `{{profile_data}}`, `{{company_data}}`, `{{source_profile_urls}}` and `{{source_post_urls}}`. Bind each one to the matching column(s) in your export; your tool's column names will differ.

Review employment and enrichment state. Missing or unresolved fields should produce a review decision, not an invented company size, job responsibility or purchase intent. A company name alone is not enough to assume a domain or identity match.

The prompt reads existing evidence; it performs no new web research and should not invent missing facts. Its answer follows the [structured output schema](../templates/qualification-output.schema.json): company/persona scores, independent disqualifiers, a fit status, reasons, missing evidence and evidence used. **Qualified means passes the rubric; it does not mean approved for outreach.**

## 4. Score one row, then calibrate

Run the prompt on one row you can assess yourself, either by asking your coding agent to apply it to that row of the export, or through an AI column in your spreadsheet or table tool. Check the output against your own judgment before scoring more.

Calibrate against a small reviewed set: a clear fit, a wrong-company case, a wrong-person case, and missing evidence. [Synthetic examples](../examples/qualification-decisions.json) show expected decisions; they are not model test results. Read the evidence behind each score and adjust the rubric before expanding.

Keep three views or filters: **Qualified**, **Review**, **Not fit**. Both scores must meet your thresholds; both disqualification flags must explicitly be false; mandatory evidence must be present. Keep engagement/recency separately for prioritization after fit. Never use an engagement bonus to rescue a failed fit gate.

## 5. Make it repeatable when the first batch works

Manual bounded batches are enough to start. When you score new engagers regularly, keep the same prompt and rubric file, cap the spend of each batch, and only score rows whose required evidence has arrived. Review existing output before re-scoring; changing the rubric does not automatically recalibrate old results.

Hand off only a reviewed cohort to [the DM framework](dm-conversion.md). This guide configures qualification, not automatic enrollment or messaging.
