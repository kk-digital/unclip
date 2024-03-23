# unclip

we follow the training guide of kandinsky 2.2 from diffusers repo

https://huggingface.co/docs/diffusers/en/training/kandinsky

# dataset

we should use reach-vb/pokemon-blip-captions as demo dataset.

https://huggingface.co/datasets/reach-vb/pokemon-blip-captions


```python
import datasets

# first we load it from huggingface

dataset = datasets.load_dataset('reach-vb/pokemon-blip-captions')

dataset.save_to_disk('pokemon-blip-captions')

# later we can load it from local path

dataset = datasets.load_dataset('arrow', data_files={'train': './pokemon-blip-captions/train/data-00000-of-00001.arrow'})
```
