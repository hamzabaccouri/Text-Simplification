# Text Simplification

This repository contains a project for simplifying French text according to the Facile à Lire et à Comprendre (FALC) guidelines. The project uses advanced language models to rewrite sentences in a simpler form while preserving the original meaning.

## Notebooks Included

### 1. Text_Simplification_with_LLAMA.ipynb
This notebook demonstrates the use of the **LLAMA model** for simplifying French text. It includes:
- A preprocessing step to format input text.
- The implementation of Gradio for an interactive user interface.
- Example prompts and outputs for text simplification.

### 2. Text_Simplification_with_FALCON.ipynb
This notebook uses the **FALCON model** for the same task. Key differences include:
- Adaptation to FALCON's tokenizer and model specifications.
- Similar interactive interface with Gradio.
- Slight differences in performance based on the model's architecture.

## Features
- Supports interactive text simplification through Gradio.
- Implements state-of-the-art language models for text simplification.
- Customizable input sentences with a focus on FALC guidelines.

## Setup and Installation

### Prerequisites
- **Python 3.8+**
- Libraries: `transformers`, `bitsandbytes`, `gradio`, `torch`, `sentencepiece`, `accelerate`
- A Hugging Face token with access to the LLAMA and FALCON model repositories.

### Steps
1. Clone this repository:
   ```bash
   git clone https://github.com/hamzabaccouri/Text-Simplification.git
   cd Text-Simplification
   ```

2. Install the dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Set up your Hugging Face token:
   ```bash
   huggingface-cli login
   ```

4. Open the desired notebook (e.g., LLAMA or FALCON) in Jupyter Notebook or Google Colab.

5. Run all cells to start the Gradio interface. Once launched, input a French sentence to see the simplified output.

## Notes
- Ensure you have access to the pretrained LLAMA and FALCON models on Hugging Face.
- The Gradio interface shuts down automatically after 20 seconds of inactivity.

## Example Input and Output

### Input:
```
L'apprentissage des mathématiques demande de la rigueur et de la patience.
```

### Output:
```
Apprendre les mathématiques nécessite de la discipline et de la persévérance.
```

## Folder Structure
```
Text-Simplification/
├── Text_Simplification_with_LLAMA.ipynb  # Notebook using LLAMA
├── Text_Simplification_with_FALCON.ipynb # Notebook using FALCON
├── requirements.txt                      # List of dependencies
├── README.md                             # Project documentation
```

## Acknowledgements
- **Hugging Face** for providing the LLAMA and FALCON models.
- **Gradio** for the interactive interface.
