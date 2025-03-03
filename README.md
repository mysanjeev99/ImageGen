# ImageGen - Stable Diffusion 3.5 Quantized Model for Local Setup

This repository contains the necessary code to download and quantize the Stable Diffusion 3.5 model for running locally. It allows you to generate images using the quantized Stable Diffusion models, optimized for better performance on your local machine.

## Requirements

To download the model, you must have access to Hugging Face. Follow these steps to get started:

### 1. **Access to the Model on Hugging Face**

You need to get access for Stable Diffusion 3.5 model from Hugging Face. 

- **For Stable Diffusion 3.5 Large**:    [Download Link](https://huggingface.co/stabilityai/stable-diffusion-3.5-large)
  
- **For Stable Diffusion 3.5 Medium**:    [Download Link](https://huggingface.co/stabilityai/stable-diffusion-3.5-medium)

### 2. **Create a Hugging Face Token**

You must have a Hugging Face API token to download the model.

- Go to [Hugging Face Token Settings](https://huggingface.co/settings/tokens).
- Create a new token.

### 3. **Hugging Face CLI Authentication**

After creating your token, you'll need to log in to the Hugging Face CLI to authenticate and download the model.

- Install the Hugging Face CLI tool:
  ```bash
  pip install huggingface_hub
## Setup Instructions

### 1. Clone the Repository

First, clone the repository to your local machine:

```bash
git clone https://github.com/mysanjeev99/ImageGen.git
cd ImageGen
```

### 2. Download the Model

Once you've logged into Hugging Face CLI, you can download the required model using the following commands:

- For **Stable Diffusion 3.5 Large**:

```bash
huggingface-cli download stabilityai/stable-diffusion-3.5-large --cache-dir ./sd
```
- For **Stable Diffusion 3.5 Medium**:

```bash
huggingface-cli download stabilityai/stable-diffusion-3.5-medium --cache-dir ./sd
```

### 3. Run the Image Generation Script

Once the model is downloaded, you can use the given notebook to quantize the model and test it out.

- For **Stable Diffusion 3.5 Large**, use: `SD_3.5_Large.ipynb`
- For **Stable Diffusion 3.5 Medium**, use: `SD_3.5_Medium.ipynb`
