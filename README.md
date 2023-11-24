# WeightQuantization_LLM

# Reducing-the-size-of-Large-Language-Models-with-8-bit-quantization
 
 
## Weight Quantization for Reducing Language Model Size
 
## Introduction
This repository demonstrates techniques to reduce the size of Large Language Models (LLMs) using 8-bit quantization. The code implements two quantization methods - **Absmax Quantization** and **Zeropoint Quantization** - applied to the weights of a GPT-2 language model.
 
## Techniques Demonstrated
- **Absmax Quantization**: Quantizes weights based on their absolute maximum value.
- **Zeropoint Quantization**: Quantizes weights around the zero-point to reduce the range.
 
## Libraries and Requirements
The code uses the following libraries:
- PyTorch
- Hugging Face Transformers
- Accelerate
 
Ensure that these are installed to run the code successfully.
 
## Code Overview
The code contains functionalities for:
- Implementing Absmax and Zeropoint Quantization functions for weight reduction.
- Loading and quantizing weights of the GPT-2 model.
- Visualizing the impact of quantization on weight distributions using histograms.
- Generating text with the original and quantized models.
- Calculating perplexity to evaluate model performance before and after quantization.
 
## Usage
1. **Installation**: Install the required packages using the specified `!pip` commands.
2. **Running the Code**: Execute the code blocks sequentially to observe each step of quantization and its impact.
3. **Visualizations**: Check the visualizations generated to understand the effects of weight quantization.
4. **Model Performance**: Evaluate model performance using perplexity scores provided before and after quantization.
 
## Model Size Reduction
The code demonstrates how 8-bit quantization significantly reduces model size compared to the original GPT-2 model. The `LLM.int8()` method creates an 8-bit quantized model, effectively reducing memory footprint while maintaining functionality.
