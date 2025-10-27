# AI Genius - Your Intelligent Companion 🤖

<div align="center">
  <img src="assets/icon/app_icon.png" alt="AI Genius Logo" width="150"/>
  
  [![Flutter](https://img.shields.io/badge/Flutter-3.35.7-02569B?logo=flutter)](https://flutter.dev)
  [![Dart](https://img.shields.io/badge/Dart-3.9.2-0175C2?logo=dart)](https://dart.dev)
  [![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
</div>

## 📱 About

**AI Genius** (Digital Twin AI) is an advanced AI-powered chat application built with Flutter. It provides intelligent conversations, creative solutions, and helpful insights powered by state-of-the-art AI models.

### ✨ Key Features

- 🤖 **Smart AI Conversations** - Powered by Groq API (LLaMA 3.3 70B)
- 🖼️ **Image Analysis** - Analyze images with Google Gemini Vision
- 🎤 **Voice Chat** - Speech-to-text and text-to-speech capabilities
- 📝 **Templates** - Pre-built templates for various tasks
- 🔍 **Search** - Search through your conversation history
- 📤 **Export** - Export conversations as TXT, MD, or PDF
- 🌍 **Bilingual** - Full support for English and Arabic
- 🎨 **Customizable Themes** - 6 color schemes and 4 theme modes
- 💾 **Local Storage** - All conversations saved locally with Hive

## 🚀 Getting Started

### Prerequisites

- Flutter SDK 3.35.7 or higher
- Dart 3.9.2 or higher
- Android Studio / VS Code
- Git

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/ai-genius.git
   cd ai-genius
   ```

2. **Install dependencies**
   ```bash
   flutter pub get
   ```

3. **Configure environment variables**
   
   Copy `.env.example` to `.env` and add your API keys:
   ```bash
   cp .env.example .env
   ```
   
   Edit `.env` file:
   ```env
   GROQ_API_KEY=your_groq_api_key_here
   GOOGLE_AI_API_KEY=your_google_ai_api_key_here
   ```

4. **Run the app**
   ```bash
   flutter run
   ```

## 🔑 API Keys Setup

### Groq API (Required)
1. Visit [Groq Console](https://console.groq.com)
2. Create an account and generate an API key
3. Add the key to your `.env` file

### Google AI API (Optional - for image analysis)
1. Visit [Google AI Studio](https://makersuite.google.com/app/apikey)
2. Create an API key
3. Add the key to your `.env` file

## 🏗️ Project Structure

```
lib/
├── core/
│   ├── config/          # Environment configuration
│   ├── localization/    # Multi-language support
│   ├── services/        # Core services (TTS, Permissions, Network)
│   └── theme/           # App theming
├── features/
│   ├── chat/
│   │   ├── data/        # Repositories & Services
│   │   ├── domain/      # Models & Business Logic
│   │   └── presentation/# UI & State Management
│   ├── home/            # Home screen
│   ├── settings/        # Settings screens
│   ├── onboarding/      # Onboarding flow
│   └── splash/          # Splash screen
└── main.dart            # App entry point
```

## 🛠️ Technologies Used

### Core
- **Flutter** - UI Framework
- **Dart** - Programming Language

### State Management
- **flutter_bloc** - BLoC Pattern
- **provider** - State Management
- **equatable** - Value Equality

### Storage
- **hive** - Local NoSQL Database
- **shared_preferences** - Settings Storage

### AI & Networking
- **dio** - HTTP Client
- **google_generative_ai** - Google AI SDK
- **Groq API** - LLaMA 3.3 70B Model

### UI/UX
- **flutter_chat_ui** - Chat Interface
- **flutter_animate** - Animations
- **lottie** - JSON Animations
- **iconsax** - Modern Icons
- **google_fonts** - Poppins Font

### Media & Files
- **image_picker** - Image Selection
- **file_picker** - File Selection
- **flutter_tts** - Text-to-Speech
- **speech_to_text** - Speech Recognition
- **record** - Audio Recording

### Utilities
- **connectivity_plus** - Network Status
- **permission_handler** - Permissions Management
- **share_plus** - Share Functionality
- **pdf** - PDF Generation
- **flutter_dotenv** - Environment Variables

## 🎨 Features in Detail

### Chat Contexts
- **General** - All-purpose conversations
- **Brainstorm** - Creative idea generation
- **Explain** - Detailed explanations
- **Learn Code** - Programming assistance
- **Companion** - Friendly conversations

### Theme Customization
- **Modes**: System, Light, Dark, AMOLED
- **Colors**: Indigo, Blue, Green, Pink, Orange, Purple

### Export Formats
- **Text** (.txt) - Simple text format
- **Markdown** (.md) - Formatted markdown
- **PDF** (.pdf) - Professional documents

## 🔒 Security & Privacy

- ✅ API keys stored in `.env` (not committed to Git)
- ✅ All conversations stored locally
- ✅ No data sent to external servers (except AI APIs)
- ✅ Permissions requested only when needed

## 🌍 Localization

Supported languages:
- 🇬🇧 English
- 🇸🇦 Arabic (العربية)

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👨‍💻 Developer

**Mina Nasser Kamal**
- 🇪🇬 Made with ❤️ in Egypt

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📞 Support

If you have any questions or issues, please open an issue on GitHub.

## 🙏 Acknowledgments

- Flutter Team for the amazing framework
- Groq for providing fast AI inference
- Google for Gemini AI
- All open-source contributors

---

<div align="center">
  Made with ❤️ using Flutter
</div>
