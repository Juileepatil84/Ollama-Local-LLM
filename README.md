# Ollama-Local-LLM
## Getting Started with Ollama and Self-Hosting Large Language Models for Local AI Solutions

**Welcome to our Ollama Local Setup Tutorial!** I'm Juilee, and I'll be guiding you through installing and configuring Ollama on your own machines. Let's dive in and unlock the full potential of this powerful data processing tool together!

For detailed visual instructions, please refer to the **[Ollama Setup PDF](https://github.com/Juileepatil84/Ollama-Local-LLM/blob/main/Ollama%20setup.pdf)** which contains step-by-step images to aid in installation and configuration.

### Watch Our Detailed Video Tutorial
For a comprehensive guide and step-by-step walkthrough, check out our **[Ollama Setup YouTube Tutorial](https://youtu.be/tOGH7vNCO4U)**.

### Setup Steps

### Setup Steps

## Ollama Website
1. **Visit the Ollama Website**  
   Go to [ollama.com](https://ollama.com/)

## Download the Installer on Windows
2. **Download the Installer for Windows**  
   Visit the [Windows Preview](https://ollama.com/blog/windows-preview) and download the installer. Once downloaded, double-click `OllamaSetup.exe` to start the installation.

## Run Ollama Installer
* Once installed, go to Windows Terminal and run any LLM of your choice: `ollama run tinyllama`.
* Pass the prompt to the model and it will return a response in return.
* Once LLM is downloaded it will automatically be served on 'http://localhost:11434' (Ollama’s API automatically runs in the background, serving on `http://localhost:11434`. Tools and applications can connect to it without any additional setup).
* To serve LLM manually, type in terminal: `ollama serve`.
  
## Choice of Model
* Ollama supports numerous models from [ollama.com/library](https://ollama.com/library).
* To view downloaded or manually created models, in terminal: `ollama list`.
* To remove a model: `ollama rm tinyllama`. Specify name of model you want to delete.
  
## Running from Terminal
* Use Ctrl + D to exit.
* Follow same steps to download new model.
* You call also use `ollama pull llama2` download and to chat with LLM from the terminal, open terminal and type: `ollama run llama2`.

  
### Display the Model File of Any Model
* `ollama show {model_name} --modelfile`.
* Example: `ollama show llama2 --modelfile`.

## Create Custom Model by Changing Model File
* To create a custom modelfile, follow the format in the model's original model file and change the instructions (system prompt).
* Now, `ollama create {custom_model_name} --file {path_to_modelfile}`.
* Check custom model by, `ollama list` in terminal.

## Usage with Ollama Python Library
* Activate Conda environment with `conda activate llm`.
* Check out the starter code in this repo at: `./ollama-python.ipynb` [Ollama Python Library](https://github.com/ollama/ollama-python).

## Usage with Llamaindex
* Activate Conda environment with `conda activate llm`.
* Check out the starter code in this repo at: `./ollama-llamaindex.ipynb` [Llamaindex](https://www.llamaindex.ai/).
