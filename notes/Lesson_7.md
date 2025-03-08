# The Transformer Block

## Transformer LLM

![Transformer LLM](../images/7_0.png)

## Transformer Block: Feedforward Neural Network Intuition

- Intuition:
  - Storage of information and statistics
  - Based on that it would be able to predict the next probable word.
    - In the case of "The Shawshank" the next probable word would be "Redemption" because of the famous movie.

![Feedforward Neural Network in Transformer](../images/7_1.png)

## Transformer Block: Self Attention

- Attention allows us to incorporate relevant information from the context
- Coreference Resolution
  ![Coreference Resolution](../images/7_2.png)
- Self-Attention achieves
  - Relevance Scoring
    - Computes context relevance of other tokens
  - Combining Information
    - Combine the relevance into the vector representation of current token

  ![Self Attention Objectives](../images/7_3.png)
