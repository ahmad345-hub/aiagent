# AI Agent in Python

A simple AI coding agent built with Python as part of the Boot.dev **Build an AI Agent in Python** course.

The agent can inspect files, read and write code, run Python files, and use the results to continue working toward a solution.

## Features

* Read files and directories
* Write and modify files
* Run Python files
* Function calling with an LLM
* Agent loop with multiple iterations
* Verbose mode for viewing token usage and function calls
* Working directory restriction for safer file operations

## Technologies

* Python
* OpenAI Python SDK
* OpenRouter
* python-dotenv
* uv

## Available Functions

The agent currently supports:

* `get_files_info`
* `get_file_content`
* `write_file`
* `run_python_file`

## Setup

Clone the repository:


git clone https://github.com/ahmad345-hub/aiagent.git
cd aiagent


Create and activate the virtual environment:


uv venv
source .venv/bin/activate


Install the dependencies:


uv sync


Create a `.env` file and add your OpenRouter API key:


OPENROUTER_API_KEY=your_api_key_here


## Usage

Run the agent with a prompt:


uv run main.py "Fix the bug in the calculator"


To enable verbose output:

uv run main.py "Fix the bug in the calculator" --verbose


## Example

The agent can inspect the calculator project, identify a problem, modify the code, run the tests, and verify the result.

## Course

This project was built as part of the **Build an AI Agent in Python** course on Boot.dev.
