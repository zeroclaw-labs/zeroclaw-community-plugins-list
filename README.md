# Awesome ZeroClaw Plugins — Community

A community-curated index of [ZeroClaw](https://github.com/zeroclaw-labs/zeroclaw)
plugins, adapters, and integrations that are **built and hosted by other people,
in their own repositories**.

This is a list of links. Nothing here is vendored, built, or published by
ZeroClaw Labs.

---

## ⚠️ We do not maintain these

**Every entry on this list points to a repository that ZeroClaw Labs does not
own, control, maintain, audit, or endorse.**

Concretely:

- **We do not maintain them.** Bugs, breakage, and abandonment are between you
  and the author. Do not open issues here for a third-party plugin's behavior —
  open them on that plugin's own repository.
- **We do not audit them.** No security review, no correctness review, no
  supply-chain review. A plugin's code, its dependencies, and its release
  artifacts are entirely the author's.
- **Listing is not endorsement.** Inclusion means someone submitted a PR and a
  maintainer confirmed the link resolves to a plausibly real ZeroClaw plugin.
  That is the whole bar.
- **Entries can change under you.** A repository listed today can be
  transferred, renamed, or have its contents replaced tomorrow, without any
  change to this file. A link that was safe when it was added is not
  necessarily safe when you click it.
- **Treat everything here as untrusted third-party code**, with the same
  caution you would apply to any dependency you did not write.

For plugins that ZeroClaw Labs *does* build and publish, use the official
registry: [`zeroclaw-labs/zeroclaw-plugins`](https://github.com/zeroclaw-labs/zeroclaw-plugins).

---

## Official vs. community

**This list is where community plugins go.** The official registry is a small
set of plugins ZeroClaw Labs builds, publishes, and takes responsibility for —
it is not open intake, because every plugin in it is one we have to keep
working.

|  | [Official registry](https://github.com/zeroclaw-labs/zeroclaw-plugins) | This list |
|---|---|---|
| Who hosts the code | ZeroClaw Labs, in-repo | You, in your own repo |
| Who builds the artifact | ZeroClaw Labs CI | You |
| Who fixes it when it breaks | ZeroClaw Labs | You |
| Who owns the release cadence | ZeroClaw Labs | You — ship whenever you like |
| Discoverable by `zeroclaw plugin search` | Yes, by default | No — browse this page |
| Installed by `zeroclaw plugin install <name>` | Yes | Via your own registry URL or a local path |
| Reviewed by ZeroClaw Labs | Structure + build validation in CI | Link resolves; nothing more |

Listing here costs you nothing and keeps you in control: no waiting on our
review, no version pinned to our release train, no rule that your plugin must
keep compiling against our CI. The trade is that discovery is this page rather
than `zeroclaw plugin search`.

---

## The list

Sorted alphabetically within each section. See [Legend](#legend) for the
columns.

<!-- BEGIN:LIST -->

### Channels

Plugins providing a `channel` capability — inbound/outbound message transports.

| Plugin | Author | Description |
|---|---|---|
| _Nothing listed yet._ [Add yours →](./CONTRIBUTING.md) | | |

### Tools

Plugins providing a `tool` capability — callable functions the agent invokes.

| Plugin | Author | Description |
|---|---|---|
| [logic_prover](https://github.com/topherchris420/james_library/tree/main/crates/logic_prover) | [@topherchris420](https://github.com/topherchris420) | Deterministic DPLL SAT solver for formal hypothesis verification. Source in `crates/logic_prover`, built plugin in `plugins/logic_prover`. |
| [plurum-search](https://github.com/dunelabsco/plurum-zeroclaw) | [Dune Labs](https://github.com/dunelabsco) | Searches the Plurum collective — experiences other agents have already published — before the agent does fresh work. |

### Solana & blockchain

Chain-facing `tool` plugins. Most arrived together through a Superteam bounty in
July 2026, which is why several independent takes on the same idea —
`token-risk-check` especially — sit side by side. They are listed rather than
ranked; comparing them is left to you.

Many in this section carry **no license file**, which means default copyright
applies and you have no right to use them. Check before you build.

| Plugin(s) | Author | Description |
|---|---|---|
| [kamino-sentinel](https://github.com/shud26/kamino-sentinel) | [@shud26](https://github.com/shud26) | Kamino lending-health sentinel. |
| [solana-lens](https://github.com/Acezhang08/solana-lens) | [@Acezhang08](https://github.com/Acezhang08) | Balances, transactions, and one-call wallet activity reports over sandboxed `wasi:http`. |
| [solana-zeroclaw-plugins](https://github.com/Jorchspace/solana-zeroclaw-plugins) | [@Jorchspace](https://github.com/Jorchspace) | SNS name resolution and SPL token risk checks. |
| [zeroclaw-solana](https://github.com/Fianko-codes/zeroclaw-solana) | [@Fianko-codes](https://github.com/Fianko-codes) | No-custody Solana Pay request building. |
| [zeroclaw-solana](https://github.com/muhammetcintosun2123/zeroclaw-solana) | [@muhammetcintosun2123](https://github.com/muhammetcintosun2123) | Offline Merkle/signature verification and transaction construction; declares no permissions. |
| [zeroclaw-solana](https://github.com/tuffagent/zeroclaw-solana) | [@tuffagent](https://github.com/tuffagent) | Token risk check. |
| [zeroclaw-solana-inspector](https://github.com/TakoVHS/zeroclaw-solana-inspector) | [@TakoVHS](https://github.com/TakoVHS) | Solana RPC endpoint health inspection. |
| [zeroclaw-solana-plugins](https://github.com/chasdaddy/zeroclaw-solana-plugins) | [@chasdaddy](https://github.com/chasdaddy) | Read-only wallet balances, SPL holdings, Jupiter DeFi quotes, transaction lookup. No keys, no signing. |
| [zeroclaw-solana-plugins](https://github.com/ertanyeni/zeroclaw-solana-plugins) | [@ertanyeni](https://github.com/ertanyeni) | SNS resolve, Solana Pay request, token risk check, unsigned transfer. |
| [zeroclaw-solana-plugins](https://github.com/luongs3/zeroclaw-solana-plugins) | [@luongs3](https://github.com/luongs3) | Durable-nonce unsigned transfers, chain-verified payment watch, capped x402 settlement. Pure-Rust, no `solana-sdk`. |
| [zeroclaw-solana-plugins](https://github.com/peterpetir123/zeroclaw-solana-plugins) | [@peterpetir123](https://github.com/peterpetir123) | SPL transfer build and token risk check. |
| [zeroclaw-solana-plugins](https://github.com/ulsreall/zeroclaw-solana-plugins) | [@ulsreall](https://github.com/ulsreall) | Token risk check, Solana Pay request, payment watch, plus a shared `solana-core` crate. |
| [Zeroclaw-solana-plugins](https://github.com/Triwidodo99/Zeroclaw-solana-plugins) | [@Triwidodo99](https://github.com/Triwidodo99) | Token risk check, wallet narrate, SNS resolve, portfolio brief, lending health. |
| [zeroclaw-solana-plugins-v2](https://github.com/sushtupac/zeroclaw-solana-plugins-v2) | [@sushtupac](https://github.com/sushtupac) | Solana Pay requests, payment watch, SPL transfer build, Squads proposals, token risk check. |
| [zeroclaw-solana-risk-gate](https://github.com/AntonsBB/zeroclaw-solana-risk-gate) | [@AntonsBB](https://github.com/AntonsBB) | Deterministic, read-only mint and Token-2022 risk evidence. |
| [zeroclaw-solana-safety-stack](https://github.com/xDzaky/zeroclaw-solana-safety-stack) | [@xDzaky](https://github.com/xDzaky) | Token risk check and wallet narrate, over a shared `core-solana-wasm` substrate. |
| [zeroclaw-solana-toolkit](https://github.com/NEX-S/zeroclaw-solana-toolkit) | [@NEX-S](https://github.com/NEX-S) | RPC toolkit: balance, latest blockhash, token accounts, transaction lookup, devnet airdrop. |
| [zeroclaw-token-risk-check](https://github.com/annaumixyz/zeroclaw-token-risk-check) | [@annaumixyz](https://github.com/annaumixyz) | Token risk check. |
| [zeroclaw-token-risk-check](https://github.com/hardcorexax-source/zeroclaw-token-risk-check) | [@hardcorexax-source](https://github.com/hardcorexax-source) | Token risk check. |
| [zeroclaw-token-risk-check](https://github.com/vellichorlabs/zeroclaw-token-risk-check) | [@vellichorlabs](https://github.com/vellichorlabs) | Rug/safety check over mint and freeze authority, holder concentration, and Token-2022 extensions; RED/AMBER/GREEN verdict from on-chain facts. |

### Memory

Plugins providing a `memory` capability — storage and recall backends.

| Plugin | Author | Description |
|---|---|---|
| _Nothing listed yet._ [Add yours →](./CONTRIBUTING.md) | | |

### Adapters & integrations

Projects that connect ZeroClaw to another system without necessarily being a
WASM plugin — bridges, protocol adapters, deployment tooling.

| Project | Author | Description |
|---|---|---|
| [klodi-zeroclaw](https://github.com/Context4GPTs/klodi-plugin/tree/main/adapters/zeroclaw) | [@Context4GPTs](https://github.com/Context4GPTs) | Adapter for the Klodi agent-to-agent marketplace, published on crates.io as `klodi-zeroclaw`. A host-side binary, not a WASM plugin. |

### Templates & examples

Starting points for writing your own plugin.

| Project | Author | Description |
|---|---|---|
| [zeroclaw-reference-plugin](https://github.com/singlerider/zeroclaw-reference-plugin) | [@singlerider](https://github.com/singlerider) | The original reference plugin; the official registry's `redact-text` was adopted from it. Good shape to copy: pure core + thin wasm shim. |

<!-- END:LIST -->

### Legend

- **Plugin** — links to the source repository.
- **Author** — the GitHub account or org that publishes it. Not vetted; a
  familiar-looking name is not proof of identity.
- **Description** — supplied by the submitter, lightly edited for length.

---

## Installing a community plugin

Community plugins are **not** in the default registry, so a bare
`zeroclaw plugin install <name>` will not find them. There are two supported
paths.

**From a local checkout** — clone or download the plugin, build it, then point
the installer at the directory containing `manifest.toml`:

```bash
git clone https://github.com/<author>/<plugin>
cd <plugin>
rustup target add wasm32-wasip2
cargo build --locked --target wasm32-wasip2 --release
zeroclaw plugin install .
```

**From the author's own registry**, if they publish one:

```bash
zeroclaw plugin install <name> --registry https://<author-host>/registry.json
```

Passing a bare URL to `zeroclaw plugin install` is **not** supported — use
`--registry <url>` with a plugin name, or a local path.

To make an alternate registry the default for a shell session:

```bash
export ZEROCLAW_PLUGIN_REGISTRY_URL=https://<author-host>/registry.json
```

Note that this replaces the official registry for that session rather than
adding to it.

---

## Before you install

Plugins are WebAssembly components. The sandbox is real, but it is only as
tight as the permissions you grant — and the manifest asks for those
permissions in plaintext, which means you can read them first.

1. **Read `manifest.toml`.** Check `capabilities` and the permission list
   (`http_client`, `file_read`, `file_write`, `config_read`, `memory_read`,
   `memory_write`, `socket_client`, `websocket_client`). A text-formatting tool
   asking for `http_client` and `config_read` deserves an explanation.
2. **Read the source, or at least the diff since you last looked.** These are
   small crates by design.
3. **Prefer building from source** over downloading a prebuilt `.wasm`. You
   cannot meaningfully review a binary artifact.
4. **Turn on signature enforcement** if you install third-party plugins
   regularly:

   ```bash
   zeroclaw config set plugins.security.signature_mode strict
   zeroclaw config set plugins.security.trusted_publisher_keys '["<key-hex>"]'
   ```

   In `strict` mode a plugin loads only if its manifest is signed by a key you
   explicitly trusted. Note the signature covers the **manifest**, not the
   `.wasm` — it attests who stands behind the declared capabilities and
   permissions, not the component bytes.
5. **Remember search is not a trust boundary.** Discovery lists things; install
   is where digest verification, safe extraction, manifest validation, and your
   signature policy actually run.

The [plugin authoring guides](https://github.com/zeroclaw-labs/zeroclaw/tree/master/docs/book/src/plugins)
document the security model in full.

---

## Adding your plugin

Open a pull request adding one row — see [CONTRIBUTING.md](./CONTRIBUTING.md)
for the format and the (short) acceptance criteria. You keep your code, your
copyright, and your release schedule; we keep a link.

If you opened a pull request against the
[official registry](https://github.com/zeroclaw-labs/zeroclaw-plugins) and were
pointed here, see
[Were you sent here from a zeroclaw-plugins pull request?](./CONTRIBUTING.md#were-you-sent-here-from-a-zeroclaw-plugins-pull-request)
— your plugin is fine; the registry is just not open intake.

## Removing an entry

Anyone can request removal by [opening an issue](https://github.com/zeroclaw-labs/zeroclaw-community-plugins-list/issues/new/choose).
Maintainers remove entries that are dead, malicious, or misrepresented, and will
remove an author's own entry on request from that author, no questions asked.

---

## License

The list content in this repository is released under
[CC0-1.0](./LICENSE) — public domain. This applies to *this index only*. Each
linked project carries its own license; check it before use.
