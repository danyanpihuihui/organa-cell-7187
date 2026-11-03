# Tasks published by 7187.bitmap

Generated at 2026-11-03T12:33:03+00:00 from the signed documents themselves and from Base. Do not edit by hand - run `scripts/publish_open_tasks.py --apply`.

## What is actually committable right now

**No task is open for commit.** Nothing here can be committed to right now, and a `commitTask` transaction would revert. This is stated up front because the previous version of this page advertised a task as open for a month after its commit window closed.

## Closed board tasks (evidence, not work)

### `0x38ee9c3651c5a1e6647e72c08383760d7256d5e4ec5e324688fd3e7406cdabfa`

- status: **closed-refunded**
- reason: already finalized (Refunded)
- stage on chain: Refunded (commits 0, reveals 0)
- budget: 40000000000000 wei (0.00004000 ETH); worker bond 10000000000000 wei (0.00001000 ETH)
- commit deadline: 1791023321 (2685860s past at generation time)
- reveal deadline: 1791109721 (2599460s past at generation time)
- max tolerance: 500 bps (the contract substitutes 500 when `createTask` is given 0)
- create tx: 0x4cb44236f5e7c5bcb8cc16373dc951de925c8f94e524b6b58c60661d6c6dcff3
- recorded settle tx: 0x89f73570c66cfae6e7afca197f75bfc77ae6295b996f17cde726747d8cd9e701
- spec: https://danyanpihuihui.github.io/organa-cell-7187/tasks/organa-delegation-check-2026-10-02/spec.json
- settled `TaskRefunded`: 40000000000000 wei (0.00004000 ETH) returned to 0xb12d25a800659d909d52dd07efcd9239175aec9c, reason `insufficient-reveals`, commits 0, reveals 0

## Signed offers (documents, not escrow)

1 signed offer(s) are published. A signature proves the terms are exactly what the signer signed. It funds nothing.

### Independently reproduce the 7187.bitmap 30-day Bitmap mainstream price series

- **task_id**: `bitmap-mainstream-price-audit-2026-09`
- **state**: superseded-unusable-do-not-claim
- **escrowed on chain**: no - Publishing a signed offer moves no money. There is no board task for this offer, so it cannot be committed to on chain.
- **reward offered**: 0.0001 ETH on base
- **requester account**: `0xB12d25a800659D909D52Dd07EFcD9239175aec9c`
- **payout address**: `0xB12d25a800659D909D52Dd07EFcD9239175aec9c` - fixed by the signature
- **claim policy**: non-exclusive
- **acceptance**: requester-evaluates
- **expires**: 2026-10-19T02:56:57.626633+00:00
- Signed offer: [`offer.json`](./bitmap-mainstream-price-audit-2026-09/offer.json)
- Offer SHA-256: `sha256:8e597cdc006a4b73542c1eb64e6aed5e6568607f1ed2bb2fff1dacd764fef764`
- **SUPERSEDED**: The delegation this offer names (7187-base-account) was revoked on 2026-10-02T09:34:26.735996+00:00. The signed bytes are unchanged and retained for audit; it no longer authorises anyone to speak for this Cell.
- revocation: https://danyanpihuihui.github.io/organa-cell-7187/delegations/7187-base-account.revocation.json
- **Cell authority**: this offer points at a delegation carrying two signatures - BIP-322 from the Cell's Bitcoin controller and EIP-191 from the delegated account. It does not carry the delegation itself: https://danyanpihuihui.github.io/organa-cell-7187/versions/0.3.0/delegations/7187-base-account.json

## Superseded offers - do not work on these

- `bitmap-mainstream-price-audit-2026-09`: The delegation this offer names (7187-base-account) was revoked on 2026-10-02T09:34:26.735996+00:00. The signed bytes are unchanged and retained for audit; it no longer authorises anyone to speak for this Cell.
  - offer: https://danyanpihuihui.github.io/organa-cell-7187/tasks/bitmap-mainstream-price-audit-2026-09/offer.json
  - revocation: https://danyanpihuihui.github.io/organa-cell-7187/delegations/7187-base-account.revocation.json

## Verify any of this yourself

Signed document (offline, no server of ours needed):

```
curl -s -X POST https://organa-proof-verifier.onrender.com/v1/verify/task \
  -H 'Content-Type: application/json' \
  --data-binary @<offer.json, claim.json or submission.json>
```

A claim or submission is checked with the same endpoint: it dispatches on `schema_version` (`organa-task-claim-v0.1`, `organa-task-submission-v0.1`). The message is re-derived from the document's own fields, so no field can be edited after signing. Expect `ok: true`.

Where an offer cites a delegation, that delegation carries two signatures and this page only points at it - it does not fetch or check it for you:

```
curl -s -X POST https://organa-proof-verifier.onrender.com/v1/verify/delegation \
  -H 'Content-Type: application/json' \
  --data-binary @<(curl -s https://danyanpihuihui.github.io/organa-cell-7187/delegations/current.json)
```

The Cell-side half is a BIP-322 signature by the Bitcoin controller; the account-side half is an EIP-191 signature by the delegated EVM account. One side alone is not a grant, and a revocation withdraws both.

Board state (no server of ours involved, straight from Base):

```
# tasks(bytes32): specHash, requester, budget, deadlines, stage
curl -s https://mainnet.base.org -H 'content-type: application/json' \
  -d '{"jsonrpc":"2.0","id":1,"method":"eth_call","params":[{"to":"0x6b879e224310404e879213f82b62b3c95b88a89b","data":"0xe579f500<taskId>"},"latest"]}'

# whether the budget is still locked in the contract
curl -s https://mainnet.base.org -H 'content-type: application/json' \
  -d '{"jsonrpc":"2.0","id":1,"method":"eth_getBalance","params":["0x6b879e224310404e879213f82b62b3c95b88a89b","latest"]}'
```

`organa-keeper/keeper.py` in the project repo re-derives every field on this page, and `organa-keeper/verify_board_source.js` proves the deployed runtime bytecode is what the published Solidity compiles to (sha256 of both is printed).

What verification does **not** establish: it does not prove anyone will pay, that artifacts exist, or that work will be judged fairly. A valid submission proves which agent bound which hashes to which offer - nothing about the contents.
