# French Text Simplifier with LLaMA

## Description
This project is a French text simplifier powered by the LLaMA model. It simplifies French text according to the "Facile à Lire et à Comprendre" (FALC) guidelines. The system takes a standard French sentence as input and rewrites it in a simpler, easier-to-understand form, preserving the original meaning.

### Key Features:
- Utilizes LLaMA with **4-bit quantization** for efficient performance.
- Supports GPU and CPU execution with memory optimization.
- Allows dynamic input for user-provided sentences.
- Integrated with a Gradio-based user interface for ease of interaction.

## FALC Guidelines Used for Simplification
- Use simple, common vocabulary.
- Write short, clear sentences.
- Avoid complex grammar and jargon.
- Retain the original meaning and key information.
- Ensure grammatical correctness.

## Setup and Installation

### Prerequisites
- Python 3.8+
- Libraries: `transformers`, `bitsandbytes`, `gradio`
- A Hugging Face token with access to the LLaMA model repository.

### Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/llama-text-simplifier.git
   cd llama-text-simplifier
   ```
2. Install the dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Set up your Hugging Face token:
   ```bash
   huggingface-cli login
   ```

4. Open the Jupyter notebook:
   ```bash
   jupyter notebook llama_text_simplifier.ipynb
   ```

## Usage

1. Run the notebook cells in order.
2. Enter a French sentence in the input box when prompted.
3. The simplified version will be displayed in the output.

## Example Input and Output

**Input:**
> L'apprentissage des mathématiques demande de la rigueur et de la patience.

**Output:**
> Apprendre les mathématiques nécessite de la discipline et de la persévérance.

## Folder Structure
```
llama-text-simplifier/
├── llama_text_simplifier.ipynb # Notebook containing the code
├── requirements.txt            # List of dependencies
├── README.md                   # Project documentation
```

## Contributing
Feel free to contribute to this project by submitting a pull request. Ensure your contributions align with the project goals.

## License
This project is licensed under the MIT License. See the `LICENSE` file for details.

## Acknowledgements
- [Hugging Face](https://huggingface.co/) for providing the LLaMA model.
- [Gradio](https://gradio.app/) for the interactive interface.

