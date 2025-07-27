# AutoTitle - AI-Powered Title Generator for Obsidian

Automatically generate meaningful titles for your Obsidian notes using OpenAI's powerful language models.

## Features

- 🤖 **AI-Powered Title Generation** - Uses GPT-3.5/GPT-4 to create contextual titles
- 🔄 **Multiple Trigger Modes** - Manual, semi-automatic, or fully automatic generation
- 🌍 **Multi-language Support** - Auto-detect language or choose from supported languages
- ⚡ **Quick Hotkey** - Generate titles instantly with `Ctrl+Shift+H`
- 🎛️ **Customizable Settings** - Adjust AI model, creativity level, and behavior
- 📝 **Smart Integration** - Works seamlessly within your Obsidian workflow

## Installation

1. Open Obsidian Settings
2. Navigate to **Community Plugins** and disable **Safe Mode**
3. Click **Browse** and search for "AutoTitle"
4. Install and enable the plugin

## Setup

### Getting Your OpenAI API Key

1. Sign up at [OpenAI Platform](https://platform.openai.com/)
2. Navigate to [API Keys](https://platform.openai.com/api-keys)
3. Create a new secret key
4. Copy the key to the plugin settings

### Plugin Configuration

1. Open Obsidian Settings
2. Go to **Community Plugins** → **AutoTitle**
3. Enter your OpenAI API key
4. Customize settings to your preference

## Usage

### Quick Start
1. Write some content in your note
2. Press `Ctrl+Shift+H` (Windows/Linux) or `Cmd+Shift+H` (Mac)
3. Review the suggested title and accept or reject it

### Trigger Modes

**Manual Mode** (Default)
- Use hotkey only: `Ctrl+Shift+H`
- Full control over when titles are generated

**Semi-Auto Mode**
- Shows a generation button after you stop typing
- Click the button to generate a title

**Auto Mode**
- Automatically generates titles after typing pause
- Optional notification before generation

### Settings Overview

| Setting | Description | Default |
|---------|-------------|---------|
| **OpenAI API Key** | Your API key for OpenAI access | Required |
| **AI Model** | Choose from GPT-4o, GPT-4.1, GPT-3.5 Turbo | gpt-3.5-turbo |
| **Creativity** | Controls randomness (0.0-1.0) | 0.3 |
| **Trigger Mode** | Manual, Semi-auto, or Auto | Manual |
| **Language** | Target language or auto-detect | Auto |
| **Replace Mode** | Replace without confirmation | Disabled |
| **Min Content Length** | Minimum characters before generation | 100 |
| **Timeout** | Delay after typing (ms) | 5000 |

## Supported Languages

AutoTitle supports title generation in multiple languages:
- English, Spanish, French, German, Italian
- Portuguese, Russian, Chinese, Japanese, Korean
- And many more through auto-detection

## Examples

**Input Note:**
```
Today I learned about the importance of proper sleep hygiene. 
Good sleep habits include maintaining a consistent sleep schedule, 
creating a comfortable sleep environment, and avoiding screens 
before bedtime. These practices can significantly improve sleep 
quality and overall health.
```

**Generated Title:**
```
# The Importance of Sleep Hygiene for Better Health
```

## Troubleshooting

### Plugin Not Working
- Verify your OpenAI API key is correct and active
- Check your OpenAI account has available credits
- Ensure stable internet connection

### Wrong Language Generation
- Set your preferred language in settings instead of auto-detect
- Ensure your note has sufficient content for language detection
- Try different AI models if results are inconsistent

### Auto-generation Issues
- Enable "Auto-generation" in trigger mode settings
- Adjust timeout if generation occurs too frequently or slowly
- Check minimum content length requirement is met

## Privacy & Security

- Your OpenAI API key is stored locally in Obsidian
- Note content is sent to OpenAI only for title generation
- No data is stored or logged by the plugin
- You maintain full control over your API usage and costs

## Support

- **Issues**: Report bugs or request features on GitHub
- **Documentation**: Full documentation available in the repository
- **Community**: Join discussions in Obsidian community forums

## License

MIT License - see the full license in the repository.

---

**Made with ❤️ for the Obsidian community**