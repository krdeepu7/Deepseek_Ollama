# Running Deepseek Locally on Windows

## Overview
This guide explains how to run **Deepseek** locally on a Windows machine using **Ollama** and **Open WebUI**. This setup allows you to experiment with Large Language Models (LLMs) without cloud dependencies, enabling local AI development and testing.

## Prerequisites
- A Windows machine with **64-bit architecture**
- Basic familiarity with **PowerShell** and **command-line interfaces**

## Installation Steps

### 1. Download and Install Ollama
Ollama is a tool for running LLMs locally. Download and install it from the official site:

🔗 [Download Ollama](https://ollama.com/download/windows)

### 2. Run Deepseek Models with Ollama
Once installed, you can start running models with the following command:

```powershell
ollama run deepseek-r1:1.5b
```

### 3. Pull Deepseek Model
To download a larger Deepseek model (7B parameters), use:

```powershell
ollama pull deepseek-r1:7b
```

### 4. Install `uv` (A Faster Python Package Manager)
Install `uv` using PowerShell:

```powershell
powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"
```

### 5. Install and Run Open WebUI
Open WebUI provides a user-friendly interface for running LLMs locally.

#### Install Open WebUI:
```powershell
$env:DATA_DIR="C:\open-webui\data"; uvx --python 3.11 open-webui@latest serve
```

### 6. Open the Web Interface
Once the installation is complete, access Open WebUI in your browser:

🔗 **http://localhost:9090**

## Usage
- **Interact with Deepseek models** through the command line using Ollama.
- **Use Open WebUI** for a graphical interface to test and fine-tune models.

## Future Improvements
- Explore **custom model fine-tuning** on local datasets.
- Integrate **Deepseek models into AI solutions** at [Retarns.com](https://retarns.com).

## License
This project follows the respective licenses of **Ollama, Deepseek, and Open WebUI**. Ensure compliance when using these tools.

---
🚀 **Happy Coding!** Follow my journey in **#100DaysOfCode** for more AI explorations!

