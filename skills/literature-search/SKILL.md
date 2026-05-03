---
name: literature-search
description: Use when the user wants to find academic literature, build a keyword strategy, compare papers, identify seminal or recent sources, or create a reading list for a research topic. Useful for assignment preparation, literature review scoping, and evidence gathering across databases such as Google Scholar, Crossref, Semantic Scholar, library search, and publisher sites.
---

# Literature Search

Help the user find relevant academic sources quickly, then narrow to the most useful papers for the task.

## What To Do

1. Clarify the research target from the user's request.
2. Extract the topic, population or context, method, time window, and any constraints such as peer-reviewed only or recent papers only.
3. Build a search strategy with:
   - core concepts
   - synonyms and related terms
   - narrower and broader variants
   - optional exclusion terms
4. Search in a sensible order:
   - Google Scholar for broad discovery
   - Crossref or Semantic Scholar for metadata and citation trails
   - library databases or publisher pages when the user needs high-quality full text
5. Prioritize sources that are:
   - directly relevant to the user's question
   - well-cited or clearly influential
   - recent enough for the topic
   - methodologically credible
6. Return a short, useful result instead of a huge dump.

## Output Format

When the user asks to find literature, usually return:

- a one-sentence topic framing
- a suggested search string or a few search strings
- 5 to 10 recommended papers or sources
- for each source:
  - full title
  - year
  - authors if easy to obtain
  - why it matters in one sentence
  - link if available
- a short note on how to narrow or expand the search next

## Search Heuristics

- Start broad, then narrow.
- If the topic is vague, propose 2 to 3 search directions instead of forcing one interpretation.
- For fast-moving topics, favor recent review papers and the last 3 to 5 years of literature.
- For foundational theory, include seminal older papers.
- Prefer review articles first when the user is unfamiliar with the field.
- If the user is writing an assignment, optimize for usable sources they can read and cite, not maximum volume.

## Quality Checks

Before presenting results, sanity-check:

- Is each source actually about the user's topic?
- Is the set balanced between foundational and recent work when appropriate?
- Are there duplicates, near-duplicates, or irrelevant citation bait papers?
- If access looks limited, mention open-access alternatives.

## Boundaries

- Do not invent papers, authors, journals, or findings.
- If a citation is uncertain, label it as approximate and suggest verification.
- If browsing or database access is unavailable, still help by producing strong search strings, database suggestions, and screening criteria.

## Helpful Response Patterns

For a broad request:
"Here are three keyword directions you can try, with the most promising one first."

For a narrow request:
"I found a small cluster of papers focused on your exact question; start with these three."

For an assignment:
"If your goal is to build a literature review section, read the review paper first, then add two recent empirical studies and one foundational source."
