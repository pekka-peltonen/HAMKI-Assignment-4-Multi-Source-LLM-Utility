# Assignment #4 – Multi-Source LLM Utility

Author: Pekka Peltonen
Course: HAMK – AI APIs and Standalone AI Applications

## Description
A Python command-line application that reads different source types and uses an OpenAI language model to analyze their contents.

## Supported sources
- TXT and Markdown files
- CSV files
- Word documents (DOCX)
- PDF documents
- HTML files and web URLs
- Multiple sources in one request

## Features
- Custom questions using -q
- Save results to a file using -o
- Verbose processing information using -v
- Source size limit and error handling
- Instructions to treat source content as untrusted data

## AI model
OpenAI gpt-5.6-sol

## Installation
Install Python and the required packages:

python -m pip install openai python-docx pymupdf

Set the OPENAI_API_KEY environment variable before running the program.

## Example
python llm_sources.py test.txt -q "Summarize this document." -v

## Multiple sources
python llm_sources.py test.txt testi.pdf -q "Compare these sources."

## Save output
python llm_sources.py test.txt -o summary.md

## Tested
TXT, CSV, DOCX, PDF, web URL, multiple-source comparison and saving output.
