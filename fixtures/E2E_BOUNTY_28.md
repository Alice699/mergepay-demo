# E2E Bounty Fixture 28

Fresh public pull request for a MergePay settlement walkthrough on Rialo DevNet.

- Contributor: `biawakLahat`
- Target repository: `Alice699/mergepay-demo`
- Target branch: `main`
- Asset: test RLO only

## Walkthrough

1. Verify this PR in MergePay and lock its exact head commit and target branch.
   Choose the reward, optional CI/review requirements, and an absolute deadline
   that leaves enough time for claim, approval, funding, and proof processing.
2. Authenticate as the PR author and request a claim using a receiving wallet
   different from the sponsor wallet.
3. Have the sponsor approve the claim and fund the escrow.
4. For the paid path, satisfy the locked policy and merge the unchanged PR
   early enough for a valid proof callback to execute before the deadline.
5. For the refund path, leave the PR unmerged and wait for native settlement
   after the deadline. An expired countdown alone does not prove a refund.
6. Read the final workflow flags and open the settlement receipt to verify the
   amount, destination, and terminal transaction when its link is available.

Do not push another commit after locking the bounty's head SHA. Leave this PR
open until the sponsor is ready. To demonstrate fully automatic settlement,
do not press Run check now or submit a manual refund; disclose any fallback use.

This fixture changes documentation only and does not modify MergePay code.
