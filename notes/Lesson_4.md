# Understanding Language Models: Transformers

## Attention is All You Need

- **Transformer**
  - A new architecture solely based on attention and without the RNN
  - Could be trained in parallel which speeds up calculation significantly
  - Stacking these blocks amplify the strength of the encoder and decoders.

  ![Transformer Encoder](../images/4_0.png)

  ![Attention is All You Need](../images/4_1.png)

## Representation Models

### Bidirectional Encoder Representations from Transformers (BERT)

![BERT](../images/4_2.png)

- BERT focusses on representing language and generating contextual word embeddings
- [CLS] token (classification token)
  - Additional input token: Used as a representation for the entire input
  - Often used as the input embedding for finetuning the model on specific tasks like classification
- Masked Language Modeling
  - Training
    - Randomly some of the words in the input sequence are masked
    - Model is trained to predict these masked words
    - By doing so, the model learns to represent language as it attempts to deconstruct these masked words
    ![Masked Language Modeling](../images/4_3.png)
  - Traning is a two-step process
    ![Two-step trainng process](../images/4_4.png)

## Generative Models

### Generative Pre-Trained Transformer (GPT)

- Embeddings are randomly initialized
![GPT & BERT](../images/4_5.png)

### Context Length

![Context Length](../images/4_6.png)

### Parameters

![GPT evolution](../images/4_7.png)

## Year of Generative AI

![Evolution of Proprietary and Open-source models](../images/4_8.png)
