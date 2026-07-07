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
