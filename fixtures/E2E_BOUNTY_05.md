# E2E Bounty Fixture 05

This fixture exercises MergePay's complete automatic payout path after the
GitHub identity-binding hardening.

- Contributor: `biawakLahat`
- Required check: `CI check`
- Sponsor action: verify this exact pull request, approve the contributor
  wallet, and fund the bounty
- Merge action: merge only after the CI check succeeds
- Expected result: MergePay observes the merge proof and releases escrow to
  the approved contributor wallet automatically

The bounty must lock this pull request's current head commit. Any later commit
requires a fresh MergePay workflow so the settlement proof remains exact.
