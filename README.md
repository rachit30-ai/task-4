# Part 4 – LLM Feature

## Feature Track Chosen

**Track C – Model Prediction Explanation Pipeline**

## Objective

This notebook demonstrates an end-to-end pipeline where a trained Random Forest model predicts the target class for handcrafted inputs. The predicted class and probability are passed to an LLM, which returns a structured JSON explanation. The response is validated using a JSON schema, a PII guardrail is applied before each API call, and outputs from different temperature settings are compared.

## Files

- Part4_LLM_feature.ipynb
- best_random_forest_model.pkl
- features.txt

## LLM Used

- OpenRouter
- Model: openai/gpt-4o-mini

## Validation

- JSON Schema Validation
- PII Guardrail
- Temperature Comparison (0 vs 0.7)
- ## API Key

For security reasons, no API keys are stored in this repository.

Before running the notebook, set the environment variable:

OPENROUTER_API_KEY=<your_api_key>

The notebook reads the key using:

API_KEY = os.getenv("OPENROUTER_API_KEY")
