# Portfolio case study

## The brief

Overseas social operators often need to respond quickly to KOL posts without sounding generic, overly promotional, or detached from the source. The challenge is not producing more words; it is consistently finding a useful angle while respecting uncertainty and the operator’s real identity.

## Product goal

Create a reusable editorial system that converts one source post into several genuinely different reply directions. The operator should be able to compare options, understand each English draft through a Chinese translation, and make the final publishing decision.

## Design decisions

### 1. Optimize for choice, not volume

The default five-option set has explicit roles: recommended, concise, expert, community, and conversation starter. This prevents five superficial rewrites of the same sentence.

### 2. Separate source facts from interpretation

The workflow first identifies what the source actually claims, then adds an editorial angle. Unverified numbers, causal claims, current roles, and breaking news require verification or conditional language.

### 3. Keep promotion proportional

When a user supplies a related link, the skill connects it to the comment in one natural sentence. It avoids generic calls to click, follow, or buy. Relevant affiliation is disclosed rather than hidden.

### 4. Preserve human accountability

The skill drafts text only. It does not log into X, post comments, scrape users, or coordinate multiple accounts. The operator reviews tone, facts, context, and disclosure before publishing.

## Information architecture

| Layer | Purpose |
| --- | --- |
| `SKILL.md` | Compact decision workflow and non-negotiable safeguards |
| `references/angle-library.md` | Domain-specific editorial lenses and sentence patterns |
| `references/examples.md` | Hypothetical examples showing the expected output standard |
| `agents/openai.yaml` | User-facing Codex metadata and starter prompt |
| Root documentation | Installation, public demonstration, and contribution guidance |

## Quality model

Every candidate is evaluated on five dimensions:

1. **Source fidelity** — it does not contradict or overstate the post.
2. **Distinct point of view** — it adds one useful interpretation.
3. **Platform fit** — it is concise, natural, and reply-shaped.
4. **Conversation value** — it gives readers something worth reacting to.
5. **Integrity** — it avoids fabricated evidence, hidden affiliation, impersonation, and spam tactics.

## Limitations

- A draft is not a fact check. Live claims may require external verification.
- Chinese translations support review; they are not intended for automatic publishing.
- Tone needs vary by account voice, market, and community norms.
- The skill cannot guarantee impressions, replies, followers, or conversion.

## Outcome

The result is a portable, installable Codex skill with progressive disclosure, bilingual editorial review, representative demos, and explicit responsible-use boundaries. It is ready to serve as a public portfolio artifact or as a foundation for a team-specific social operations workflow.
