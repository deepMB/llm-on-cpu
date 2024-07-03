# Running Large Language Models (LLM) on CPU

This repository provides guidelines and scripts to run large language models (LLMs) on CPU, utilizing techniques such as quantization and GGML to optimize performance and reduce resource usage.

## Table of Contents
- [Introduction](#introduction)
- [Quantization](#quantization)
- [GGML](#ggml)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Introduction

Running large language models (LLMs) on CPUs can be challenging due to their significant computational and memory requirements. However, with optimization techniques like quantization and GGML (General Graph Machine Learning), it is possible to achieve efficient inference on CPU, making it accessible for a wider range of applications.

## Quantization

Quantization is a technique used to reduce the computational and memory footprint of neural networks. By converting the weights and activations of the model from higher precision (e.g., 32-bit floating-point) to lower precision (e.g., 8-bit integer), we can significantly decrease the model size and increase the inference speed. There are different types of quantization methods, including:
- **Post-Training Quantization:** Quantizing a pre-trained model without requiring additional training data.
- **Quantization-Aware Training (QAT):** Training the model with quantization in mind to achieve better accuracy.

Quantization helps in reducing the resource requirements, making it feasible to run large models on CPUs with limited computational power.

## GGML (General Graph Machine Learning)

GGML is an optimization framework designed to efficiently run machine learning models, particularly on resource-constrained environments like CPUs. GGML optimizes both the computation graph and the underlying hardware instructions to enhance the performance of machine learning models. Key features of GGML include:
- **Graph Optimization:** Reduces redundant computations and optimizes the execution order.
- **Hardware-Specific Optimizations:** Leverages CPU-specific instructions and optimizations to accelerate inference.
- **Memory Management:** Efficiently manages memory allocation and deallocation to handle large models on CPUs.

By integrating GGML with quantization, we can further optimize the performance of LLMs on CPU.

## Installation

To run LLMs on CPU using this repository, you need to have Python and the required libraries installed. Follow the steps below to set up the environment:

1. Clone the repository:
    ```bash
    git clone https://github.com/deepMB/llm-on-cpu.git
    cd llm-on-cpu
    ```

2. Install the necessary dependencies:
    ```bash
    pip install -r requirements.txt
    ```

## Usage
### Create new Conda Environment

conda create -n llmapp python=3.10 -y

### Activate conda environment

conda activate llmapp
### Install the requirements

pip install -r requirements.txt
  

## Contributing

Contributions are welcome! Please open an issue or submit a pull request if you have any improvements or bug fixes.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.






