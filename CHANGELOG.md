# Changelog

All notable changes to AutoTitle plugin will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.0.0] - 2025-10-14

### Added
- Automatic title generation using OpenAI GPT models (GPT-4o, GPT-4o-mini, GPT-4 Turbo, GPT-4)
- Multiple trigger modes: Manual (hotkey only), Semi-auto (button after pause), Auto (after typing pause)
- Multi-language support with automatic language detection
- Customizable generation parameters (temperature, timeout, minimum content length)
- Smart duplication handling to prevent duplicate titles
- Auto-ignore functionality for processed notes
- Manual and automatic replace modes
- Configurable maximum title length
- Support for including existing titles in generation context
- Comprehensive settings panel with real-time configuration
- Cross-platform compatibility (Windows, macOS, Linux, Android, iOS)

### Features
- **AI Models**: Support for latest OpenAI models including GPT-4o and GPT-4o-mini
- **Language Support**: Auto-detection for European languages (English, Spanish, French, German, Italian, Portuguese, Russian, Polish, Dutch, Swedish, Norwegian, Danish) and Asian languages (Chinese, Japanese, Korean, Hindi, Bengali, Arabic, Thai, Vietnamese)
- **Smart Generation**: Configurable minimum content length (default: 100 characters)
- **Customizable Timing**: Adjustable timeout delay after typing stops (default: 5000ms)
- **User Control**: Multiple generation count support with ignore list management
- **Interface**: Intuitive settings panel with usage instructions and hotkey reference
- **Performance**: Optimized for responsiveness with indicator notifications

### Security
- Secure API key storage
- No data collection or external transmission beyond OpenAI API calls
- Local processing and settings storage

### Compatibility
- Minimum app version: 0.15.0
- Supports both desktop and mobile platforms
- Compatible with Obsidian's latest API standards

### Documentation
- Comprehensive README with installation and usage instructions
- Clear configuration guidelines
- Troubleshooting and FAQ section
- Developer attribution and license information