---
title: view.code
status: reference
---

# view.code

Code editor for [GAMS](https://github.com/kkgams/gams). Host runtime APIs, utilities and widgets remain external dependencies.

| View | Source | Screenshot | Original work |
| --- | --- | --- | --- |
| `view-code` | [views/view-code.js](https://github.com/kkgams/view.code/blob/release/src/views/view-code.js) | Not available | GAMS contributors |

## Development

Requires Node.js 24+, Python 3, Make, curl, tar, unzip and zip. No compilation or package installation is required.

| Command | Purpose |
| --- | --- |
| `make open` | Open local gams.json in the released macOS Apple Silicon Host. |
| `make check` | Check View JavaScript syntax. |
| `make package` | Build stable-name View ZIPs and SHA256SUMS under build.nosync/. |
| `make docs` | Build pinned wiki v1.4.0 under build.nosync/site/. |
| `make serve-docs DOCS_PORT=8081` | Preview the wiki on an independent port. |
| `make validate-docs` | Validate wiki content and links. |
| `make clean` | Remove build.nosync and identified downloaded Host/Unit caches; refuse tracked files or symlinks and preserve supplied tools/Units. |

The local Project edits the real repository `README.md`; saving changes that file. Set `data-source` in the layout to edit another Project-local document. It uses canonical source and pinned released dependencies, including separately installed plugin.fs and ui-service.popup. Editor interaction, syntax highlighting and file persistence need native GUI verification. Missing required Host imports, config or schemas are errors.
