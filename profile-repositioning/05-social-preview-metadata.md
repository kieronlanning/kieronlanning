# Consistent metadata descriptions for social previews

**Deliverable 5.** A consistent set of `description` / `og:description` / `twitter:description` values. The current Purview-Dev site metadata was inspected and is already aligned with the new positioning — no KJL.dev or consultancy references exist in the site source (`src/`). These descriptions form one coherent set across the personal profile and the Purview-Dev site.

## Personal GitHub profile

| Field | Value |
| --- | --- |
| Title | Kieron Lanning — Purview-Dev |
| Description | Software engineer and application architect. Creator and maintainer of Purview-Dev, building open-source .NET tools that remove friction from software development. |

## Purview-Dev site (site-wide default — `src/lib/site.ts`, `SITE.description`)

Keep as-is (already consistent):

> Purview Dev builds developer tooling for .NET: event sourcing, telemetry, validation, source generators, and build automation — designed to be fast, typed, and painless to adopt.

## Home page (`src/pages/index.astro`)

Title: `{SITE.orgName} — .NET developer tooling by Purview`
Description: `SITE.description` (site-wide default above).

## About page (`src/pages/about.astro`)

Title: `About — {SITE.fullName}`
Description (keep as-is):

> About Purview Development, the people and principles behind the Purview-Dev .NET tooling family.

Optionally extend once the creator section is added:

> About Purview Development, the people and principles behind the Purview-Dev .NET tooling family — built by Kieron Lanning.

## Projects catalogue (`src/pages/projects/index.astro`)

Title: `Projects — {SITE.fullName}`
Description (keep as-is):

> The Purview-Dev product family: event sourcing, telemetry, validation, source generators, and build automation for .NET.

## Project detail pages (`src/pages/projects/[project].astro`)

Title: `{project.name} — {SITE.fullName}`
Description: `project.shortDescription` (pulled from the typed catalogue; already purposeful and KJL-free).

## Consistency rules applied

- Every description names real Purview capabilities (telemetry, event sourcing, validation, source generators, build automation).
- No "consultancy", "digital delivery", "KJL", or personal-brand sales language anywhere.
- The personal profile describes the person and why; the site describes the tools and how to adopt them.