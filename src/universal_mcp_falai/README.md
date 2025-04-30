# Universal Mcp Fal AI MCP Server

An MCP Server for the Universal Mcp Fal AI API.

## 📋 Prerequisites

Before you begin, ensure you have met the following requirements:
* Python 3.11+ (Recommended)
* [uv](https://github.com/astral-sh/uv) installed globally (`pip install uv`)

## 🛠️ Setup Instructions

Follow these steps to get the development environment up and running:

### 1. Sync Project Dependencies
Navigate to the project root directory (where `pyproject.toml` is located).
```bash
uv sync
```
This command uses `uv` to install all dependencies listed in `pyproject.toml` into a virtual environment (`.venv`) located in the project root.

### 2. Activate the Virtual Environment
Activating the virtual environment ensures that you are using the project's specific dependencies and Python interpreter.
- On **Linux/macOS**:
```bash
source .venv/bin/activate
```
- On **Windows**:
```bash
.venv\\Scripts\\activate
```

### 3. Start the MCP Inspector
Use the MCP CLI to start the application in development mode.
```bash
mcp dev src/universal_mcp_falai/mcp.py
```
The MCP inspector should now be running. Check the console output for the exact address and port.

## 🔌 Supported Integrations

- AgentR
- API Key (Coming Soon)
- OAuth (Coming Soon)

## 🛠️ Tool List

This is automatically generated from OpenAPI schema for the Universal Mcp Fal AI API.


| Tool | Description |
|------|-------------|
| `run` | Run a Fal AI application directly and wait for the result. Suitable for short-running applications with synchronous execution from the caller's perspective. |
| `submit` | Submits a request to the Fal AI queue for asynchronous processing and returns a request ID for tracking the job. |
| `status` | Checks the status of a previously submitted Fal AI request and retrieves its current execution state |
| `result` | Retrieves the result of a completed Fal AI request, waiting for completion if the request is still running. |
| `cancel` | Asynchronously cancels a running or queued Fal AI request. |
| `upload_file` | Uploads a local file to the Fal CDN and returns its public URL |
| `generate_image` | Asynchronously generates images using the 'fal-ai/flux/dev' application with customizable parameters and default settings |


## 📁 Project Structure

The generated project has a standard layout:
```
.
├── src/                  # Source code directory
│   └── universal_mcp_falai/
│       ├── __init__.py
│       └── mcp.py        # Server is launched here
│       └── app.py        # Application tools are defined here
├── tests/                # Directory for project tests
├── .env                  # Environment variables (for local development)
├── pyproject.toml        # Project dependencies managed by uv
├── README.md             # This file
```

## 📝 License

This project is licensed under the MIT License.

---

_This project was generated using **MCP CLI** — Happy coding! 🚀_

## Usage

- Login to AgentR
- Follow the quickstart guide to setup MCP Server for your client
- Visit Apps Store and enable the Universal Mcp Fal AI app
- Restart the MCP Server

### Local Development

- Follow the README to test with the local MCP Server 