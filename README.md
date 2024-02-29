# Ollama-Local-LLM
Getting started with Ollama and self hosting Large Language Models for local AI solutions

# Setup Steps

## Create new Conda environment 
* `conda create -n llm python`

## Activate Conda environment
* `conda activate llm`

## Install All Requirements
* In terminal, `pip install -r requirements.txt`
* `requirements.txt` contains ollama python library, llama-index ollama library, jupyter notebook and llama-index
* If you get `Microsoft Visual C++ 14.0 or greater is required` error , try the solution provided here: https://github.com/Akshay-Dongare/Error-Cpp-Build-Tools and run above command again

## Ollama Website
* https://ollama.com/

## Download the Installer on Windows
* https://ollama.com/blog/windows-preview

## Run Ollama Installer
* Double-click the installer, `OllamaSetup.exe`
* Once installed, go to command prompt and pull any LLM of your choice: `ollama pull llama2` (Size: 3.8GB)
* Once LLM is downloaded it will automatically be served on 'http://localhost:11434' (Ollama’s API automatically runs in the background, serving on `http://localhost:11434`. Tools and applications can connect to it without any additional setup.)
* To serve LLM manually, type in terminal: `ollama serve`
  
## Choice of model:
* Ollama supports numerous models from https://ollama.com/library
* To view downloaded or manually created models, in terminal: `ollama list`
* To remove a model: `ollama rm llama2`
  
## Running from Terminal
* To chat with LLM from terminal, open command prompt and type: `ollama run llama2`
* Use Ctrl + d or /bye to exit
  
### Display the model file of any model
* `ollama show {model_name} --modelfile`
* Example: `ollama show llama2 --modelfile`

## Create custom model by changing model file
* To create a custom modelfile, follow the format in the model's original model file and change the instructions (system prompt)
* Now, `ollama create {custom_model_name} --file {path_to_modelfile}`
* Check custom model by, `ollama list` in terminal

## Usage with Ollama Python Library (https://github.com/ollama/ollama-python)
* Activate Conda environment with `conda activate llm`
* Check out the starter code in this repo at: `./ollama-python.ipynb` 

## Usage with llamaindex (https://www.llamaindex.ai/)
* Activate Conda environment with `conda activate llm`
* Check out the starter code in this repo at: `./ollama-llamaindex.ipynb` 
