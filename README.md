# LLM Model Comparison: AI Safety Lab Evaluation

## Overview
This project runs a lightweight comparison of four large language models evaluating fictional AI labs in terms of:
- AI safety risk
- Investment suitability (ROI perspective)

The goal is to assess differences in reasoning quality, structure adherence, and analytical depth across models rather than to optimise a production system.

## Models Evaluated
- GPT-4.1
- GPT-4.1 Mini
- Llama 3.1 8B
- Qwen 2.5 7B

## Method
Each model is given the same prompt describing an AI lab and asked to produce a structured analysis including:
- causal chain
- assumptions and failure points
- ROI implications
- summary

Responses are scored using a lightweight rubric across:
- causal clarity
- assumption quality
- ROI linkage
- specificity
- markdown adherence

## Outputs
The notebook generates:
- comparative scores across models and labs
- summary statistics
- visualisations of total scores per model/lab
- optional exported Plotly charts

## Results

![Model comparison](./"Total scores per Lab by Model.png")

## Requirements
Install dependencies via:

```bash
pip install -r requirements.txt
```
Or using uv if preferred.

## Running

Open the notebook and run all cells. Ensure environment variables are set for API access:

OPENAI_API_KEY

Ollama models are expected to be running locally if used.

## Notes

This is an exploratory evaluation exercise, not a benchmark. Results should be interpreted qualitatively rather than statistically.