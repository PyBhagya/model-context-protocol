# model-context-protocol

A custom server project built using the Model Context Protocol (MCP) in Python. This repository implements a simple AI Sticky Notes application that demonstrates the core functionality of MCP.

## What We've Built

This project implements a simple but functional MCP server that acts as an AI Sticky Notes application with the following features:

- **Adding Notes**: Users can add new notes to a persistent storage file
- **Reading Notes**: Users can retrieve all stored notes
- **Accessing Latest Note**: A resource endpoint to get only the most recent note
- **Note Summarization**: A prompt generator that asks an AI to summarize all current notes

## Core Components

1. **FastMCP Server**: The main server implementation using the MCP framework
2. **Tools**: Function endpoints that perform specific actions
   - `add_note`: Adds a new note to storage
   - `read_notes`: Retrieves all stored notes
3. **Resources**: Data endpoints that provide specific information
   - `notes://latest`: Provides the most recently added note
4. **Prompts**: Template generators for AI interactions
   - `note_summary_prompt`: Creates a prompt asking an AI to summarize all notes

## What You Can Do With This Server

### For Developers

- **Extend Functionality**: Add new tools, resources, or prompts to enhance the application
- **Integrate with AI Models**: Connect this server to LLMs to create an intelligent note-taking application
- **Use as a Reference**: Learn how to structure MCP applications for your own projects
- **Build a UI**: Create a frontend that interacts with these endpoints

### For Users

- **Manage Notes**: Add and retrieve notes through the API
- **Get AI Summaries**: Use the prompt endpoint to generate summaries of your notes
- **Access Latest Information**: Quickly retrieve the most recent note

## Getting Started

To run the server:

```bash
python main.py
```

The server will start and expose endpoints for adding notes, reading notes, accessing the latest note, and generating summary prompts.

## Future Enhancements

Potential improvements for this project:

- Add note deletion and editing capabilities
- Implement note categorization and tagging
- Create a web interface for easier interaction
- Add authentication for multi-user support
- Integrate with external AI services for automatic note analysis
