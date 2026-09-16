# E2E Bounty Fixture 04

This fixture exercises the refund fallback around an expired MergePay bounty.

- Intended path: automatic refund with manual fallback available
- Contributor: `biawakLahat`
- Sponsor action: fund the bounty and keep this PR unmerged through its deadline
- Expected result: escrow is refunded exactly once, even if a manual retry races the timer

The fixture should remain open until the terminal refunded state is visible on-chain.
