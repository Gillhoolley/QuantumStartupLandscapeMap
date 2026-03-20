# Quantum Startups Landscape Map

## Overview
This project contains the research dataset and supporting documentation for an interactive global map of quantum startups.

All project assets are maintained in Markdown for portability and easy review.

## Project Goals
- Track quantum startups across major global regions.
- Normalize startup metadata for map visualization and filtering.
- Provide analysis on regional clusters, investment trends, and funding momentum.

## Dataset Schema (Logical)
Each startup record tracks:

- `name`
- `country`
- `city`
- `region`
- `continent`
- `year_founded`
- `status`
- `specialty`
- `technology_modality`
- `technology_focus`
- `notable_breakthroughs`
- `funding_rounds`
- `website`
- `short_profile`

## File Layout (Markdown-Only)
- `data/startups.v2.md`: Canonical startup dataset.
- `data/startups.v2.enriched.md`: Enriched map-ready dataset.
- `analysis/regional_clusters.md`: Regional innovation cluster summary.
- `analysis/investment_trends.md`: Investment trend analysis.
- `analysis/fastest_growing_top10.md`: Funding momentum ranking methodology + results.
- `sources/sources.md`: Source links and verification notes.
- `INDEX.md`: Repository navigation index.

## Data Quality Rules
- Leave unknown fields empty, do not guess.
- Prefer official company/investor/government sources.
- Timestamp updates and refresh cycles.

## Update Workflow
1. Add or update startup records in `data/startups.v2.md`.
2. Sync normalized fields in `data/startups.v2.enriched.md`.
3. Refresh analysis documents in `analysis/`.
4. Log sources in `sources/sources.md`.
5. Update `INDEX.md` if structure changes.

## Current Status
- Markdown scaffold created.
- Core data, analysis, and source templates in place.
