<!-- {
    "url": "https://github.com/shhossain/whisper_base_bn_sifat",
    "name": "whisper-base-bn-sifat",
    "type": "base",
    "host": "github.com",
    "cloneable": true,
    "private": false,
    "license": "apache-2.0",
    "author": "Sifat"
} -->

# How to use

## Prerequisites
- [Python 3+](https://www.python.org/downloads/)
- [Pytorch](https://pytorch.org/get-started/locally/)
- [Transformers](https://huggingface.co/transformers/installation.html)


## Installation

```bash
pip install transformers
```

```bash
pip install PyAudio
```

```bash
pip install torch
```
__Note__: This is only simple installation of pytorch. For more details, please visit [Pytorch](https://pytorch.org/get-started/locally/)

## Usage

Clone any model from the config file in each model directory. For example, to clone the `whisper-base-bn-sifat` model, run:

```bash
git clone https://github.com/shhossain/whisper_base_bn_sifat
```

Then, you can use the model in your code:


```python
from transformers import pipeline

pipe = pipeline('automatic-speech-recognition', model='path/to/whisper-base-bn-sifat',device=0)

def transcribe(audio_file):
    return pipe(audio_file)

print(transcribe('audio.wav'))
```
__Note__: For `device` refer to [Pytorch](https://pytorch.org/)