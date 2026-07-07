The purpose fo this work is to test which local models are best at writing 
knowledge transfer docs and config files

Each model is inputed the same prompt below:

Create two files in the current working directory (do not create any subdirectories unless specified):

1. instruction.md
2. config.yml

## instruction.md

Create a beginner-friendly guide explaining how to use Aider with Ollama.

Include the following sections:

### 1. Prerequisites
- Install Ollama
- Install Aider
- Verify both installations

Include example commands such as:

ollama --version
aider --version

### 2. Downloading a Model

Explain how to download a model using Ollama.

Include examples:

ollama pull qwen2.5-coder:7b
ollama pull llama3.1:8b
ollama list

Briefly explain what each command does.

### 3. Running Aider with Ollama

Explain how to navigate to a project directory.

Example:

cd my-project

Show how to launch Aider using different Ollama models.

Examples:

aider --model ollama_chat/qwen2.5-coder:7b

aider --model ollama_chat/llama3.1:8b

aider --model ollama_chat/gemma3:4b

Explain that Aider will use the selected local Ollama model for the session.

### 4. Helpful Commands

Include examples for:

ollama list
ollama ps
ollama stop <model>
aider --help

Briefly explain each command.

---

## config.yml

Create a sample configuration file showing how users can configure Aider to use different Ollama models.

Include several commented examples, such as:

- qwen2.5-coder:7b
- llama3.1:8b
- gemma3:4b
- deepseek-coder
- phi3

Show how to switch the default model by changing a single configuration value.

Add comments explaining what each model is best suited for (general coding, web development, reasoning, lightweight, etc.).

The `config.yml` should be intended as a reference/example only and should be heavily commented so users understand how to customize it.
