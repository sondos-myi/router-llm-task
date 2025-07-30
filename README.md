# Router LLM Task

## Overview

This project implements a router LLM that decides between a vision LLM and a text LLM based on input type, using Multi-Component Prompting. The solution uses OpenAI's GPT-3.5-turbo for text, GPT-4o for vision, and routes requests accordingly.

## Files

- `mcpTask.ipynb`: Main Jupyter notebook with all code and tests.
- `cat.jpg`: Sample image for testing vision LLM.
- `requirements.txt`: Python dependencies (install with `pip install -r requirements.txt`).

## How to Run

1. Install dependencies:
   ```
   pip install -r requirements.txt
   ```
2. Set your OpenAI API key in a `.env` file:
   ```
   OPENAI_API_KEY=your_api_key_here
   ```
3. Open `mcpTask.ipynb` in Jupyter and run the cells.

## Notes

- The router uses GPT-3.5-turbo to decide which LLM to use.
- Vision LLM uses GPT-4o.
- Make sure you have sufficient OpenAI API quota.

## Example

- Text input: "What is the capital of Jordan?"
- Image input: `cat.jpg` with prompt "Describe this image."
