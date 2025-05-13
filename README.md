# 🧠 Static Code Analyzer App

A **Static Code Analyzer** built using **Python** and **Streamlit** to analyze Python source code without executing it. It evaluates code quality, complexity, maintainability, and visualizes important metrics and code structure.

---

## 🚀 Features

- ✅ **Basic Code Metrics**: Lines of code, comments, blank lines, etc. using `radon.raw`.
- 📈 **Maintainability Index & Halstead Metrics**: Measures code quality and difficulty using `radon.metrics`.
- 🔁 **Cyclomatic Complexity**: Analyzes decision complexity with `radon.complexity`.
- 🧠 **Keyword & Identifier Analysis**:
  - Frequency of Python reserved keywords
  - Usage of built-in functions/types
  - Custom identifiers
- 🌳 **AST (Abstract Syntax Tree)**: Parses Python code and visualizes the AST in JSON format.
- 📊 **Visualizations**:
  - Word cloud of keywords and identifiers
  - Bar and pie charts using Altair and Plotly

---

## 🛠️ Technologies Used

- Python 3.10+
- [Streamlit](https://streamlit.io/)
- [Radon](https://pypi.org/project/radon/)
- [WordCloud](https://pypi.org/project/wordcloud/)
- Altair, Plotly, Matplotlib, Pandas, AST



## 🧪 How It Works

The app parses the user's Python code input and performs:
- **Static analysis** using `radon` for maintainability and complexity
- **Tokenization** for keyword and identifier counting
- **AST traversal** using Python’s built-in `ast` module
- **Real-time visualizations** to help users understand their code’s structure and quality

---

## 📁 Project Structure

static-code-analyzer/
│
├── app.py # Main Streamlit app logic
├── ast_parser.py # AST visualization and conversion to JSON
├── utils.py # Token parsing and frequency count functions
├── requirements.txt # Project dependencies
└── .gitignore

