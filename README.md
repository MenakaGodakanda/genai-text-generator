# Text Generator with GenAI

This project demonstrates the use of Generative AI to build a text generator using Hugging Face's `transformers` library. The model used is OpenAI's GPT-2, a popular pre-trained language model.

## Overview
<img width="1086" alt="Screenshot 2025-01-30 at 6 54 21 pm" src="https://github.com/user-attachments/assets/0469a7f2-b967-453f-ae2f-4b80a34be2f1" />

### Explanation:
#### 1. User Input
- The user enters a text prompt via the terminal.

#### 2. Model & Tokenizer Initialization
- The script loads the GPT-2 model and tokenizer.
- Sets `pad_token = eos_token` to prevent padding issues.

#### 3. Preprocessing
- Tokenizes the input.
- Applies padding and truncation.

#### 4. Text Generation
- Generates text using `max_length`, `temperature`, `top_k`, and `do_sample=True`.

#### 5. Output Handling
- Displays generated text in the terminal.
- Saves the input and output to `generated_texts.txt`.

## Features
- Accepts text prompts from the user
- Generates coherent text completions
- Based on the GPT-2 model

## Installation

### 1. Clone the repository:
```
git clone https://github.com/MenakaGodakanda/genai-text-generator.git
cd genai-text-generator
```

### 2. Set up the virtual environment:
```
sudo apt install python3-venv -y
python3 -m venv genai_project
source genai_project/bin/activate
```
![Screenshot 2025-01-12 163700](https://github.com/user-attachments/assets/b8e62d8d-2ef7-4b5d-b7cb-fe0fd28906c7)

### 3. Install Dependencies:
- Install Required Libraries:
```
pip install transformers torch
```

### 4. Run the script:
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
![Screenshot 2025-01-12 163513](https://github.com/user-attachments/assets/16c79a34-6dac-4afb-b4dd-1a2bee90f16e)

### Example 2
- Input:
```
Once upon a time in a distant galaxy,
```
- Output:
![Screenshot 2025-01-12 163623](https://github.com/user-attachments/assets/d3c69c9b-ff25-4c21-a86d-ecd5eb39b9ee)


### Saved user inputs and outputs to a log file:
- Output of `generated-texts.txt`:
![Screenshot 2025-01-12 163634](https://github.com/user-attachments/assets/6cf90153-b177-4951-8c60-37370ec2e61f)

## File Structure
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
