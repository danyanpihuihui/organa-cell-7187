# 7187.bitmap — Bitcoin L1 Weekly Commitments Proof Index

Generated at `2026-11-26T12:04:55+00:00` directly from **confirmed Bitcoin mainnet transaction witnesses**. Do not edit by hand — regenerate with `PYTHONPATH=src python3 scripts/publish_bitcoin_weekly_proofs.py --apply`.

## Strict On-Chain Disclosure Boundary

- **Source policy**: `bitcoin-l1-confirmed-witness-only` (every entry is decoded directly from confirmed Bitcoin L1 Taproot witness bytes; local private directories and unconfirmed/in-progress weeks are never read).
- **Minimal public allowlist**: inscription IDs, Bitcoin block heights/hashes/timestamps, exact witness payload SHA-256 & byte lengths, on-chain parent tags, chain pointers, trade counts, `strategy_index` / weekly return %, and daily cryptographic Merkle roots.
- **Excluded by policy**: account balance amounts, cash flow amounts, sampled trade row names/tickers, holdings, stock selection logic, model parameters, and broker statements.

## Summary

- **Parent Bitmap**: `50123b2d404f0ca8d97d07a98bd897d748b2db3d611496fa4eb1288171e8ea61i0` (Bitcoin block `794524`)
- **Strategy Passport**: `399fded9cb7caa4e0d3058d86e22cd5958b2dfd966d3e42f3dc4f36586417122i0` (Bitcoin block `956675`)
- **Confirmed Weekly Commitments**: `19` (`2026-W28` .. `2026-W47`)
- **Confirmed Weekly Reveals**: `18`
- **Bitcoin Block Span**: `957422` → `976860`
- **Total Committed Trades**: `1409`
- **Latest On-Chain Strategy Index**: `90.9797` (weekly return `-5.3840%`)
- **Deliberately Skipped Weeks**: `2026-W35`
- **Index JSON SHA-256**: `sha256:109c7edb79f51915a3e3ff3950124d674b0bfa16afdbe6308ba97bc5acf593dd`
- **OpenTimestamps Proof**: [`index.json.ots`](./index.json.ots) (submitted to 2 official OTS calendars)

## Historical Chain Continuity Notes (Preserved Verbatim)

- **2026-W40** (`750e37241fba6839959654540d873a3532490450dd661303d7c360546c8a1509i0`): Immutable on-chain payload points to 62f9b306e72a2442b528401b280547add829d65d7eb407335ef55bc51bab225fi0 (2026-W38 reveal inscription) instead of 2026-W39 commitment 97822fcfa2e81c70abd1402043db95a6b5347ec0a8f9d6b654a86bdb5205746bi0; preserved verbatim from Bitcoin L1 witness.

## Confirmed Bitcoin L1 Weekly Record

| Week | Trading Range | Trades | Strategy Index | Weekly % | Commitment Block & ID | Reveal Block & ID |
|---|---|---:|---:|---:|---|---|
| 2026-W28 | 2026-07-06..2026-07-10 | 68 | — | — | #957422 [`970bef575e…`](https://blockstream.info/tx/970bef575e16a101616905ebb48be2101844c31acf98bcc68c9448bc52f6b095) | #957431 [`5acab23e61…`](https://blockstream.info/tx/5acab23e616a664ab7b81e6f44e70f11d5fb5d5b9e999a0416c964d91dab5b0d) |
| 2026-W29 | 2026-07-13..2026-07-17 | 108 | — | — | #958480 [`f4e11247b1…`](https://blockstream.info/tx/f4e11247b10c00a7041f64c81e27d81a28a8c85ffa090a3c3c4672dba037734e) | #958489 [`8e6472f3d1…`](https://blockstream.info/tx/8e6472f3d1f98a85da28dc126c1266855641f8a2c639274190ed70359b5e4285) |
| 2026-W30 | 2026-07-20..2026-07-24 | 88 | — | — | #959489 [`9c913cd805…`](https://blockstream.info/tx/9c913cd8058a6fb136f7cd93ef3478f8425c84756af37d3cd4bd03591c10d618) | #959502 [`8ace1c8761…`](https://blockstream.info/tx/8ace1c8761efcf3addc7173f103d7c6b47a38859d75a8d286f34a5e73f2df1b9) |
| 2026-W31 | 2026-07-27..2026-07-31 | 73 | — | — | #960910 [`fc88e6d1a3…`](https://blockstream.info/tx/fc88e6d1a344cd8069cfe451a6379937d2cad79aa0c95e0910fbeb89f185698d) | #960943 [`4f52e2496a…`](https://blockstream.info/tx/4f52e2496a85575084bc68bddf4ef440fb511d22e00f5ca2da0bba657854c551) |
| 2026-W32 | 2026-08-03..2026-08-07 | 77 | — | — | #961521 [`b835605191…`](https://blockstream.info/tx/b8356051913834ed4bf347d56de9a076cee2af1ff91e2d703a805716a09726e1) | #961535 [`58b948d25e…`](https://blockstream.info/tx/58b948d25e199f974017cdc128dc4aa0c143d5586fd5dae5a8ed95598a713b58) |
| 2026-W33 | 2026-08-10..2026-08-14 | 74 | — | — | #962509 [`0a8390af02…`](https://blockstream.info/tx/0a8390af0265d9ff675d1c3128806d0fe39989715cc88ed6d08eaf1252d2f12d) | #962537 [`fbd8648346…`](https://blockstream.info/tx/fbd8648346a6510a665a065676b14e5f51c0cb79ec172616a1669b692f75d4ca) |
| 2026-W34 | 2026-08-17..2026-08-21 | 98 | — | — | #963516 [`3350c15f5d…`](https://blockstream.info/tx/3350c15f5d52ce50b25929f312e1d538c3c814b9250a7ced404eb37f0592a6a3) | #963593 [`a6df62dc56…`](https://blockstream.info/tx/a6df62dc56a890543e9b47386032a4c6f595681b0e9e08d9db8b37271a04c331) |
| 2026-W36 | 2026-08-31..2026-09-04 | 68 | — | — | #965519 [`5e14ab6fac…`](https://blockstream.info/tx/5e14ab6facd8cce03fe782362323b21469dfcbcddab960700cc5cb845ef230ed) | _commit-only_ |
| 2026-W37 | 2026-09-07..2026-09-11 | 53 | — | — | #966712 [`3b1fa62d3f…`](https://blockstream.info/tx/3b1fa62d3f78d165bdc94c056cbe0e2de60e2af756e066b83771176f25d77c31) | #966759 [`47c440167d…`](https://blockstream.info/tx/47c440167dbb08f412c5d246a6b9490767d163f77573f1e8de65777dfaaa2ed1) |
| 2026-W38 | 2026-09-14..2026-09-18 | 64 | 105.2640 | — | #967559 [`79778ae702…`](https://blockstream.info/tx/79778ae7028e5e3304ef93894b35aa1472b9ca55ede3cc0108e66914063ddb68) | #967627 [`62f9b306e7…`](https://blockstream.info/tx/62f9b306e72a2442b528401b280547add829d65d7eb407335ef55bc51bab225f) |
| 2026-W39 | 2026-09-21..2026-09-24 | 53 | 102.9428 | -2.2050% | #968381 [`97822fcfa2…`](https://blockstream.info/tx/97822fcfa2e81c70abd1402043db95a6b5347ec0a8f9d6b654a86bdb5205746b) | #968462 [`421290394a…`](https://blockstream.info/tx/421290394a3b400e65e4e5c2ffae77a97741cca5b84ac01af71c50656e4133f5) |
| 2026-W40 | 2026-09-28..2026-09-30 | 32 | 100.8434 | -2.0395% | #969287 [`750e37241f…`](https://blockstream.info/tx/750e37241fba6839959654540d873a3532490450dd661303d7c360546c8a1509) | #969331 [`e074804d25…`](https://blockstream.info/tx/e074804d2524bb9170b15bf983f7ed5a3dc9160bfac26d7bcfcb05cd747bb3d2) |
| 2026-W41 | 2026-10-08..2026-10-09 | 18 | 99.0170 | -1.8112% | #970748 [`0fece084a3…`](https://blockstream.info/tx/0fece084a3597912ba679693c9428703887d927d680a88ab67a04e57cafe7800) | #970780 [`b98ae489ba…`](https://blockstream.info/tx/b98ae489bad762a721ab04e57a20b23ec282d5fd7cf47a3a774bd552e7970119) |
| 2026-W42 | 2026-10-12..2026-10-16 | 50 | 97.9296 | -1.0981% | #971693 [`012b2e02d9…`](https://blockstream.info/tx/012b2e02d9cfc83545d9be646a0cbe7d1f472313f475aa1bf07af5916fc9198a) | #971702 [`f7bbf9b51f…`](https://blockstream.info/tx/f7bbf9b51fb67f7d793629b4580cac8370740495910b424276761816ee9bec9b) |
| 2026-W43 | 2026-10-19..2026-10-23 | 53 | 96.9286 | -1.0221% | #972864 [`724a313a0e…`](https://blockstream.info/tx/724a313a0ec819186552f6ef81062cbf3099f0f75053521bacf66a25f29ababc) | #972876 [`a3ffd720a9…`](https://blockstream.info/tx/a3ffd720a9fcdc779c51e135bee3283947b63d8bb82f549365b896a58b96ae51) |
| 2026-W44 | 2026-10-26..2026-10-30 | 80 | 95.9707 | -0.9883% | #973813 [`99a6d86742…`](https://blockstream.info/tx/99a6d8674213fc20804390ad0a61be2528014a7feecf14f5408fdfa6deb45c01) | #973827 [`d4ad0bc362…`](https://blockstream.info/tx/d4ad0bc362dd28430e8b6c6c91a129d33fc646a19fad4af7ac05934b3b6973d2) |
| 2026-W45 | 2026-11-02..2026-11-06 | 54 | 96.4201 | 0.4683% | #974901 [`15a920070a…`](https://blockstream.info/tx/15a920070a987bc8f4ba084df4774680fa786a60d71a8473425e1d1afb5b52a9) | #974920 [`0d7f66be11…`](https://blockstream.info/tx/0d7f66be117cbe63744a70597a94e4a50bae56f4f394d45614be59ea6b95ff02) |
| 2026-W46 | 2026-11-09..2026-11-13 | 151 | 96.1568 | -3.8232% | #975673 [`471e99a703…`](https://blockstream.info/tx/471e99a7037189ebeda0d33d691235f77188dc5c08dd20ab98001d6d07543a5a) | #975682 [`f88a3e6727…`](https://blockstream.info/tx/f88a3e672760b0cb84e645c4b411002fd24a98692fa9a04794ad64de729cad77) |
| 2026-W47 | 2026-11-16..2026-11-20 | 147 | 90.9797 | -5.3840% | #976833 [`9992002e6d…`](https://blockstream.info/tx/9992002e6d862478a942d4adb8b6f3afb036b26dad9f2b64b1ca28b6ed4aa6d4) | #976860 [`d8917af885…`](https://blockstream.info/tx/d8917af88500640a0ddb7d7a8456ea1b73b9b7a070ebfe076765e330a81a384a) |

## Verify Independently

1. **Verify index structure, privacy boundary & monotonic chain checks via public verifier**:

```bash
curl -s -X POST https://organa-proof-verifier.onrender.com/v1/verify/bitcoin-weekly-index \
  -H 'Content-Type: application/json' \
  --data-binary @<(curl -s https://danyanpihuihui.github.io/organa-cell-7187/proofs/bitcoin-weekly-commitments/index.json)
```

2. **Re-derive directly from Bitcoin L1 witnesses (no Organa server required)**:

```bash
PYTHONPATH=src python3 scripts/publish_bitcoin_weekly_proofs.py
```

## What This Proves / Does Not Prove

- **Proves**: Each listed commitment and reveal inscription exists in a confirmed Bitcoin mainnet transaction witness, declares 7187.bitmap as parent, matches its reported SHA-256 and byte length, and binds each reveal to its week's commitment with a post-commit Bitcoin seed block.
- **Does not prove**: It does not expose private holdings, stock selection models, broker statements, or fiat account balances, and it does not by itself verify broker-to-chain accounting without private/selective-reveal audit material or prove future performance.
