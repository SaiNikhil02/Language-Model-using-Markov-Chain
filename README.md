# Sherlock Holmes Story Generator

This project is a language model that generates Sherlock Holmes stories using a Markov Chain. The model is trained on a dataset of Sherlock Holmes stories and can create new, coherent stories in the style of Arthur Conan Doyle.

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Dataset](#dataset)
- [Methodology](#methodology)
- [Examples](#examples)
- [Contributing](#contributing)
- [License](#license)

## Introduction
The Sherlock Holmes Story Generator uses a Markov Chain model to generate text based on the patterns found in the original Sherlock Holmes stories. This project showcases the power of Markov Chains in natural language processing and text generation.
## DataSet  
Dataset can be found in this link "/kaggle/input/sherlock-holmes-stories"
## Features
- Generates new Sherlock Holmes stories based on the original dataset.
- Simple and easy-to-understand implementation.
- Customizable text generation length and starting points.

## Installation
To run this project, you need to have Python installed on your system. Follow the steps below to set up the project:

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/sherlock-holmes-story-generator.git
    cd sherlock-holmes-story-generator
    ```

2. Create a virtual environment and activate it (optional but recommended):
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

## Usage
To generate a new Sherlock Holmes story, run the `generate_story.py` script:

```bash
python generate_story.py
```

You can customize the length of the generated text and the starting point by modifying the script parameters.

## Dataset
The dataset used to train the Markov Chain model consists of the complete Sherlock Holmes stories by Arthur Conan Doyle. You can find the dataset in the `data/` directory.

## Methodology
The model is based on a Markov Chain, which is a probabilistic model that predicts the next word in a sequence based on the previous word. Here's a brief overview of the process:

1. **Text Preprocessing**: The dataset is cleaned and tokenized to prepare it for the Markov Chain.
2. **Building the Markov Chain**: A dictionary is created where each key is a word, and the value is a list of words that follow it in the text.
3. **Generating Text**: Starting from a random word, the next word is chosen based on the probabilities in the Markov Chain, and this process is repeated to generate the desired length of text.

## Examples
Here are some examples of the generated text:

*Example 1:*
```
Sherlock Holmes looked at the paper and then at the woman. "I see," he said, "that you have been to India." The woman nodded, surprised. "How did you know?" she asked. Holmes smiled. "It is my business to know," he replied.
```

*Example 2:*
```
The room was dark and silent. Suddenly, a shadow moved across the floor. Holmes sprang to his feet. "Watson, quick!" he whispered. "There is someone in the house." Watson grabbed his revolver and followed Holmes into the hallway.
```

## Contributing
Contributions are welcome! If you have any ideas or improvements, feel free to open an issue or submit a pull request.

1. Fork the repository
2. Create a new branch (`git checkout -b feature/your-feature`)
3. Commit your changes (`git commit -am 'Add your feature'`)
4. Push to the branch (`git push origin feature/your-feature`)
5. Create a new Pull Request

## License
This project is licensed under the MIT License. See the `LICENSE` file for more details.

---
