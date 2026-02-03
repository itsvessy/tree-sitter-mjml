# tree-sitter-mjml

A Tree-sitter grammar for MJML (Mailjet Markup Language), based on the
`tree-sitter-xml` grammar with MJML-specific packaging and build fixes for Zed.

## Status

- Language: MJML
- Tree-sitter CLI: generated with v0.25.x
- Editor support: Zed (via the MJML Zed Plugin)

## Usage

This repo is primarily intended as a grammar dependency for the
[`mjml-zed-plugin`](https://github.com/itsvessy/mjml-zed-plugin). Zed will fetch
and compile this grammar automatically when the MJML extension is installed.

## Attribution

This grammar is derived from:

- [tree-sitter-xml](https://github.com/tree-sitter-grammars/tree-sitter-xml) (MIT)

The MJML grammar retains the XML grammar structure and scanner logic, with
adjustments to:

- rename the grammar and external scanner symbols to `mjml`
- vendor Tree-sitter headers needed for Zed’s WASM grammar build

## License

MIT
