# Contributing

This repository is an index of links. A contribution is one row in a table.

## Add your plugin

1. Fork this repository.
2. Add one row to the correct section of [`README.md`](./README.md), in
   alphabetical order within that section:

   ```markdown
   | [plugin-name](https://github.com/you/plugin-name) | [@you](https://github.com/you) | One sentence, under 140 characters, saying what it does. |
   ```

3. Open a pull request using the template. Title it `add: <plugin-name>`.

Remove the `_Nothing listed yet._` placeholder row if yours is the first entry
in that section.

## What gets accepted

The bar is deliberately low and deliberately explicit — we are confirming a link
is real, not vouching for the code.

A maintainer will merge your PR if:

- **It works with ZeroClaw.** The repository is a ZeroClaw plugin, adapter, or
  integration — not a general-purpose library that happens to be Rust or WASM.
- **The link resolves** to a public repository with a README explaining what it
  is.
- **The description is accurate and plain.** One sentence, no marketing. "Sends
  metrics to Prometheus" — not "revolutionary observability platform".
- **You are the author, or you say who is.** Submitting someone else's project
  is fine; do not imply it is yours.
- **It is in the right section.** Channels, Tools, and Memory mean the
  corresponding plugin `capabilities` value. If it is not a WASM plugin, it goes
  in Adapters & integrations.

A maintainer will decline if the repository is empty, is a fork with no
substantive changes, is unrelated to ZeroClaw, is malware, or if the description
misrepresents what it does.

## What we do not do

We do not review your code. We do not test that it builds. We do not verify the
author's identity. Merging your PR is not an endorsement, and the README says so
prominently — please do not describe a listing here as ZeroClaw Labs having
approved, verified, certified, or partnered with your project.

If you want a plugin that ZeroClaw Labs builds and publishes, contribute it to
the [official registry](https://github.com/zeroclaw-labs/zeroclaw-plugins#add-a-plugin)
instead. That path has real CI and real review.

## Keeping your entry accurate

You own your row. If your repository moves, is renamed, is archived, or changes
scope, please open a PR to update or remove the entry. Maintainers periodically
remove entries whose links have died.

## Removing an entry

Open an issue. An author asking for their own project to be delisted is honored
without discussion.

## Licensing

By contributing you agree that your changes to *this index* are released under
[CC0-1.0](./LICENSE). This says nothing about the license of the project you are
linking to, which stays entirely yours.
