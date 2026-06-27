# Data Source and Method Notes

## Source

The public files in this repository are sanitized aggregate artifacts derived from an existing local BPCR research run under:

- Local source directory: `result/summary_20260426_172702/`
- Local generation time: `2026-04-26T17:31:02`
- Songs included: 10
- Anonymous comments included in the local aggregate: 69,975
- Political/historical related comments identified by the local pipeline: 7,609

## Processing Method

The local BPCR workflow used the following steps before this public release:

1. Collect related Bilibili music-video comments for selected ancient-style songs.
2. Clean comment text by removing URLs, user mentions, emoji markers, and excessive whitespace.
3. Anonymize user identifiers before research analysis.
4. Segment Chinese text and compute word frequency, TF-IDF, and keyword co-occurrence tables.
5. Use a four-axis political/historical semantic layer to identify potentially relevant comments.
6. Apply rule-based exclusions, manual lexicon overrides, and AI-assisted review for semantic cleaning.
7. Recode project-internal stance labels into broad course-paper categories: 建制派, 左派, 自由派, 民粹, and 娱乐化/未归类.
8. Publish only sanitized aggregate tables.

## Public Release Scope

This repository excludes:

- Raw comments
- User IDs, usernames, avatars, profile links, or other direct identifiers
- Cookies, API keys, or local configuration files
- Specific sensitive second-level labels that may contain concrete names or events

The uploaded data should be treated as exploratory course-paper material, not as a representative survey of Bilibili users or a definitive political classification system.
