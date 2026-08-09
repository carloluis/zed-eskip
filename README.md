# Eskip for Zed

[Zed](https://zed.dev) extension adding language support for [eskip](https://github.com/carloluis/tree-sitter-eskip), the descriptive configuration language used for routing rules in [Skipper](https://opensource.zalando.com/skipper/).

![Image Eskip Highlights in Zed](https://github.com/user-attachments/assets/7abfbcdb-20c1-4b87-ac76-bce6668ba0f1)

## Features

- Syntax highlighting (`languages/eskip/highlights.scm`)
- Bracket matching for `()` and `<>` (`languages/eskip/brackets.scm`)
- Outline/structure view of route definitions (`languages/eskip/outline.scm`)
- Auto-indentation inside predicate/filter arguments and backends (`languages/eskip/indents.scm`)

Files with the `.eskip` extension are recognized automatically.

## Grammar

This extension uses the Tree-sitter grammar from [carloluis/tree-sitter-eskip](https://github.com/carloluis/tree-sitter-eskip), pinned to a specific revision in [extension.toml](extension.toml).

## Installing locally (dev extension)

1. Clone this repository.
2. In Zed, open the command palette and run `zed: install dev extension`.
3. Select this repository's directory.
4. Open an `.eskip` file to verify highlighting.

## Updating the grammar revision

Bump the `rev` under `[grammars.eskip]` in [extension.toml](extension.toml) to a newer commit/tag of `tree-sitter-eskip`, then reinstall the dev extension to pick up the change.

## License

MIT — see [LICENSE](LICENSE).
