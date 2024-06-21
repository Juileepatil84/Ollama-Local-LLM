# Ollama-Local-LLM
## Getting started with Ollama and self-hosting Large Language Models for local AI solutions.

**Welcome to our Ollama Local Setup Tutorial!** I'm Juilee, and I'll be guiding you through installing and configuring Ollama on your own machines. Let's dive in and unlock the full potential of this powerful data processing tool together!

### Setup Steps

## Ollama Website
1. **Visit the Ollama Website**  
   Go to https://ollama.com/

## Download the Installer on Windows
2. **Download the Installer for Windows**  
   Visit [Windows Preview](https://ollama.com/blog/windows-preview) and download the installer. Once downloaded, double-click `OllamaSetup.exe` to start the installation.

## Run Ollama Installer
* Double-click the installer, `OllamaSetup.exe`
* Once installed, go to windows terminal and run any LLM of your choice: `ollama run tinyllama` 
* Once LLM is downloaded it will automatically be served on 'http://localhost:11434' (Ollama’s API automatically runs in the background, serving on `http://localhost:11434`. Tools and applications can connect to it without any additional setup.)
* To serve LLM manually, type in terminal: `ollama serve`
  
## Choice of model:
* Ollama supports numerous models from https://ollama.com/library
* To view downloaded or manually created models, in terminal: `ollama list`
* To remove a model: `ollama rm tinyllama`
  
## Running from Terminal
* To chat with LLM from terminal, open command prompt and type: `ollama run llama2`
* Use Ctrl + d to exit
  
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
