---
description:  Dutch to English translation using PyTorch and a Seq2Seq RNN model with attention
title: Dutch to English translation
toc: true
badges: true
comments: true
author: Rajesh Kanna V
categories: [machine learning, natural language processing, deep learning]
image: images/posts/RajeshProfilePic2.jpg
cover: images/covers/RajeshProfilePic2.jpg
layout: notebook
permalink: /blog/:year:month:day/dutch-english-translation
sticky_rank: 2
group: Machine Learning
github_repo: AI-ML-NLP-MachineTranslation
project_id: PROJECT_5
highlights: 
  <ul>
  <li> This machine translation project translates Dutch sentences into English using PyTorch and a Sequence-to-Sequence (Seq2Seq) Recurrent Neural Network (RNN) model with attention. </li>
  </ul>
---
# Dutch to English Machine Translation using PyTorch Seq2Seq RNN

This repository contains a machine translation project that translates Dutch sentences into English using PyTorch and a Sequence-to-Sequence (Seq2Seq) Recurrent Neural Network (RNN) model with attention.

## Dataset

The dataset used in this project is loaded from [http://www.manythings.org/anki/](http://www.manythings.org/anki/).

## Project Structure

- `Data/`: Data files, including the Dutch-English sentence pairs.
- `savedModel/`: Saved model weights (if applicable).
- `README.md`: This README file.
- `Translation-Dutch-to-English-PyTorch-Seq2Seq-RNN.ipynb`: The main Jupyter notebook containing the code.

## Usage

To use this project, follow these steps:

1. Clone the repository:

   ```bash
   git clone https://github.com/vrajeshtrichy/AI-ML-NLP-MachineTranslation.git
   cd AI-ML-NLP-MachineTranslation
   ```

2. Open the `Translation-Dutch-to-English-PyTorch-Seq2Seq-RNN.ipynb` notebook in your Jupyter environment to explore the code and execute it.

3. Experiment with different inputs and sentences for translation.

## Dependencies

Make sure you have the following dependencies installed:

- Python (>=3.6)
- PyTorch
- Jupyter Notebook

You can install the required Python libraries using `pip`:

```bash
pip install torch jupyter
```

## License

This project is licensed under the MIT License.

## Acknowledgments

- The code in this project was developed based on the tutorials and documentation provided by PyTorch.
