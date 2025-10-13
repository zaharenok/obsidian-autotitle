# AutoTitle - AI-Powered Title Generator for Obsidian

Automatically generate meaningful titles for your Obsidian notes using OpenAI's latest and most powerful language models.

## 🚀 Features

- 🤖 **Latest AI Models** - Powered by OpenAI's GPT-4o family plus GPT-4 Turbo, GPT-4, and GPT-3.5 Turbo
- 🔄 **Flexible Generation Modes** - Manual, semi-automatic, or fully automatic title generation
- 🌍 **Multi-language Support** - Auto-detect language or choose from 20+ supported languages
- ⚡ **Instant Generation** - Quick hotkey access with `Ctrl+Shift+H` (Windows/Linux) or `Cmd+Shift+H` (Mac)
- 🎛️ **Customizable Settings** - Fine-tune AI behavior, creativity level, and generation preferences
- 📝 **Smart Integration** - Seamlessly integrates with your existing Obsidian workflow
- 🔒 **Privacy-First** - Your API key stays local, no data logging or storage
- ✨ **Duplicate Prevention** - Automatically prevents duplicate titles in note content
- 🔧 **Migration Tools** - Fix existing notes with duplicate titles
- 🚀 **Batch Processing** - Generate titles for multiple notes simultaneously
- 🎯 **Smart Context** - Analyzes note content intelligently for better title generation
- ⚙️ **Advanced Configuration** - Temperature control, timeout settings, and generation limits

## 📦 Installation

### From Obsidian Community Plugins (Recommended)

1. Open **Obsidian Settings** (⚙️ icon or `Ctrl/Cmd + ,`)
2. Navigate to **Community Plugins** in the left sidebar
3. Disable **Safe Mode** if it's currently enabled
4. Click **Browse** and search for **"AutoTitle"**
5. Click **Install** and then **Enable**
6. Configure your OpenAI API key in the plugin settings

### Manual Installation

1. Download the latest release files (`main.js`, `manifest.json`, `styles.css`) from the [releases page](https://github.com/zaharenok/obsidian-autotitle/releases)
2. Navigate to your Obsidian vault folder
3. Create the plugins directory: `YourVault/.obsidian/plugins/autotitle/`
4. Copy the downloaded files to this folder
5. Restart Obsidian
6. Go to **Settings** → **Community Plugins** → **AutoTitle** and enable the plugin
7. Configure your OpenAI API key in the plugin settings

## ⚙️ Setup & Configuration

### Getting Your OpenAI API Key

1. Visit [OpenAI Platform](https://platform.openai.com/)
2. Sign up or log in to your account
3. Navigate to [API Keys](https://platform.openai.com/api-keys)
4. Click **"Create new secret key"**
5. Copy the generated key (starts with `sk-`)

### Plugin Configuration

1. Open **Obsidian Settings**
2. Go to **Community Plugins** → **AutoTitle**
3. Paste your OpenAI API key
4. Configure your preferred settings

## 🎯 Usage Guide

### Quick Start

1. Write content in your note (minimum 100 characters recommended)
2. Press `Ctrl+Shift+H` (Windows/Linux) or `Cmd+Shift+H` (Mac)
3. Review the AI-generated title suggestion
4. Click **Accept** to apply or **Reject** to dismiss

### Generation Modes

#### Manual Mode (Default)

- **Best for**: Full control over title generation
- **How it works**: Use hotkey only when you want a title
- **Recommended for**: Users who prefer explicit control

#### Semi-Auto Mode

- **Best for**: Balanced automation with user control
- **How it works**: Shows generation button after typing pause
- **Recommended for**: Users who want suggestions without interruption

#### Auto Mode

- **Best for**: Seamless, hands-free experience
- **How it works**: Automatically generates titles after typing pause
- **Recommended for**: Power users who want maximum automation

### Available Commands

- **Generate title for note** (`Ctrl+Shift+H`) - Generate title with confirmation
- **Generate title without confirmation** (`Ctrl+Shift+Alt+H`) - Direct title application
- **Fix duplicate titles in all notes** - Batch fix existing notes with duplicate titles
- **Fix duplicate title in current note** - Fix current note only
- **Reset rejected files** - Allow auto-generation for previously rejected notes

## 🤖 AI Models Explained

### GPT-4o (Recommended)

- **Best for**: High-quality, nuanced titles with superior reasoning
- **Strengths**: Excellent understanding of context, tone, and multimodal capabilities, 128K context window
- **Cost**: Standard pricing (~$0.0005-0.002 per title)
- **Use when**: You want the best balance of quality and performance for most use cases

### GPT-4o-mini (Cost-Effective)

- **Best for**: Fast, cost-effective generation with excellent quality
- **Strengths**: Excellent balance of quality and speed, 128K context window, latest model
- **Cost**: Most budget-friendly option (~$0.00015-0.0006 per title)
- **Use when**: You need frequent title generation at low cost without sacrificing quality

### GPT-4 Turbo

- **Best for**: Complex content requiring deep understanding
- **Strengths**: Enhanced reasoning, large context window (128K tokens)
- **Cost**: Premium pricing
- **Use when**: Working with complex, technical, or lengthy content

### GPT-4

- **Best for**: Highest quality output for critical content
- **Strengths**: Superior reasoning and creativity
- **Cost**: Premium pricing
- **Use when**: Quality is more important than speed or cost

### GPT-3.5 Turbo

- **Best for**: Basic title generation needs
- **Strengths**: Fast and economical with broad availability
- **Cost**: Lowest cost option (~$0.0001-0.0004 per title)
- **Use when**: Budget is the primary concern or when the note requires only light summarization

> **Note:** GPT-5 and GPT-4.1 models are not yet available in the plugin UI. Support will be added once OpenAI exposes stable API endpoints for those models.

## ⚙️ Settings Reference

| Setting                      | Description                                 | Options                                                  | Default     |
| ---------------------------- | ------------------------------------------- | -------------------------------------------------------- | ----------- |
| **OpenAI API Key**           | Your personal API key                       | Text input                                               | Required    |
| **AI Model**                 | Choose the AI model                         | GPT-4o, GPT-4o-mini, GPT-4 Turbo, GPT-4, GPT-3.5 Turbo | GPT-4o-mini |
| **Creativity (Temperature)** | Controls randomness in generation           | 0.0 (conservative) - 1.0 (creative)                      | 0.3         |
| **Trigger Mode**             | How titles are generated                    | Manual, Semi-auto, Auto                                  | Manual      |
| **Language**                 | Target language for titles                  | Auto-detect, English, Spanish, French, etc.              | Auto-detect |
| **Replace Mode**             | Skip confirmation dialog                    | On/Off                                                   | Off         |
| **Min Content Length**       | Minimum characters before generation        | Number (characters)                                      | 100         |
| **Timeout**                  | Delay after typing stops                    | Milliseconds                                             | 5000        |
| **Show Indicator**           | Display notification before auto-generation | On/Off                                                   | On          |
| **Generation Count**         | Max generations per note                    | Number                                                   | 1           |
| **Max Title Length**         | Maximum characters for generated titles     | Number (characters)                                      | 100         |
| **Include Existing Title**   | Consider existing title during generation   | On/Off                                                   | Off         |

## 🌍 Supported Languages

AutoTitle automatically detects and generates titles in:

**European Languages:**
- English, Spanish, French, German, Italian, Portuguese, Russian, Polish, Dutch, Swedish, Norwegian, Danish

**Asian Languages:**
- Chinese (Simplified & Traditional), Japanese, Korean, Hindi, Bengali, Arabic, Thai, Vietnamese

**And many more through intelligent auto-detection!**

## 💡 Usage Examples

### Academic Note

**Input:**
```
The concept of neuroplasticity refers to the brain's ability to reorganize
itself by forming new neural connections throughout life. This remarkable
capacity allows the brain to compensate for injury and disease and to
adjust their activities in response to new situations or changes in their
environment.
```

**Generated Title:**
```
# Understanding Neuroplasticity: The Brain's Ability to Adapt and Reorganize
```

### Meeting Notes

**Input:**
```
Discussed Q4 marketing strategy with the team. Key points: increase social
media presence, launch influencer partnerships, focus on video content,
and allocate 30% more budget to digital advertising. Next steps include
creating content calendar and identifying potential influencers.
```

**Generated Title:**
```
# Q4 Marketing Strategy Meeting: Social Media and Influencer Focus
```

### Personal Journal

**Input:**
```
Today was challenging but rewarding. Started the morning with meditation,
which helped center my thoughts. The presentation at work went better than
expected, and I received positive feedback from the team. Feeling grateful
for the support and looking forward to tomorrow's challenges.
```

**Generated Title:**
```
# A Challenging Yet Rewarding Day: Meditation, Success, and Gratitude
```

## 🔧 Troubleshooting

### Common Issues

#### "API Key Invalid" Error
- **Solution**: Verify your API key is correct and active
- **Check**: Ensure the key starts with `sk-` and has no extra spaces or line breaks
- **Verify**: Log into [OpenAI Platform](https://platform.openai.com/api-keys) to confirm key status
- **Note**: API keys are case-sensitive and must be copied exactly

#### "Insufficient Credits" Error
- **Solution**: Add credits to your OpenAI account
- **Check**: Visit [OpenAI Billing](https://platform.openai.com/account/billing)
- **Note**: New accounts include $5 in free credits (as of 2024)
- **Tip**: Monitor your usage in the OpenAI dashboard to avoid unexpected charges

#### Titles in Wrong Language
- **Solution**: Set specific language instead of auto-detect
- **Tip**: Ensure your note has enough content for accurate detection
- **Alternative**: Try different AI models for better language handling

#### Auto-generation Not Working
- **Check**: Trigger mode is set to "Auto" or "Semi-auto"
- **Verify**: Content meets minimum length requirement
- **Adjust**: Increase timeout if generation happens too quickly
- **Test**: Try manual generation first to verify setup

#### Slow Generation
- **Solution**: Switch to GPT-4o-mini for faster responses
- **Check**: Your internet connection stability
- **Consider**: OpenAI API response times vary by demand

#### Duplicate Titles Issue
- **Solution**: Use the "Fix duplicate titles" commands in settings
- **Prevention**: The plugin now automatically prevents new duplicates
- **Migration**: Run the migration tool to fix existing notes

#### "Rate Limit Exceeded" Error
- **Solution**: Wait a few minutes before trying again
- **Check**: Monitor your API usage in the OpenAI dashboard
- **Tip**: Consider switching to GPT-4o-mini for higher rate limits
- **Note**: Rate limits vary by model and account type

#### Plugin Not Appearing in Settings
- **Solution**: Ensure the plugin is properly installed in the correct directory
- **Check**: Verify files are in `YourVault/.obsidian/plugins/autotitle/`
- **Restart**: Completely restart Obsidian after installation
- **Enable**: Manually enable the plugin in Community Plugins settings

### Performance Tips

1. **For Speed**: Use GPT-4o-mini model
2. **For Quality**: Use GPT-4o model
3. **For Cost**: Use GPT-4o-mini or GPT-3.5 Turbo
4. **For Latest Features**: Monitor OpenAI announcements; new models will be added once stable
5. **For Accuracy**: Provide more context in your notes
6. **For Consistency**: Set specific language instead of auto-detect

## 🔒 Privacy & Security

- **Local Storage**: Your API key is stored only in your local Obsidian settings
- **No Logging**: The plugin doesn't log or store any of your content
- **Direct Communication**: Your notes are sent directly to OpenAI's API
- **User Control**: You control what content is sent for title generation
- **No Tracking**: No analytics or usage tracking implemented

## 💰 Cost Considerations

Title generation costs depend on your chosen model (as of 2024):

- **GPT-4o-mini**: ~$0.00015-0.0006 per title (most economical)
- **GPT-3.5 Turbo**: ~$0.0001-0.0002 per title (budget-friendly)
- **GPT-4o**: ~$0.0005-0.002 per title (recommended)
- **GPT-4 Turbo**: ~$0.001-0.004 per title (premium)
- **GPT-4**: ~$0.002-0.006 per title (high quality)

_Costs are approximate and depend on content length. OpenAI pricing may change over time. Check [OpenAI Pricing](https://openai.com/pricing) for current rates._

## 🆘 Support & Community

### Getting Help

- **GitHub Issues**: [Report bugs or request features](https://github.com/zaharenok/obsidian-autotitle/issues)
- **GitHub Discussions**: [Join community discussions](https://github.com/zaharenok/obsidian-autotitle/discussions)
- **Obsidian Forum**: Search for "AutoTitle" in community discussions
- **Documentation**: Comprehensive guides available in the repository
- **Discord**: Join the Obsidian Discord server and search for "AutoTitle"

### Contributing

- **Feedback**: Share your experience and suggestions
- **Bug Reports**: Help improve the plugin by reporting issues
- **Feature Requests**: Suggest new functionality

## 📄 License

MIT License - See the repository for full license details.

## 🙏 Acknowledgments

- **OpenAI** for providing powerful language models
- **Obsidian Team** for creating an amazing platform
- **Community Contributors** for feedback and suggestions
- **Plugin Users** for making this project worthwhile

---

**Made with ❤️ for the Obsidian community**

_Transform your note-taking with AI-powered titles. Install AutoTitle today and experience the future of intelligent note organization._