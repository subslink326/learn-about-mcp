This project implements a Model Context Protocol (MCP) client using Replit. It allows you to interact with AI language models through a simple command-line interface.

All you have to do is:
- Remix this template
- Paste in your API key
- Start prompting!

Try it out:

```
llm "Summarize this video https://youtu.be/1qxOcsj1TAg and write the summary to summary.txt"
```

## Overview

The Model Context Protocol (MCP) provides a standardized way to interact with various AI models. This implementation uses the `mcp-client-cli` package to enable simple command-line interactions with AI models like OpenAI's GPT.

## Setup Instructions

1. **Remix** this Replit project
2. **Set up your OpenAI API key**:
   - Click on the "Tools" menu in the Replit sidebar
   - Select "Secrets"
   - Add a new secret with:
     - Key: `LLM_API_KEY`
     - Value: Your OpenAI API key
3. **Run the project** by clicking the Run button

## How to Use

Once the project is running, simply type:

```
llm "Your prompt here"
```

For example:
```
llm "What is the Model Context Protocol?"
```

The system will process your prompt using the configured language model and display the response.

## Project Configuration

The project uses the configuration in `mcp-server-config.json` to define:
- The system prompt for the AI assistant
- Which LLM provider and model to use (OpenAI's gpt-4o-mini by default)
- Various MCP servers for additional functionality

## Files in the Project

- `mcp-server-config.json`: Configuration for the MCP client
- `pyproject.toml`: Python project dependencies
- `package.json`: Node.js dependencies
- `.replit`: Replit configuration file

## Dependencies

This project uses:
- `mcp-client-cli`: The MCP command-line interface (learn more [here](https://pypi.org/project/mcp-client-cli/))
- `yt-dlp`: YouTube download capability (available through MCP servers)

## Advanced Features

The MCP client supports various server extensions including:
- YouTube content processing
- Filesystem access
- Fetch capabilities for external content

## Troubleshooting

If you encounter any issues:

1. Make sure your OpenAI API key is correctly set in Secrets
2. Verify that the model specified in the configuration is available with your API key
3. Check that all dependencies are properly installed

## License

See the project license for details on usage and distribution.
