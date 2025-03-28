# AI Pricing Strategy Code Generator
*** This is a mini project uses large language models (LLMs) like GPT, Claude, and Mistral(HuggingFace) to generate pricing strategy functions based on structured product data. It enables you to simulate and test different logic-based pricing strategies for e-commerce decision-making.

## Features

- Generates Python functions for cost-based, competitor-based, and conversion-optimized pricing
- Supports GPT-4, Claude 3.5, and Mistral via API
- Displays generated code and suggested prices interactively using Gradio
- Stream-based outputs for real-time feedback
- Modular setup for plug-and-play strategy testing

## Inside this code. Explaination

- `SYSTEM_PROMPT`: Defines how the model should act (as a pricing expert)
- `PRICING_FUNCTION_EXAMPLE`: A starter function to teach the model the expected structure
- `decision_gpt()`, `decision_claude()`, `decision_mistral()`: Calls different LLMs to generate pricing strategies
- `strategy()`: Controls model selection and response streaming
- `Gradio UI`: User-friendly interface to input functions and view output

## Sample## Sample
```python
product = {
    "name": "Sunscreen",
    "cost": 100,
    "stock": 80,
    "competitor_prices": [120, 130, 125],
    "historical_conversion": {110: 0.03, 115: 0.05, 120: 0.04},
    "is_promo_day": False
}

```

