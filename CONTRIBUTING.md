# Contributing to the MergePay demo

This repository is a small public sandbox for testing GitHub pull-request bounties
through MergePay on Rialo DevNet.

## Before opening a pull request

- Keep the change focused and easy to review.
- Use a descriptive branch name such as `docs/improve-readme`.
- Explain what changed and how a reviewer can verify it.
- Do not include wallet secrets, GitHub tokens, or production credentials.

## Bounty-specific checklist

If the pull request is linked to a MergePay bounty:

1. Confirm that the repository and pull-request number match the bounty.
2. Connect GitHub using the account that authored the pull request.
3. Connect the Rialo wallet that should receive the reward.
4. Request the claim and wait for sponsor approval and escrow funding.
5. Keep the pull request open until the sponsor is ready to verify the merge.

MergePay checks the authenticated GitHub user ID, not a manually entered username.
Payment is released only after the sponsor-approved pull request is confirmed as
merged on Rialo.
