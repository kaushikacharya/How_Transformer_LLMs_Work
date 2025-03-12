# How Transformer LLMs Work

## About

This repository contains

- [Course notes](#course-contents)
- [Assignments](#assignments)
- Additional resources (collected for better understanding of the concepts)

## Course Information

- Instructors: Jay Alammar, Maarten Grootendorst
- [Course Website](https://www.deeplearning.ai/short-courses/how-transformer-llms-work/)

## Course Contents

|#|     Lesson  |   Description   |
|-|-------------|-----------------|
|0|[Introduction](./notes/Lesson_0.md)|<ul><li>Transformer outline</li><li>Course outline</li></ul>|
|1|[Understanding Language Models: Language as a Bag-of-Words](./notes/Lesson_1.md)|<ul><li>Evolution of numerical representation of language</li><li>Example of Bag-of-Words' vector representation</li></ul>|
|2|[Understanding Language Models: (Word) Embeddings](./notes/Lesson_2.md)|<ul><li>Drawbacks of Bag-of-Words</li><li>Word2Vec explanation</li></ul>|
|3|[Understanding Language Models: Encoding and Decoding Context with Attention](./notes/Lesson_3.md)|<ul><li>Drawbacks of Word2Vec embeddings</li><li>Recurrent Neural Networks (RNNs)</li><li>Attention Mechanism</li></ul>|
|4|[Understanding Language Models: Transformers](./notes/Lesson_4.md)|<ul><li>Transformer architecture</li><li>Representation vs Generative Models</li><li>Context Length</li><li>Evolution of Generative AI over recent years</li></ul>|
|5|[Tokenizers](./notes/Lesson_5.md)|<ul><li>Contextualized embeddings</li><li>Tokenization</li></ul>|
|6|[Architectural Overview](./notes/Lesson_6.md)|<ul><li>Three major components of transformer LLM</li><li>Parallel processing of tokens</li><li>KV Caching</li></ul>|
|7|[The Transformer Block](./notes/Lesson_7.md)|<ul><li>Feedforward Neural Network intuition</li><li>Self-Attention intuition</li></ul>|
|8|[Self-Attention](./notes/Lesson_8.md)|<ul><li>Advanced techniques of Self-Attention for efficient computation</li></ul>|
|9|[Model Example](./notes/Lesson_9.md)|<ul><li>Text generation using model from Hugging Face</li></ul>|
|10|[Recent Improvements](./notes/Lesson_10.md)|<ul><li>Efficient organization of training data</li><li>Rotatory Embeddings (RoPE)</li><li>Mixture of Experts (MoE)</li></ul>|
|11|[Mixture of Experts (MoE)](./notes/Lesson_11.md)|<ul><li>MoE components: Experts & Router</li><li>Computational Requirements</li><li>Pros & Cons of MoE</li></ul>|

## Assignments

|Lesson|         Assignment        |   Description   |
|-------|---------------------------|-----------------|
|#5|[Comparing Trained LLM Tokenizers](./notes/Lesson_5.md#notebook)|<ul><li>Explore tokenization by different tokenizers</li><li>Visualize tokens in different colors using ANSI escape codes</li></ul>|
|#9|[Model Example](./notes/Lesson_9.md#notebook)|<ul><li>Text generation using `microsoft/Phi-3-mini-4k-instruct`</li></ul>|
