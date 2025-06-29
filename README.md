⚡ Python-to-C++ High Performance Code Translator (with GPT/Claude)



This project converts Python code into highly optimized C++ code using powerful language models like OpenAI GPT (gpt-4o-mini) and Anthropic Claude (claude-3-haiku).


Built with Gradio, this tool provides a live web interface where users can:

 ✅ Paste Python code and instantly see C++ output.
 
 🚀 Compile and run the translated C++.
 
⚡ Compare execution performance between Python and C++ versions.

🔀 Choose between GPT and Claude models for code translation.



✨ Features


 Streamed Code Conversion from Python to C++
 Uses `gpt-4o-mini` and `claude-3-haiku`🖥️ Run both Python and C++ output inside the app
 Autocompiles and benchmarks translated C++ code
 Toggle models interactively
 Example-heavy with compute-intensive test cases



🚀 Quickstart

 Clone the repo


git clone https://github.com/chuksintech/python-to-cpp-translator.git
cd python-to-cpp-translator
 Install dependencies
Make sure Python 3.9+ is installed.

pip install -r requirements.txt

Set up your API keys

   
Create a .env file with your API keys:

touch .env

Inside .env, paste:

env

OPENAI_API_KEY=your-openai-key-here

ANTHROPIC_API_KEY=your-anthropic-key-here

Launch the app

python app.py

Your browser should open automatically. If not, visit http://localhost:7860.

requirements.txt

openai>=1.14.3

anthropic>=0.24.0

google-generativeai>=0.3.2


gradio>=4.20.1

python-dotenv>=1.0.1

⚠️ Notes
The app uses clang++ for compiling C++ code. Ensure it's installed:


clang++ --version

You may need to adjust compilation flags depending on your platform:


-march=armv8.3-a for M1/M2 Macs


-march=native or -mtune=intel for Intel CPUs
