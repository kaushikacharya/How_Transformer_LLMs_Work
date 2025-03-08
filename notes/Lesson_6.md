# Architectural Overview

- Three major components:
  - Tokenizer
  - Stack of Transformer Blocks
  - Language Modeling Head

- Tokenizer holds a vocabulary, the model contains token embeddings
  ![Tokenizer: Vocabulary and Model: Token embeddings](../images/6_0.png)
- Language Model head scores the best (most probable) next token to output
  ![LM head output](../images/6_1.png)

- Multiple decoding strategies exist to choose the best output token
  ![Decoding strategies](../images/6_2.png)
  - Choose the highest
    - `temperature` = 0
    - Greedy decoding
  - Choose `top_p`
    - This considers multiple tokens based on their probability i.e. not limited to the highest probable one.
  - Add randomness
    - `temperature` > 0

- Multiple tracks in parallel
  - Number of tracks = Context length
  ![Multiple tracks in Transformer](../images/6_3.png)
  - Generated output token in transformer is the output of the final token.
  - TTFT: Time to First Token
    - Time taken by model to process the above shown calculation

- KV Caching
  ![KV Caching](../images/6_4.png)
  - Post 1st token generation, input also contains the generated tokens.
