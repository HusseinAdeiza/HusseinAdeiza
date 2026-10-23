# Mabera Hussein Adeiza Yunusa

Infrastructure and protocol engineer. I work across **Rust** and **Go** on
compilers, consensus clients and SDKs, and I run validator, node and prover
infrastructure across a long list of networks. The contributions I'm proudest of
are the small ones that are awkward in the reasoning — error paths, lifecycle
bugs, feature-gating, rounding.

I contribute upstream rather than only building my own things: **39 merged pull
requests across 20 public repositories**, all tested against each project's own
suite and merged through its normal review process.

---

## Merged upstream work

**tangle-network/blueprint** — 15 merged PRs to the Blueprint Rust SDK
(`cli/src` and the `no_std` crate stack). CLI error surfacing, subprocess
lifecycle, `--init` scaffolding, keystore fail-closed behaviour, tracing,
release tooling.

**starkware-libs/cairo** — [#10458](https://github.com/starkware-libs/cairo/pull/10458),
`#[must_use]` now honoured on impl methods in the semantic layer, with a
diagnostic test.

**celestiaorg/celestia-node** — [#5349](https://github.com/celestiaorg/celestia-node/pull/5349),
removed a panic on a nil `TxConfig` in the state package, normalising to defaults
across the tx-client path.

**celestiaorg/celestia-core** — [#3383](https://github.com/celestiaorg/celestia-core/pull/3383),
prevote draining before precommits are injected into the consensus test state.

**IntersectMBO/mithril** — [#3566](https://github.com/IntersectMBO/mithril/pull/3566),
conversion coverage across the halo2 IVC proof system.

**genlayerlabs/genvm-manager** — 4 merged PRs: failed-to-start handling, run and
semantic-validation ordering, a shared cross-major test harness.

Also merged in: `gluwa/creditcoin3`, `pushchain/push-chain-wallet`,
`FhenixProtocol/cofhesdk`, `tkhq/qos`, `NousResearch/atropos`, `vlayer-xyz/vlayer`,
`bandprotocol/bandchain-docs`, `0xMiden/tutorials`.

---

## Hacking and contests

**Flip the Switch** (WeMakeDevs × Switch) — agent invitation policy for
[a shared room-service layer](https://github.com/sandbox-quantum/switch/issues/805):
one shared check reused by every invite path, an unverified-join path that admits
but announces, and tests for each. Implemented against the maintainer's written
policy, tested against the project's own suite, and prepared for the November PR
window.

**Stocklana** — [`streamdividend`](https://github.com/HusseinAdeiza/streamdividend):
a dividend-streaming vault for tokenized stocks on Solana. Hold `AAPLx`, earn its
real dividends in USDC pro-rata, on-chain. Mainnet-live, Pyth Lazer price feeds,
self-audited.

**PayPal AI Hackathon 2026** — [`amanah-paypal`](https://github.com/HusseinAdeiza/amanah-paypal):
an autonomous, auditable treasury agent for charities on PayPal rails.

**HackCanton S4** — [`provenance`](https://github.com/HusseinAdeiza/provenance):
payment holds where the honesty rule is enforced by the ledger, in Canton/Daml.

**Graph Hacks 2026** (WeMakeDevs × FalkorDB), Agents Track —
[`graphhacks-refusal-agent`](https://github.com/HusseinAdeiza/graphhacks-refusal-agent):
an agent that walks a FalkorDB call graph, finds an exploit path, refuses to
certify it, and files a BLOCKED CertificationRequest.
[`graphhacks-patchweaver`](https://github.com/HusseinAdeiza/graphhacks-patchweaver).

**Cairo** — the `#[must_use]` compiler fix above started as a hunt through the
semantic layer for unreported attributes.

**Security review** — reading code with a specific question in mind and refusing
to call something a bug until a runnable artifact proves it: a candidate finding
only counts when a command fails on the current tree and passes once repaired,
and the demonstration has to name the real file it is about. Findings submitted
through HackenProof, Guardian Defender and Sherlock.

---

## Projects

[`streamdividend`](https://github.com/HusseinAdeiza/streamdividend) — dividend-streaming
vault for tokenized stocks on Solana. Mainnet-live.

[`claimscout`](https://github.com/HusseinAdeiza/claimscout) — finds open-source issues
actually worth your time: deterministic triage plus open-weight-model ranking.
Python.

[`holdwatch`](https://github.com/HusseinAdeiza/holdwatch) — PayPal payout holds and
account restrictions explained the moment they happen. Webhook receiver with
signature verification and concrete next actions. Python.

[`provenance`](https://github.com/HusseinAdeiza/provenance) — payment holds where the
honesty rule is enforced by the ledger. Canton/Daml.

[`auditgraph`](https://github.com/HusseinAdeiza/auditgraph) — smart-contract
vulnerability knowledge graph on FalkorDB. Python.

[`deathclock`](https://github.com/HusseinAdeiza/deathclock) — verifiable inheritance on
Solana: an estate releases on a zero-knowledge proof of absence (RISC Zero Groth16).

[`PharmChain`](https://github.com/HusseinAdeiza/PharmChain) — one-scan medicine
verification on Monad mainnet.

[`washmap`](https://github.com/HusseinAdeiza/washmap) — crowdsourced water and
sanitation facility mapping for Nigeria: report broken boreholes, contaminated
water points and open defecation sites in real time.

---

## Validator, node and prover infrastructure

I've run and still run validators, nodes, sequencers, provers, miners and
workers across a long list of networks — testnet and mainnet, from bare metal.

<details>
<summary><b>Whitelisted validator / node runner</b></summary>

Lumoz ZkRass · Aleo ([contributor](https://github.com/HusseinAdeiza/Aleo-contributor-fan)) ·
Avail (Clash of Nodes, incl. Avail × Madara) · Sending Network (core node runner) ·
Flock.io (AI trainer and validator)

</details>

<details>
<summary><b>Public node operator</b></summary>

Taiko · CESS Storage · Dusk · Tanssai Network · Nillion (verifier) · Quai (miner)

</details>

<details>
<summary><b>Currently validating / running</b></summary>

0g Lab · Titanic (miner and node) · Drill · Gainnet AI · NESA (miner) ·
Brinx AI (worker) · KUZCO (inferencer) · Spheron (GPU distribution validator) ·
Dria (validator) · Hemis (validator) · PWR (validator) · Crynux AI (inferencer) ·
Rynus (worker) · Hyperspace aiOS (inferencer) · T3rn (validator) ·
Axone AI (validator) · Chainbase AVS (validator) · Covalent HQ (validator) ·
Gensyn AI (trainer)

[Drosera trap](https://app.drosera.io/trap?trapId=0x417f46a2d57b8abc3bfed0f0f3f5638cf96c6520) ·
[Gensyn explorer address](https://gensyn-testnet.explorer.alchemy.com/address/0xca972650be237e27467bcc78a837d4c229e77d4c?tab=internal_txns)

</details>

---

## What else I'm building

[`SanitovaCheck`](https://github.com/HusseinAdeiza/SanitovaCheck) — water, sanitation
and hygiene risk assessment for Android (Kotlin).
[`sanitova-resolve`](https://github.com/HusseinAdeiza/sanitova-resolve) — environmental
compliance disputes and parametric sanitation insurance through AI validator
consensus on GenLayer.
[`wash-risk-agent`](https://github.com/HusseinAdeiza/wash-risk-agent) — WASH incident
risk assessment on Alibaba Cloud Function Compute.

---

## Tools

Rust, Go, Python, TypeScript, Solidity, Move, Nim · Foundry, Echidna, Slither ·
Git, Docker, Linux.

---

## Contact

- Email: web3alphatester@gmail.com
- X: [@Adeiza_web3](https://twitter.com/Adeiza_web3)
- LinkedIn: [hussein-adeiza-yunusa](https://www.linkedin.com/in/hussein-adeiza-yunusa-72864b21b/)
