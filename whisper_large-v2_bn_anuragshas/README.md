# Whisper Large-v2 Bengali by [Anurag Singh](https://github.com/anuragshas)

This model is a fine-tuned version of [openai/whisper-large-v2](https://huggingface.co/openai/whisper-large-v2) on the mozilla-foundation/common_voice_11_0 bn dataset.
It achieves the following results on the evaluation set:

- Loss: 0.0746
- Wer: 11.1086

## Model description

More information needed

## Intended uses & limitations

More information needed

## Training and evaluation data

More information needed

## Training procedure

### Training hyperparameters

The following hyperparameters were used during training:

- learning_rate: 1e-05
- train_batch_size: 32
- eval_batch_size: 16
- seed: 42
- distributed_type: multi-GPU
- optimizer: Adam with betas=(0.9,0.999) and epsilon=1e-08
- lr_scheduler_type: linear
- lr_scheduler_warmup_steps: 100
- training_steps: 1000

### Training results

| Training Loss | Epoch | Step | Validation Loss |   Wer   |
| :-----------: | :---: | :--: | :-------------: | :-----: |
|     0.046     | 1.21  | 1000 |     0.0746      | 11.1086 |

### Framework versions

- Transformers 4.26.0.dev0
- Pytorch 1.13.0+cu117
- Datasets 2.7.1.dev0
- Tokenizers 0.13.2

[mozilla-foundation/common_voice_11_0](https://huggingface.co/datasets/mozilla-foundation/common_voice_11_0)

## Evaluation Dataset:

[mozilla-foundation/common_voice_11_0](https://huggingface.co/datasets/mozilla-foundation/common_voice_11_0)

## Credits

This package includes a model that is licensed under the Apache License, Version 2.0. A copy of the Apache License, Version 2.0 can be found in the [LICENSE](LICENSE) file.
Copyright 2022 [Anurag Singh](https://github.com/anuragshas)

## Citation

```bibtex
@misc{anuragshas2022whispersmallbn,
  author = {Anurag Singh},
  title = {Whisper Small Bangla},
  year = {2022},
  publisher = {Hugging Face},
  howpublished = {\url{https://huggingface.co/anuragshas/whisper-large-v2-bn}},
}
```
