# MCP Server Example - Add Numbers

This repository contains a Model Context Protocol (MCP) server that provides a simple addition tool.

## Features

- **Add Tool**: Add two numbers together using the `add()` function
- **FastMCP Framework**: Built using the FastMCP framework for easy MCP server development

## Installation

To install and use the Add_numbers MCP server in Claude Desktop, add the following configuration to your `claude_desktop_config.json` file:

```json
{
  "mcpServers": {
    "Add_numbers": {
      "command": "uvx",
      "args": [
        "--from",
        "git+https://github.com/siddheshmahadik24/mcpserverexample.git",
        "mcp-server"
      ]
    }
  }
}
```

## Usage

After adding the configuration to Claude Desktop and restarting the application, you can use the addition tool by asking Claude to add numbers together. The server will automatically be invoked to perform the calculation.

## Development

To run the server locally for development:

```bash
# Clone the repository
git clone https://github.com/siddheshmahadik24/mcpserverexample.git
cd mcpserverexample

# Install dependencies
uv sync

# Run the server
uv run python src/mcpserver/deployment.py
```