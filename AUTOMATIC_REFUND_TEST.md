# Automatic refund test fixture

This pull request is a small, documentation-only fixture for verifying that a
funded but unmerged bounty returns to the sponsor after its deadline on Rialo
DevNet.

## Expected path

1. Create a bounty for this exact pull request with a short future deadline.
2. Authenticate as the pull request author and request a claim.
3. Have the sponsor approve the claim and fund the escrow.
4. Keep this pull request open and do not merge it.
5. After the deadline, confirm that the workflow reaches `refunded` through the
   native deadline timer, without clicking a manual refund action.

Record the bounty link, workflow address, refund signature, and final decoded
state. This repository is a public DevNet fixture; never use production funds
or private credentials.
