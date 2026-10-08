# The Decrees

Forking is a right granted by the license, not a verdict on the people who
wrote the code. Upstream said no. That is a legitimate decision. We build the
yes somewhere else and never make it their problem.

---

## I. Upstream owes us nothing

- No issues, PRs, discussions, emails, mailing-list posts, or chat messages to
  upstream about the fork, AI, or Rust.
- No @-mentions of upstream maintainers or contributors, anywhere.
- Never link upstream issues, PRs, or discussions from our repos. GitHub
  posts a backreference on their timeline, which is contacting them. Link
  repository roots and policy files only; quote text when you need it.
- Never ask upstream to link to us, merge back, or "reconsider".

## II. No scoreboard

- Proposals live in `natural-selection` and nowhere else. No lists elsewhere,
  no wall of shame, no "next up" posts on social media.
- A proposal states upstream's policy as a fact and links to it. It never
  characterizes the policy or the people behind it.
- Rejected and withdrawn proposals are closed and locked. Threads that drift
  into commentary about upstream maintainers are locked on sight.
- Never quote a maintainer's AI or Rust policy to mock it.
- Benchmarks are allowed; benchmarks framed as dunks are not.
- A fork's README says what the fork *is*, never what upstream got wrong.

## III. The license is the law

- Fork only projects under an OSI-approved license. Source-available, BSL,
  SSPL, non-commercial, or custom "no AI" licenses: don't touch.
- Preserve every copyright notice, `LICENSE`, `NOTICE`, and `AUTHORS` file.
- New code, Rust or otherwise, ships under upstream's license. It runs in
  the same program, so it follows the same terms.
- Crate dependencies must be compatible with upstream's license, enforced by
  `cargo deny` in CI. Watch for GPL-2.0-only: Apache-2.0-only crates can't
  be linked into it.
- Porting an existing upstream component to Rust is a translation, so it keeps
  upstream's license. That holds whether a human or an AI did the porting.
- When the license and these decrees disagree, the stricter one wins.

## IV. Not their name

- Every fork gets a distinct name. The upstream name appears only in
  attribution ("derived from X").
- No upstream logos, artwork, or branding.
- Read upstream's trademark policy before naming. When in doubt, pick
  something else.

## V. Don't leak into upstream

- Every fork carries the [banner](templates/BANNER.md) at the top of its README.
- Fork issue templates state that bugs are reported here, never upstream.
- Fork users who file fork bugs upstream get pointed back here — by us, in our
  own tracker. We do not follow them into upstream's.

## VI. Security is the one exception

- A vulnerability that also affects upstream is disclosed to upstream through
  their security policy. User safety outranks everything else in this file.
- The report must be reproduced, written, and sent by a human, with a working
  PoC. If upstream bans AI-assisted reports, the report must stand on its own
  without AI-generated prose.
- No public disclosure before upstream's embargo window closes.
- The report is about the bug. It never mentions the fork, AI, or Rust unless
  that is technically necessary to reproduce.

## VII. Earn it

- A fork passes upstream's test suite before its first release. Shipping
  regressions hands upstream the argument.
- Every `unsafe` block carries a `// SAFETY:` comment.
- "It has Rust now" is not a feature. Each fork states what it adds.

## VIII. Don't poach

- No recruiting upstream contributors or users in upstream spaces.
- No advertising the fork in upstream's issue tracker, forum, chat, or
  subreddit. People find us; we don't go find them.

## IX. Sync or sunset

- Every fork has a named human steward.
- A fork is upstream plus additions, not a replacement. Merge upstream
  regularly, and keep Rust in its own directories so the merges stay clean.
- Upstream security fixes are merged as soon as they land.
- A fork with no steward activity for 90 days is archived, with a README notice
  pointing users back to upstream. A stale fork carrying known CVEs harms users.

## X. Upstream requests

- If an upstream maintainer asks us to rename something, drop a mention,
  remove a reference to them, or stop contacting them, we comply promptly,
  without argument, in public or in private.
- The license gives us the code. It does not give us their goodwill to burn.

## XI. Enforcement

- Violating I, II, VIII, or X gets a member removed from the org. No warning
  round for harassment.
- Any member may archive a fork that violates III or VI pending review.
