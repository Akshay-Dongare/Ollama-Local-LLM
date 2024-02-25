# Ollama-Local-LLM
Getting started with Ollama and self hosting Large Language Models for local AI solutions

## Ollama Website
* https://ollama.com/

## Download the Installer on Windows
* https://ollama.com/blog/windows-preview

## Create new Conda environment 
* `conda create -n llm python`

## Run Ollama Installer
* Double-click the installer, `OllamaSetup.exe`
* Once installed, go to command prompt and pull any LLM of your choice: `ollama pull llama2`
* Once LLM is downloaded it will automatically be served on 'http://localhost:11434' (Ollama’s API automatically runs in the background, serving on `http://localhost:11434`. Tools and applications can connect to it without any additional setup.)
* To serve LLM manually, type in terminal: `ollama serve`

## Running from Terminal
* To chat with LLM from terminal, open command prompt and type: `ollama run llama2`
* Use Ctrl + d or /bye to exit

## Usage with Ollama Python Library (https://github.com/ollama/ollama-python)
* Activate Conda environment with `conda activate llm`
* Run `pip install ollama` on terminal
* Run 

## Usage with llamaindex (https://www.llamaindex.ai/)
* Run `pip install llama-index` on terminal
* If you get `Microsoft Visual C++ 14.0 or greater is required` error , try the solution provided here: https://github.com/Akshay-Dongare/Error-Cpp-Build-Tools
* Run 
