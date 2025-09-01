To install the "Add_numers" MCP server, run the following command 

'''json


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