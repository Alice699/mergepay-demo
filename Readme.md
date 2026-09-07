# MergePay Demo

Public sandbox repository for testing GitHub bounty payments through MergePay on Rialo DevNet.

## Test task

Add a short section to this README describing why contributors should use MergePay.

Example:

> MergePay connects GitHub pull requests with onchain bounty escrow. Contributors prove PR authorship through GitHub OAuth and receive payment after the sponsor approves the claim and the PR is merged.

## Why MergePay?

Open-source contributors often finish useful work before a reward is ready to be
sent. MergePay keeps the reward in a Rialo escrow workflow, verifies the exact
GitHub pull request author, and releases the bounty only after the sponsor has
approved the contributor and Rialo confirms that the pull request was merged.

This makes the payment terms visible before work starts while keeping the
contributor's payout wallet separate from the sponsor's wallet.

## How to contribute

1. Fork this repository.
2. Create a new branch.
3. Make a small documentation change.
4. Open a public pull request.
5. Keep the pull request open until the bounty workflow is ready.

## Bounty flow

The sponsor creates a bounty for an open pull request in MergePay.

The contributor must:

- authenticate with the GitHub account that authored the pull request;
- connect the wallet that should receive the bounty;
- request a claim;
- wait for sponsor approval and funding;
- merge the pull request after approval.

Payment is released only after Rialo verifies the merge proof.

## Important notes

- This repository is for testing only.
- The bounty runs on Rialo DevNet.
- No payment is guaranteed until the sponsor approves and funds the bounty.
- Never use production funds or private credentials.
