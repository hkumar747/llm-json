# Extracting JSON data from text with LLMs

### Atlas-USACE project

![Python](https://img.shields.io/badge/python-3.8+-blue.svg) ![Jupyter](https://img.shields.io/badge/Jupyter-Notebooks-orange.svg) 
This repository hosts a series of Jupyter notebooks that demonstrate the extraction and analysis of environmental impact data from textual descriptions of USACE (U.S. Army Corps of Engineers) wetland projects. Leveraging both traditional NLP techniques and advanced machine learning models from OpenAI, these notebooks provide a comprehensive guide to understanding and predicting the environmental impacts of proposed projects.

The core task we want to accomplish here is to convert a text passage into a structured dictionary of key-value pairs:

**Input:**
>>'This project would place approximately 855 cubic yards of commercially obtained fill material within 23,087 square feet (0. 53 acres) of herbaceous wetlands for >>phase II of a single-family housing subdivision.

**Output:**
```
{
  "wetlands": [
    {
      "wetland_type": herbaceous "wetlands",
      "impact_quantity": "0.53",
      "impact_unit": "acres",
      "impact_duration": "unknown",
      "impact_type": "fill",
      "project_type:" "residential",
    }
  ]
}

```


## Overview of Notebooks

### [Notebook 1: Extract JSON from text using OpenAI](#)
In this notebook, we focus on extracting key information from PDF documents related to wetland projects. Techniques include abstractive summarization, regular expressions for data extraction, and querying OpenAI's API for structured data extraction.

### [Notebook 2: Fine-Tuning OpenAI GPT-3.5](#)
Explore the process of fine-tuning OpenAI's GPT model with domain-specific data and using the model to extract structured information from project descriptions.

### [Notebook 3: JSON mode and fine-tuning Mistral and Llama using AnyScale](#)
This notebook shows how to perform fine-tuning on the AnyScale platform for open LLMs like Llama-13b, Mistral-7b and Mistral-8x7B.

### [Notebook 4: LoRA Fine-tuning Mistral-7b on HuggingFace and WandB](#)
This notebook uses HuggingFace's `trl` library perform parameter efficient fine-tuning (PEFT) on Mistral-7b for our JSON generation task.

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
