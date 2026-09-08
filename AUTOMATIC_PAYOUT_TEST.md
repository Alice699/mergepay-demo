# Automatic payout test fixture

This pull request is a small, documentation-only fixture for verifying the
successful MergePay settlement path on Rialo DevNet.

## Expected path

1. Create a bounty for this exact pull request.
2. Authenticate as the pull request author and request a claim.
3. Have the sponsor approve the claim and fund the escrow.
4. Merge the pull request after funding.
5. Confirm that the workflow reaches `paid` through the native settlement path,
   without clicking the manual merge-check fallback.

Record the bounty link, workflow address, settlement signature, and final
decoded state. This repository is a public DevNet fixture; never use production
funds or private credentials.
