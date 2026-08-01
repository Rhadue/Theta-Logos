# Changelog

All notable changes to θ-Logos will be documented in this file.

---

## [1.2] - 2026-08-01

### Fixed

- **The repository landing page was empty.** `README.md` had been deleted, leaving
  only `README_v1.1.md`. GitHub renders only a file named exactly `README.md`, so
  a visitor saw a bare file list and none of the documentation. Restored by
  renaming.
- **Eight of nine internal links were broken.** Documents pointed at
  `theta_logos_core_v1.1.md`, `EXAMPLES.md` and `README.md` while the files on
  disk were `theta_logos_core.md`, `EXAMPLES_v1.1.md` and nothing. Every entry
  point into the specification returned 404.

### Changed

- **Version numbers removed from filenames.** They were the root cause of the
  broken links: with the version in the name, every release requires rewriting
  every link in every document, and one missed rename breaks navigation silently.
  The version now lives in each document's header and in the git tag, where it
  can change without touching anything else.

  | Was | Now |
  | --- | --- |
  | `README_v1.1.md` | `README.md` |
  | `EXAMPLES_v1.1.md` | `EXAMPLES.md` |

- **`LICENSE` replaced with the complete, unmodified CC BY-SA 4.0 text.** The
  previous file stopped after Section 7; Section 8 (Interpretation), which carries
  the severability and construction terms, was absent entirely. An abridged licence
  is not the licence it names, and the file closed with a link to the real text
  rather than containing it.
- **The copyright holder is now named.** Nobody was identified anywhere in the
  file. Under an *Attribution* licence that is not a formality — the central
  condition cannot be met if there is no one to attribute. A header now names the
  holder and gives the exact attribution string to use.

  `LICENSE` holds the canonical text and nothing else; the copyright notice and
  attribution string live in the README instead. That is Creative Commons' own
  guidance — the legal code stays unmodified and the notice is applied to the
  work — and it is also what lets GitHub recognise the licence, since detection
  compares the file against the canonical text from the first byte.

### Added

- **`¬` — negation (symbol #9).** `¬∃[X]` states that X does not exist, or has
  ceased to. Versions 1.0 and 1.1 offered no way to express cessation at all,
  which left elementary transformations inexpressible: burning, dissolution,
  death. `¬` applies to `∃` and `∈`, and not to `→`, `θ`, or emotional states.

  The gap was found empirically rather than by review. In a multi-model session on
  the sentence *"a paper burns to ash"*, four models with different architectures
  each introduced `¬` unprompted, no such symbol being available to them.
  Independent convergence on the same character is why it was adopted in this form
  rather than another, and the reasoning is recorded in the specification itself.

- **A definition of the colon.** `∃:`, `∈:`, `⊂:` and `θ:` appear 41 times across
  the specification, but the colon was never listed among the symbols or explained
  anywhere, leaving a reader unable to tell whether `∃` and `∃:` were the same
  operator. It is now documented as punctuation marking "this operator applies to
  what follows", with the note that `→` and `⊕` are infix and never take it.

### Changed

- **The core is 9 primitives, not 14.** The previous count included the six
  emotional states as symbols #9–#14, while also defining `θ` as accepting any
  label at all — so `θ_catalysis` and `θ_phase_change` were equally valid and
  counted as nothing. Either labels are symbols, in which case the core is
  unbounded and the "minimal core" claim fails, or they are not.

  They are now presented as what they are: a standard vocabulary of six
  conventional labels on symbol #8, listed because they recur and because they
  carry composition rules the general `θ_name` form does not. The core is seven
  structural operators, `θ`, and `¬`.

  The claim is stronger this way — nine primitives is a better argument for
  minimality than fourteen. Counts were updated across README, CONTRIBUTING and
  the specification; the v1.1 entry below correctly still says 14, being a record
  of what was true then.

---

## [1.1] - 2025-11-16

### Added
- **Explicit symbol numbering** (1-14) in Core Specification for clarity
- **Badge GitHub** in README for professional presentation
- **Before/After examples** in README demonstrating token compression
- **Validation disclaimer** clearly stating experimental status, not peer-reviewed
- **Emotional state rules** explicitly documented (no substructures, terminal nodes)
- **Mediation pattern** (⟨x⟩) clarified early in Core Specification
- **Common patterns section** separating core symbols from recommended extensions
- **Nuclear fission example** (conceptual) in EXAMPLES.md
- **Ultra-simple examples** for absolute beginners in EXAMPLES.md
- **Expanded bad vs good notation** section with 6 comparison examples
- **Extension development step-by-step** guide in EXAMPLES.md
- **CONTRIBUTING.md** with clear guidelines for community development
- **LICENSE** file (CC-BY-SA 4.0) for legal clarity
- **Poetic test example** in Core Specification validation section

### Changed
- **README reduced to 40%** of original length for better GitHub presentation
- **Core Specification restructured** with numbered symbols first
- **Validation section expanded** with honest limitations and scope
- **Examples reorganized** with beginner → advanced progression
- **Philosophy section** refined across all documents

### Improved
- **Syntax rules** reformulated for visual clarity
- **Extension guidelines** with concrete before/after example
- **Design principles** consistently applied across all documents
- **Comprehensibility** through better structure and examples

---

## [1.0] - 2025-11-16 (Initial)

### Added
- Core specification with 14 symbols
- Basic README
- Examples across multiple domains
- Validation through cross-LLM experiments

### Validated
- Biochemistry applications (Krebs cycle, protein folding, translation)
- Abstract concepts (consciousness, emotions, purpose)
- Process dynamics (collaboration, workflows)

---

## Future Considerations

Potential areas for community development:
- Domain-specific extension collections
- Syntax validator tool
- Visual notation renderer
- Cross-domain pattern library
- Educational materials
- Integration with other notation systems

---

**Note**: Version numbers follow semantic versioning principles. Breaking changes to core symbols would trigger major version increment (2.0). New extensions or documentation improvements trigger minor version increment (x.1).
