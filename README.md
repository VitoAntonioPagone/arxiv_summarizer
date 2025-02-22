# ArXiv Paper Summarizer

This repository provides a Python script to fetch and summarize research papers from arXiv using the free Gemini API. The tool is designed to help researchers, students, and enthusiasts quickly extract key insights from arXiv papers without manually reading through lengthy documents.

## Features
- **Single Paper Summarization**: Summarize a single arXiv paper by providing its URL.
- **Batch Summarization**: Summarize multiple arXiv papers by listing their URLs in a text file.
- **Easy Setup**: Simple installation and configuration process using Conda and pip.
- **Gemini API Integration**: Leverages the free Gemini API for high-quality summarization.

## Prerequisites
- Python 3.11
- Conda (for environment management)
- A Gemini API key (free to obtain)

## Installation

### 1. Clone the Repository
```bash
git clone https://github.com/Shaier/arxiv_summarizer.git
cd arxiv_summarizer
```

### 2. Set Up the Conda Environment
Create and activate a Conda environment with Python 3.11:
```bash
conda create -n arxiv_summarizer python=3.11
conda activate arxiv_summarizer
```

### 3. Install Dependencies
Install the required Python packages using pip:
```bash
pip install -r requirements.txt
```

### 4. Configure the Gemini API Key
Obtain your Gemini API key from [Google's Gemini API page](https://ai.google.dev/gemini-api/docs/api-key). Once you have the key, open the `arxiv_summarize.py` file and replace `YOUR_GEMINI_API_KEY` on line 5 with your actual API key.

## Usage

### Summarize a Single Paper
To summarize a single arXiv paper, run the script and provide the arXiv URL (ensure it is the abstract page, not the PDF link):
```bash
python arxiv_summarize.py
```
When prompted:
1. Enter `1` to summarize a single paper.
2. Provide the arXiv URL (e.g., `https://arxiv.org/abs/2410.08003`).

### Summarize Multiple Papers
To summarize multiple papers:
1. Add the arXiv URLs to the `links.txt` file, with one URL per line.
2. Run the script:
```bash
python arxiv_summarize.py
```
3. When prompted, enter `2` to process all URLs listed in `links.txt`. The result summaries will be written in `result.txt`.

## Example
Here’s an example of how to use the script:
```bash
python arxiv_summarize.py
> Enter 1 for single paper or 2 for multiple papers: 1
> Enter the arXiv URL: https://arxiv.org/abs/2410.08003
```

## Contributing
Contributions are welcome! If you have suggestions, improvements, or bug fixes, please open an issue or submit a pull request.

## Support
If you encounter any issues or have questions, feel free to open an issue.