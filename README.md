# Gen-AI-With-Deep-Seek-R1
# 🧠 DeepSeek Code Companion
🚀 Your AI Pair Programmer with Debugging Superpowers

# 📌 Overview
DeepSeek Code Companion is an AI-powered coding assistant designed to help developers with:
✅ Writing Python code
✅ Debugging and troubleshooting
✅ Code documentation
✅ Solution design

This project leverages Streamlit for the UI, LangChain for handling LLM interactions, and Ollama for local model execution.

# ⚙️ Tech Stack
Streamlit – Interactive UI for chat interface
LangChain – Manages LLM prompt processing
Ollama – Runs DeepSeek AI models locally
Python – Backend logic
📂 Project Structure
css
Copy
Edit
📦 DeepSeek-Code-Companion
│── 📜 README.md
│── 📜 requirements.txt
│── 📜 app.py
│── 📂 models
│── 📂 data
│── 📂 assets
# 🚀 Setup & Installation
1️⃣ Clone the repository
bash
Copy
Edit
git clone https://github.com/your-username/deepseek-code-companion.git
cd deepseek-code-companion
# 2️⃣ Install dependencies
bash
Copy
Edit
# pip install -r requirements.txt
3️⃣ Run Ollama (if not installed, install it first)
bash
Copy
Edit
ollama serve
# 4️⃣ Start the Streamlit app
bash
Copy
Edit
streamlit run app.py
🏗 Features
✅ Interactive Chat Interface – Ask coding questions in natural language
✅ AI-Powered Debugging – Get strategic print statements for debugging
✅ Multiple LLM Models – Choose from deepseek-r1:1.5b or deepseek-r1:3b
✅ Code Explanation & Documentation – Understand code better

# 🎨 Customization
🔹 Modify Model Settings
You can adjust the LLM temperature for different response behaviors:

python
Copy
Edit
llm_engine = ChatOllama(
    model=selected_model,
    base_url="http://localhost:11434",
    temperature=0.3
)
Lower values = deterministic responses
Higher values = more creative responses

# 🔹 Modify UI Theme
Custom CSS is included for a dark-themed UI. Modify styles in app.py under:

python
Copy
Edit
st.markdown("""
<style>
    .main { background-color: #1a1a1a; color: #ffffff; }
</style>
""", unsafe_allow_html=True)
💡 Usage Guide
1️⃣ Select an LLM model from the sidebar
2️⃣ Type a coding question in the chat box
3️⃣ View AI-generated solutions & explanations
4️⃣ Use debugging suggestions to fix errors

🛠 Future Improvements
🚀 Add support for more programming languages
🚀 Implement code execution sandbox
🚀 Improve UI/UX with better chat history management

🤝 Contributing
Contributions are welcome! Open a pull request or submit an issue to suggest improvements.

# 📜 License
This project is licensed under the MIT License.
