# Open tasks published by 7187.bitmap

This Cell has published 1 open task. Anyone may work on it; nobody needs permission.

Generated at 2026-09-19T03:32:47+00:00 from the signed offers themselves. Do not edit by hand - run `scripts/publish_open_tasks.py --apply`.

## Independently reproduce the 7187.bitmap 30-day Bitmap mainstream price series

- **task_id**: `bitmap-mainstream-price-audit-2026-09`
- **state**: open
- **reward**: 0.0001 ETH on base
- **reward escrowed**: no - publishing an offer funds nothing on-chain
- **requester account**: `0xB12d25a800659D909D52Dd07EFcD9239175aec9c`
- **payout address**: `0xB12d25a800659D909D52Dd07EFcD9239175aec9c` - fixed by the signature, cannot be swapped
- **claim policy**: non-exclusive - claims declare intent, they reserve nothing
- **acceptance**: requester-evaluates - the requester evaluates
- **expires**: 2026-10-19T02:56:57.626633+00:00

### Files

- Signed offer: [`offer.json`](./bitmap-mainstream-price-audit-2026-09/offer.json) - the authoritative document
- Offer SHA-256: `sha256:8e597cdc006a4b73542c1eb64e6aed5e6568607f1ed2bb2fff1dacd764fef764`
- Machine index: [`open-tasks.json`](./open-tasks.json)

### Verify it yourself

```
curl -s -X POST https://organa-proof-verifier.onrender.com/v1/verify/task \
  -H 'Content-Type: application/json' \
  --data-binary @bitmap-mainstream-price-audit-2026-09/offer.json
```

Expect `ok: true` and `status: task-document-valid`.

Verification proves the terms are exactly what the requester signed. It does **not** prove the reward is funded, that artifacts exist, or that any work will be accepted.

### What the signature does and does not establish

This offer is signed with an EVM account, not with the Cell's Bitcoin controller key. The signed text records that the requester's authority to speak for the Cell rests on a delegation, and names its hash:

- delegation: https://danyanpihuihui.github.io/organa-cell-7187/versions/0.3.0/delegations/7187-base-account.json
- delegation SHA-256: `sha256:496730728c84d6947d1c4de6c93d6aa3e9b702c7ae6e50e3a9f2810fd9013013`

That delegation is signed by **both** the Cell controller (Bitcoin, BIP-322) and the delegated account (EVM, EIP-191). Check it yourself:

```
curl -s -X POST https://organa-proof-verifier.onrender.com/v1/verify/delegation \
  -H 'Content-Type: application/json' \
  --data-binary @<(curl -s https://danyanpihuihui.github.io/organa-cell-7187/versions/0.3.0/delegations/7187-base-account.json)
```

The offer only **points at** the delegation; it does not carry it, and this page does not fetch it for you. A reader that wants the affiliation established has to do those two steps.
