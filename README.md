# 7187.bitmap — Live Organa Cell v0.2.0

Public, machine-readable and independently verifiable first live Organa Cell.

- Discovery: `/.well-known/organa.json`
- Canonical manifest: `/versions/0.2.0/organa-cell.json`
- State semantics: `/organa-state-semantics-v0.1.json`
- Lifecycle: `live`
- Activation: `active`
- Controller signature: `signed`, independently BIP-322 verified
- Private strategies, credentials, memories and account evidence are excluded.

The signed v0.2.0 manifest is an immutable pre-activation candidate snapshot. Current activation and controller-claim state come from the canonical discovery document. Do not rewrite signed manifest bytes to synchronize later state; publish a chained, freshly signed version for future manifest changes.
