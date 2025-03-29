# Self-Attention

- Projection Matrices
![Self-Attention Projection Matrices](../images/8_0.png)

- End goal of Relevance Scoring
  ![Relevance Scoring: End Goal](../images/8_1.png)

- Recommended Course on Attention
  - [Attention in Transformers: Concepts and Code in PyTorch](https://github.com/kaushikacharya/Attention_in_Transformers_Concepts_and_Code)

- Combining Information from other tokens
  ![Combining Information](../images/8_2.png)

## Multi-Head Attention

![Multi-Head Attention](../images/8_3.png)

- Each Attention Head has its own Key, Query, Value matrices

## Multi-Query Attention

- One of the approaches for efficient computation of self-attention
- Self-attention component contributes a major chunk of computation
![Multi-Query Attention](../images/8_4.png)
- Shared Key and Values matrix for each transformer block
- Can be visualized as compression of parameters

## Grouped-Query Attention

![Grouped-Query Attention](../images/8_5.png)

- Instead of single Keys and Values matrix, it has same as number of groups.
- Works better than Multi-Query Attention for large models.

## Sparse Attention

![Sparse Attention](../images/8_6.png)

- Local attention boosts performance of large models by only paying attention to a small number of previous positions.
- This need not be applied to all the layers.
  - First layer can attend to all previous positions.
  - But interleaved layers can attend to a small number of previous positions.

- Full attention vs Sparse attention
  ![Full attention vs Sparse attention](../images/8_7.png)
- Source: [Generating Long Sequences with Sparse Transformers by Child et al (2019)](https://arxiv.org/abs/1904.10509)

## Ring Attention

- Uses multiple devices to scale to a near infinite context window
- Referred blog: [Coconut Mode](https://coconut-mode.com/posts/ring-attention/)

## Paper: The Llama 3 Herd of Models

- 8B parameter model's hyperparameters visualization
  ![Llama 3 8B parameter model](../images/8_8.png)
- ?? How is FFN dimension matching in visualization?
