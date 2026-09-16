# Purview-Dev About page — creator section

**Deliverable 4.** Add an understated creator section to the Purview-Dev About page (`src/pages/about.astro`). Keep it secondary to the organisation and its projects — one short section, placed after the "Release process" section and before "Licensing".

## Prose / copy

### Built to remove friction

Purview-Dev was created by [Kieron Lanning](https://github.com/kieronlanning), a software engineer and application architect focused on developer experience and modern .NET tooling.

It grew from a recurring observation: engineering teams repeatedly lose time solving the same setup, integration, and delivery problems. Purview packages those lessons into open-source tools designed to make good practices easier to adopt.

## Ready-to-paste Astro snippet

Insert the following `<section>` into `src/pages/about.astro` inside the left-hand content column (the `<div class="min-w-0 space-y-10">` block), e.g. between the "Release process" and "Licensing" sections:

```astro
<section>
  <h2 class="text-xl font-semibold">Built to remove friction</h2>
  <p class="mt-4 leading-relaxed text-muted">
    Purview-Dev was created by{' '}
    <a
      href="https://github.com/kieronlanning"
      class="pv-link"
      rel="noopener noreferrer"
      target="_blank"
    >
      Kieron Lanning
    </a>
    , a software engineer and application architect focused on developer
    experience and modern .NET tooling.
  </p>
  <p class="mt-4 leading-relaxed text-muted">
    It grew from a recurring observation: engineering teams repeatedly lose
    time solving the same setup, integration, and delivery problems. Purview
    packages those lessons into open-source tools designed to make good
    practices easier to adopt.
  </p>
</section>
```

Notes:

- Links Kieron's name to `https://github.com/kieronlanning` as required.
- Uses existing site styling (`pv-link`, `text-muted`, `leading-relaxed`) consistent with the other sections on the page.
- The section is organisation-first: it explains the origin of the tools, not a personal portfolio.