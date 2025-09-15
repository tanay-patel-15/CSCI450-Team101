# CSCI450-Team101

This project uses a pre-trained BERT model from [Hugging Face](https://huggingface.co/) for NLP tasks as an example.

## Model Used
- [`google/bert_uncased_L-2_H-128_A-2`](https://huggingface.co/google/bert_uncased_L-2_H-128_A-2)

## License Compatibility

**Model License:** Apache 2.0  
- This license allows academic and commercial use.
- Requirements: you must provide attribution (credit the model’s source), indicate any changes you make, and cannot relicense the model under a more restrictive license like GPL.

> See the [Hugging Face license documentation](https://huggingface.co/docs/hub/en/repositories-licenses) for details.

## Setup

1. Install dependencies:

    ```
    pip install transformers torch
    ```

    - `transformers` is the Hugging Face core library for model access.
    - `torch` is required for most model backends (PyTorch).

2. Example: load and use the model in Python

    ```
    from transformers import AutoModel, AutoTokenizer

    model_name = "google/bert_uncased_L-2_H-128_A-2"
    model = AutoModel.from_pretrained(model_name)
    tokenizer = AutoTokenizer.from_pretrained(model_name)
    ```

3. Check the `urls.txt` for details of which models are being used.

## License Notice

This repo and any outputs from using the model should include attribution:
- Cite the original Hugging Face model and its authors.
- Retain the Apache 2.0 license notice if distributing code or derived models.

