# Dashboard

Public aggregate insights dashboard for Make AI Visible.

This repository owns the public-facing view of privacy-protected research findings. The MVP should make patterns visible without exposing individual contributors, conversations, schools, locations, or rare cohorts.

## MVP Scope

- Display aggregate counts and behavioral score distributions.
- Support cohort-level filters only when privacy thresholds are satisfied.
- Apply suppression and differential privacy noise before publication.
- Show methodology notes and data freshness metadata.
- Avoid individual-level records, quotes, or small-cell drilldowns.

## Privacy Boundary

The dashboard must only consume aggregate, publication-approved data. No raw conversations, anonymized full transcripts, or reviewer-only records should be shipped to the client.

## Suggested Stack

- React or Next.js with TypeScript.
- Static aggregate JSON or a read-only API.
- Charting library with accessible labels.
- Automated checks for minimum cohort sizes.

## First Milestone

Build a static dashboard using synthetic aggregate data, including suppression rules for cohorts below the publication threshold.
