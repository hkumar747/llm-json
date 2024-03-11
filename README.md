# Extracting JSON data from text with LLMs

### Atlas-USACE project

![Python](https://img.shields.io/badge/python-3.8+-blue.svg) ![Jupyter](https://img.shields.io/badge/Jupyter-Notebooks-orange.svg) ![OpenAI](https://img.shields.io/badge/OpenAI-API-green.svg)

This repository hosts a series of Jupyter notebooks that demonstrate the extraction and analysis of environmental impact data from textual descriptions of USACE (U.S. Army Corps of Engineers) wetland projects. Leveraging both traditional NLP techniques and advanced machine learning models from OpenAI, these notebooks provide a comprehensive guide to understanding and predicting the environmental impacts of proposed projects.

The core task we want to accomplish here is to convert a text passage into a structured dictionary of key-value pairs:

## Overview of Notebooks

### [Notebook 1: Extract Fields from PDF Text](#)
In this notebook, we focus on extracting key information from PDF documents related to wetland projects. Techniques include abstractive summarization, regular expressions for data extraction, and querying OpenAI's API for structured data extraction.

### [Notebook 2: Fine-Tuning and Inference with OpenAI](#)
Explore the process of fine-tuning OpenAI's GPT model with domain-specific data and using the model to extract structured information from project descriptions.

### [Notebook 3: Advanced Techniques for Environmental Data Extraction](#)
This notebook delves into more advanced data extraction techniques, including fine-tuning large language models on environmental datasets and leveraging the latest in AI research to improve data extraction efficiency and accuracy.

## Getting Started

To use these notebooks, you'll need to install the required Python packages and set up your environment.

- Python 3.8 or higher
- Jupyter Notebook or JupyterLab
- An OpenAI API key

Clone the repository and install the required dependencies:

```bash
git clone https://github.com/hkumar747/llm-json.git
cd llm-json
pip install -r requirements.txt
```

Make sure to configure your environment with your OpenAI API key:

```bash
export OPENAI_API_KEY='your_api_key_here'
```

## Contributing
Contributions are welcome! If you have improvements or bug fixes, please open a pull request.

## License
Distributed under the MIT License. See LICENSE for more information.

## Acknowledgments:
For the full `wetland-tracker' repository and application, check out [this repo](https://github.com/AtlasPublicPolicy/wetlands-tracker/tree/main) by Atlas Public Policy.