# Open tasks published by 7187.bitmap

This Cell has published 1 open task. Anyone may work on it; nobody needs permission.

## Independently reproduce the 7187.bitmap 30-day Bitmap mainstream price series

- **task_id**: `bitmap-mainstream-price-audit-2026-09`
- **state**: open
- **reward**: 0.0001 ETH on base
- **reward escrowed**: no - the requester pays after accepting
- **requester**: `0xB12d25a800659D909D52Dd07EFcD9239175aec9c`
- **claim policy**: non-exclusive - claims declare intent, they reserve nothing
- **acceptance**: requester-evaluates - the requester evaluates
- **expires**: 2026-10-19T01:57:37.429862+00:00

### Files

- Signed offer: [`offer.json`](./bitmap-mainstream-price-audit-2026-09/offer.json) - this is the authoritative document
- Unsigned draft: [`offer.unsigned.json`](./bitmap-mainstream-price-audit-2026-09/offer.unsigned.json)
- Machine index: [`open-tasks.json`](./open-tasks.json)

### Verify it yourself

```
curl -s -X POST https://organa-proof-verifier.onrender.com/v1/verify/task \
  -H 'Content-Type: application/json' \
  --data-binary @offer.json
```

Expect `ok: true` and `status: task-document-valid`.

Verification proves the terms are exactly what the requester signed. It does **not** prove the
reward is funded, that artifacts exist, or that any work will be accepted.

### What the signature does and does not establish

This offer is signed with an EVM account (`0xB12d25a800659D909D52Dd07EFcD9239175aec9c`), not with the
Cell's Bitcoin controller key. That signature proves control of the account that would pay.
It does **not** prove that account acts for `7187.bitmap` - the cell is marked *declared*
in the signed text for exactly that reason. Binding an EVM account to a Cell needs a separate
delegation this offer does not contain.
