# MergePay bounty test scenarios

Use these small scenarios when reviewing a bounty linked to this repository.
They are intentionally documentation-only so the repository remains safe to use as
a public DevNet sandbox.

## Scenario A: approved contributor

1. Open a pull request with a focused change.
2. Ask the sponsor to create a bounty for the exact repository and pull-request number.
3. Authenticate with the GitHub account that authored the pull request.
4. Connect the wallet that should receive the reward and request a claim.
5. Have the sponsor approve the claim and fund the escrow.
6. Merge the pull request, then run the merge check in MergePay.
7. Confirm that the workflow reaches `paid` and that the contributor wallet receives the reward.

## Scenario B: expired unmerged pull request

1. Create a second bounty with a short future deadline.
2. Claim and fund it, but leave the pull request unmerged.
3. Wait until the deadline has passed.
4. Confirm that the workflow does not pay the contributor.
5. Verify the refund path and record the final transaction signature.

For both scenarios, record the bounty link, workflow address, transaction signatures,
and final workflow state. Never use production credentials or real funds in this
repository.

## Scenario C: contributor claim review

1. Open a fresh pull request with a focused documentation change.
2. Create a bounty for the exact pull request and authenticate as its author.
3. Request the contributor claim and verify the sponsor review state.
4. Approve and fund the claim, then confirm that the contributor page advances
   without a manual refresh.
