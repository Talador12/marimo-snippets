# Changelog

## [1.0.4] - 2024-12-19

### Added
- **Markdown support**: Added proper detection and rendering of markdown code blocks in marimo snippets
  - Code blocks with `language-md` or `language-markdown` classes are now properly detected and rendered as markdown cells
  - Markdown cells are automatically wrapped with `mo.md()` and have `hide_code=True` set
  - The `marimo as mo` import is automatically added when markdown cells are present
  - Both `<marimo-button>` and `<marimo-iframe>` elements now support markdown code blocks
  - Mixed Python and Markdown cells can be used together in the same notebook

### Fixed
- Fixed typo in package.json "files" field (was "exctractor.js", now "extractor.js")

### Documentation
- Added comprehensive documentation and examples for markdown support in README.md
- Added example showing mixed Python and Markdown cells in the same notebook

This release addresses GitHub issue #17: "Enable language based marimo snippets, namely Markdown" 