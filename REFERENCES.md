---
updated: "2026-08-17"
---

# Phoenix House: Reference

## Line of Work

Staging the named phenomena of fire as **first-person entities**: each production
takes one mechanism — a fuel, a chemistry, a dynamic — and gives it a voice
(_„Ich bin…"_). The house does not model fires as events that befall a place; it
models each as an actor with its own conditions, its own way of feeding, and the
paradox by which the obvious way to fight it fails or feeds it. One entity, one
dominant mechanism.

### Staging Status

The cycle is planned at 52 entities across four domains — wildland and
ecological, enclosure and atmospheric, industrial and chemical, anthropogenic and
craft. Three have been published ahead of this house and are pending deposit.

- [x] **Zunderkind** — published (surface ignition)
- [x] **Moorleiche** — published (peat smoulder)
- [x] **Der Erdbäcker** — published (duff smoulder)
- [ ] **the remaining 49** — planned

## Origin

This house has no public-domain literary source. Its origin is the fire science
carried by the khai engines it declares, and through them the literature those
engines warrant.

| Source                       | Key Work / Event              | Scope                                                                                                |
| ---------------------------- | ----------------------------- | ---------------------------------------------------------------------------------------------------- |
| **khai `fire` engine**       | the burn regime of a place    | ignition, creep, conflagration, smoulder, exclusion, renewal — the modes a place's fire runs in      |
| **khai `combustion` engine** | the named phenomena of fire   | the catalogue: wildland, compartment, industrial, and made fires, each with its own fuel and paradox |
| **khai `blaze` composite**   | a fire read as its whole life | kindling, run, renewal — used where an entity lives an arc rather than a single mode                 |

Each engine carries its own `REFERENCES.md`; the scientific warrant for a
mechanism lives there, not here. This house cites the member, the member cites
the science.

## Restrictions

What the house refuses to model, and to whom it delegates.

- **Scientific authority**: The house refuses to claim fire-science authority
  beyond what its declared engines warrant. Where a production's mechanism is not
  carried by a member of `fire` or `combustion`, that is an engine gap to close in
  khai, not a detail to improvise here.
- **Anthropomorphism as decoration**: The voice is the entity's mechanism
  speaking, never a character wearing a fire as costume. What the entity can say
  is bounded by what its mechanism does.
- **Operational instruction**: The house refuses to read as firefighting or
  ignition guidance. Productions are literary; the paradoxes they stage are
  descriptive, never procedural.
- **Language Policy**: The house defines its own language policy regarding the
  staging prose and schema compatibility:
  - **English for Architecture & Schema**: structural headings, frontmatter keys,
    reference warrants (`REFERENCE.md` or `REFERENCES.md`), and the house identity
    (`README.md`) are written in English, for compatibility with the `khai`
    validation tooling.
  - **German for Prose & Staging**: entity voices, projections, actions, tells,
    and staging notes are written in German, the cycle's own language.

## Encoding

Source to constraint, per file.

- **the house ([README.md](README.md))**: The Estate identity that answers for the entire run.
- **the productions (`plays/`)**: The individual staging packages, each containing the play definition, personas, positions, pieces, places, processes, and plots.
- **the engines (`package.json` dependencies)**: The declared repertoire — `fire`, `combustion`, and `blaze` — from which every production casts its mechanism. A link without a declared dependency is a build error.
- **the gates (`tests/`, `khai-guard.config.json`)**: The conformance and governance checks ensuring that all plays comply with the canon.
