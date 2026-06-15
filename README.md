# AI Chatbot - Intelligent Conversation System

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![Streamlit](https://img.shields.io/badge/Streamlit-1.0+-red.svg)](https://streamlit.io/)
[![OpenAI](https://img.shields.io/badge/OpenAI-API-green.svg)](https://openai.com/)

A modern, interactive web application for intelligent chatbot conversations powered by OpenAI's GPT models. Built with Streamlit for an intuitive user experience with Arabic and English language support.

## 🌟 Features

- 🤖 **AI-Powered Conversations** - Uses OpenAI's GPT models for intelligent responses
- 🌍 **Multilingual Support** - Full support for both Arabic and English
- 💾 **Conversation History** - Maintains and displays chat conversation logs
- ⚙️ **Customizable Personality** - Configure chatbot name and personality traits
- 🎨 **Modern UI** - Clean and responsive interface built with Streamlit
- 🔐 **Secure API Handling** - Environment variable support for API keys
- 📱 **Responsive Design** - Works seamlessly on desktop and mobile devices

## 🛠️ Tech Stack

- **Backend**: Python 3.8+
- **Frontend Framework**: Streamlit
- **AI Model**: OpenAI API (GPT-3.5-turbo / GPT-4)
- **Environment Management**: python-dotenv
- **Dependencies Management**: pip

## 📋 Prerequisites

Before running this project, make sure you have:

- Python 3.8 or higher
- pip (Python package manager)
- An OpenAI API key (get it from [openai.com](https://platform.openai.com/api-keys))
- Git (for cloning the repository)

## 📥 Installation

### 1. Clone the repository

```bash
git clone https://github.com/nadaelkholi29-beep/chatbot-.git
cd chatbot-
```

### 2. Create a virtual environment

```bash
# On Windows
python -m venv venv
venv\Scripts\activate

# On macOS/Linux
python3 -m venv venv
source venv/bin/activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Configure environment variables

Create a `.env` file in the root directory (use `.env.example` as a template):

```bash
cp .env.example .env
```

Edit `.env` and add your OpenAI API key:

```env
OPENAI_API_KEY=sk-your-api-key-here
```

## 🚀 Usage

### Running the Application

```bash
streamlit run app.py
```

The application will open in your default web browser at `http://localhost:8501`

### Using the Chatbot

1. **Start Chatting**: Type your message in the input field at the bottom
2. **Send Message**: Press Enter or click the send button
3. **View History**: All conversations are displayed in the chat window
4. **Clear Chat**: Use the sidebar to start a new conversation

### Example Interactions

**English:**
```
User: Hello, what is artificial intelligence?
Bot: Artificial intelligence (AI) refers to computer systems...
```

**Arabic:**
```
User: مرحبا، ما هو التعليم الآلي؟
Bot: التعليم الآلي (Machine Learning) هو فرع من فروع...
```

## ⚙️ Configuration

### Environment Variables

The application uses the following environment variables:

| Variable | Description | Required |
|----------|-------------|----------|
| `OPENAI_API_KEY` | Your OpenAI API key | Yes |
| `CHATBOT_NAME` | Name of the chatbot (default: "AI Assistant") | No |
| `MODEL_NAME` | OpenAI model to use (default: "gpt-3.5-turbo") | No |
| `TEMPERATURE` | Response creativity (0-2, default: 0.7) | No |
| `MAX_TOKENS` | Maximum response length | No |

### Customization

Edit the configuration in `app.py`:

```python
CHATBOT_NAME = "Your Chatbot Name"
SYSTEM_PROMPT = "Your custom system instructions here"
```

## 📁 Project Structure

```
chatbot-/
├── app.py                 # Main Streamlit application
├── requirements.txt       # Python dependencies
├── .env.example          # Example environment variables
├── README.md             # This file (English)
├── README.ar.md          # Arabic documentation
├── CONTRIBUTING.md       # Contribution guidelines
├── LICENSE               # MIT License
└── docs/                 # Documentation and screenshots
    └── screenshots/      # Application screenshots
```

## 🤝 Contributing

Contributions are welcome! Please follow these guidelines:

1. **Fork the repository**
2. **Create a feature branch** (`git checkout -b feature/amazing-feature`)
3. **Commit your changes** (`git commit -m 'Add amazing feature'`)
4. **Push to the branch** (`git push origin feature/amazing-feature`)
5. **Open a Pull Request**

For detailed contribution guidelines, see [CONTRIBUTING.md](CONTRIBUTING.md)

## 🐛 Known Issues

- API rate limits: OpenAI API has rate limits based on your plan
- Response time: May vary based on API load and response complexity
- Arabic text display: Ensure proper UTF-8 encoding in your terminal

## 🔐 Security Considerations

- Never commit your `.env` file with actual API keys
- Use environment variables for sensitive information
- Keep your OpenAI API key private and secure
- Regularly rotate your API keys
- Review OpenAI's security best practices

## 📊 Performance Tips

- Use `gpt-3.5-turbo` for faster responses and lower costs
- Adjust `temperature` parameter for response consistency
- Monitor your OpenAI API usage in the dashboard
- Consider caching responses for frequently asked questions

## 🔗 Resources

- [Streamlit Documentation](https://docs.streamlit.io/)
- [OpenAI API Documentation](https://platform.openai.com/docs/)
- [Python Documentation](https://docs.python.org/3/)
- [Git Documentation](https://git-scm.com/doc)

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👨‍💼 Author

**Nada Elkholi**
- GitHub: [@nadaelkholi29-beep](https://github.com/nadaelkholi29-beep)
- Email: nadaelkholi29@gmail.com

## 🙏 Acknowledgments

- [OpenAI](https://openai.com/) for the GPT API
- [Streamlit](https://streamlit.io/) for the amazing web framework
- Community contributors and supporters

## 📧 Support

If you encounter any issues or have questions:

1. Check the [Issues page](https://github.com/nadaelkholi29-beep/chatbot-/issues)
2. Review the [CONTRIBUTING.md](CONTRIBUTING.md) file
3. Open a new GitHub issue with detailed information

---

**Made with ❤️ for the AI community**
