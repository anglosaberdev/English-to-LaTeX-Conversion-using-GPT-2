# English to LaTeX Conversion using GPT-2

## Project Overview

This project demonstrates how to fine-tune a **GPT-2 transformer model** to convert English descriptions of mathematical expressions into **LaTeX code**.

The model is trained using **prompt-based fine-tuning**, where each training example follows a structured format:

```
LCT
English: <English description>
LaTeX: <LaTeX expression>
```

By learning this structure, the GPT-2 model predicts the next tokens and generates the correct LaTeX expression from the English input.

The project includes:

* Data preprocessing and prompt construction
* Tokenization using GPT-2 tokenizer
* Fine-tuning GPT-2 using HuggingFace Transformers
* Training with `Trainer` API
* Saving and loading the trained model
* Generating LaTeX expressions from English prompts

---

## Technologies Used

* Python
* PyTorch
* HuggingFace Transformers
* GPT-2
* Pandas
* Prompt Engineering

---

## Example

Input prompt:

```
LCT
English: integral from a to b of x squared
LaTeX:
```

Model output:

```
\int_{a}^{b} x^2 dx
```

---

## Acknowledgment

Special thanks to the Coursera course:

**Introduction to Transformer Models for NLP using BERT, GPT, and More**

The implementation and ideas in this project were inspired by the lecture:

**“GPT for Code Dictation”**

from this course:

https://www.coursera.org/learn/pearson-introduction-to-transformer-models-for-nlp-using-bert-gpt-and-more-mv7zg/lecture/AyzuZ/gpt-for-code-dictation

The course provides hands-on examples of working with transformer models such as GPT and BERT, including fine-tuning techniques and prompt-based learning for NLP tasks. ([Coursera][1])

---

## License

This project is for educational and research purposes.

[1]: https://www.coursera.org/learn/pearson-introduction-to-transformer-models-for-nlp-using-bert-gpt-and-more-mv7zg?utm_source=chatgpt.com "Introduction to Transformer Models for NLP: Unit 2 | Coursera"
