# Text Generator with Hugging Face Transformers

This project demonstrates the use of Generative AI to build a text generator using Hugging Face's `transformers` library. The model used is OpenAI's GPT-2, a popular pre-trained language model.

## Features
- Accepts text prompts from the user
- Generates coherent text completions
- Based on the GPT-2 model

## Installation

1. Clone the repository:
```
git clone https://github.com/yourusername/genai-text-generator.git
cd genai-text-generator
```

2. Set up the virtual environment:
```
sudo apt install python3-venv -y
python3 -m venv genai_project
source genai_project/bin/activate
```

3. Install Dependencies:
- Install Required Libraries:
```
pip install transformers torch
```

- Create `requirements.txt`:
```
transformers==4.x.x
torch==2.x.x
```
- Replace `4.x.x` and `2.x.x` with the installed versions from the `pip freeze` command.

4. Run the script:
```
python main.py
```
- Enter a prompt, e.g., "Once upon a time".
- The program will generate text based on your input.

## Example Usage

### Example 1
- Input:
```
Once upon a time, there was a magical kingdom
```
- Output:

### Example 2
- Input:
```
Once upon a time in a distant galaxy,
```
- Output:


### Saved user inputs and outputs to a log file:
- Output of `generated-texts.txt`:

## File Structure
- Organize your project directory like this:
```
genai-text-generator/
│
├── README.md
├── requirements.txt
├── main.py
└── generated_texts.txt
```

## License

This project is licensed under the MIT License.
