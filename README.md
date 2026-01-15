# Fine Data Generation

(This repo is based on Stable Diffusion and [attend-and-excite](https://github.com/yuval-alaluf/Attend-and-Excite))

Demo repo showing how to:

- generate images with different Stable Diffusion based models
- fine-tune Stable Diffusion with **LoRA** to generate a specific kind of data

## Notebooks

- [notebooks/compare_models.ipynb](notebooks/compare_models.ipynb)
    - same prompt + same seeds across models
  
![Different models with the same prompt](link)

- [notebooks/train_sd35_lora.ipynb](notebooks/train_sd35_lora.ipynb)
    - LoRA training (Diffusers + Accelerate)
    - load the LoRA for inference

![Effect of fine tuning](link)
![Explainability](link)

## Install

Recommended (editable install so notebooks import local code):

```bash
python -m venv .venv
source .venv/bin/activate
pip install -e .
```

Alternative: `pip install -r requirements.txt`

## Hugging Face token (SD 3.5 / gated models)

Some models (e.g. SD 3.5) require that you accept terms on Hugging Face and provide a token:

```bash
export HF_TOKEN=hf_...
```

Restart the notebook kernel after setting the token.
