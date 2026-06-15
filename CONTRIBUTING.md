# Contributing to AI Chatbot

First off, thank you for considering contributing to the AI Chatbot project! It's people like you that make this such a great tool.

## Code of Conduct

This project and everyone participating in it is governed by our Code of Conduct. By participating, you are expected to uphold this code. Please report unacceptable behavior to [nadaelkholi29@gmail.com](mailto:nadaelkholi29@gmail.com).

## How Can I Contribute?

### Reporting Bugs

Before creating bug reports, please check the issue list as you might find out that you don't need to create one. When you are creating a bug report, please include as many details as possible:

* **Use a clear and descriptive title**
* **Describe the exact steps which reproduce the problem**
* **Provide specific examples to demonstrate the steps**
* **Describe the behavior you observed after following the steps**
* **Explain which behavior you expected to see instead and why**
* **Include screenshots and animated GIFs if possible**
* **Include your environment details:**
  - Operating System
  - Python version
  - Streamlit version
  - OpenAI API version

### Suggesting Enhancements

Enhancement suggestions are tracked as GitHub issues. When creating an enhancement suggestion, please include:

* **Use a clear and descriptive title**
* **Provide a step-by-step description of the suggested enhancement**
* **Provide specific examples to demonstrate the steps**
* **Describe the current behavior and the expected behavior**
* **Explain why this enhancement would be useful**

### Pull Requests

* Fill in the required template
* Follow the Python and code style guide
* Include appropriate test cases
* End all files with a newline
* Document new code based on the Documentation Styleguide

## Development Setup

### Prerequisites

- Python 3.8 or higher
- pip
- Virtual environment tool (venv)
- Git

### Steps

1. **Fork the repository**
   ```bash
   git clone https://github.com/yourusername/chatbot-.git
   cd chatbot-
   ```

2. **Create a virtual environment**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   pip install -r requirements-dev.txt  # For development tools
   ```

4. **Create a branch for your changes**
   ```bash
   git checkout -b feature/your-feature-name
   ```

5. **Make your changes**

6. **Test your changes**
   ```bash
   streamlit run app.py
   ```

7. **Commit your changes**
   ```bash
   git commit -m "Add your commit message"
   ```

8. **Push to your fork**
   ```bash
   git push origin feature/your-feature-name
   ```

9. **Submit a Pull Request**

## Styleguides

### Git Commit Messages

* Use the present tense ("Add feature" not "Added feature")
* Use the imperative mood ("Move cursor to..." not "Moves cursor to...")
* Limit the first line to 72 characters or less
* Reference issues and pull requests liberally after the first line
* Consider starting the commit message with an applicable emoji:
  - 🎨 `:art:` when improving the format/structure of the code
  - 🚀 `:rocket:` when improving performance
  - 📚 `:books:` when writing docs
  - 🐛 `:bug:` when fixing a bug
  - ✨ `:sparkles:` when introducing a new feature
  - ⚙️ `:gear:` when configuring something
  - 🔒 `:lock:` when dealing with security
  - ✅ `:white_check_mark:` when adding tests

### Python Styleguide

All Python code must adhere to [PEP 8](https://www.python.org/dev/peps/pep-0008/):

* Use 4 spaces for indentation
* Use snake_case for variable and function names
* Use PascalCase for class names
* Add docstrings to all functions and classes
* Use type hints where possible
* Keep lines under 100 characters

**Example:**

```python
def process_message(user_input: str) -> str:
    """
    Process user input and return chatbot response.
    
    Args:
        user_input: The message from the user
        
    Returns:
        The chatbot's response message
    """
    response = client.chat.completions.create(
        model="gpt-3.5-turbo",
        messages=[{"role": "user", "content": user_input}]
    )
    return response.choices[0].message.content
```

### Documentation Styleguide

* Use clear, concise language
* Write in second person ("you" instead of "I" or "we")
* Use examples to illustrate points
* Include both English and Arabic documentation
* Use markdown formatting consistently

## Testing

* Write tests for new features
* Ensure all tests pass before submitting a PR
* Maintain or improve code coverage
* Run tests locally: `pytest` (if implemented)

## Pull Request Process

1. Update the README.md with any new features or API changes
2. Update the CHANGELOG.md with notes on your changes
3. Ensure your code follows the styleguides
4. Make sure all tests pass
5. Add a clear description of what your PR does
6. Link any related issues
7. Request review from maintainers

## Additional Notes

### Issue and Pull Request Labels

* `bug` - Something isn't working
* `enhancement` - New feature or request
* `documentation` - Improvements or additions to documentation
* `good first issue` - Good for newcomers
* `help wanted` - Extra attention is needed
* `question` - Further information is requested
* `wontfix` - This will not be worked on

### Community

* Be respectful and welcoming to all community members
* Assume good intentions in discussions
* Provide constructive feedback
* Ask questions if you don't understand something

## Licensing

By contributing to this project, you agree that your contributions will be licensed under the MIT License.

## Questions?

Feel free to contact the maintainers or open an issue with your questions.

Thank you for contributing! 🎉
