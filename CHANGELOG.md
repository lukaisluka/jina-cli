# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.0.2] - 2025-03-02

### Fixed
- Fix `jina search` returning 0 results due to incomplete JSON parsing
- Implement proper JSON response parsing for Jina Search API
- Add `Accept: application/json` header to search requests

[1.0.2]: https://github.com/geekjourneyx/jina-cli/releases/tag/v1.0.2

## [1.0.1] - 2025-03-02

### Fixed
- Fix GLIBC compatibility issue on Ubuntu 20.04 and older distributions
- Fix version information showing "unknown" for build date and commit hash

### Changed
- Linux builds now use static linking (CGO_ENABLED=0) for maximum compatibility
- Release builds now inject version, build date, and git commit via ldflags

[1.0.1]: https://github.com/geekjourneyx/jina-cli/releases/tag/v1.0.1

## [1.0.0] - 2025-02-28

### Added
- Initial release of jina-cli
- `read` command for extracting content from URLs
- `search` command for AI-powered web search
- `config` command for configuration management
- JSON and Markdown output formats
- Batch URL processing from file
- Configuration file support (`~/.jina-reader/config.yaml`)
- Environment variable overrides
- Image captioning support with VLM
- Proxy support
- CSS selector-based content extraction
- Cookie forwarding
- POST method for SPA applications
- One-line installation script
- Comprehensive test coverage (70%+)

### Features
- Read URLs and convert to LLM-friendly formats (Markdown/HTML/Text)
- Search the web with automatic content fetching from top 5 results
- Site-restricted search
- Cache bypass support
- Configurable timeout settings
- Sensitive data masking in config display

### Documentation
- Bilingual README (Chinese/English)
- CLAUDE.md with development workflow
- MIT License

[1.0.0]: https://github.com/geekjourneyx/jina-cli/releases/tag/v1.0.0
