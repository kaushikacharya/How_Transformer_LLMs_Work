# Model Example

- Objective: Explore model from HuggingFace library

## Notebook

- [Jupyter Notebook](../code/L9.ipynb)
- Text generation using decoder-only model `microsoft/Phi-3-mini-4k-instruct`
- `model_output[0].shape` -> torch.Size([1, 5, 3072])
  - 1: Batch size
  - 5: No. of tokens
  - 3072: Vector embedding dimension
- Issues faced during local run
  - `RuntimeError: Expected all tensors to be on the same device, but found at least two devices, cuda:0 and cpu!`
    - As suggested in [StackOverflow thread](https://stackoverflow.com/questions/66091226/runtimeerror-expected-all-tensors-to-be-on-the-same-device-but-found-at-least), move input also to CUDA
      - Added `to(device)` in `input_ids.to(device)`
