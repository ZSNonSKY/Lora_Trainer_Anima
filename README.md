# Lora_Trainer_Anima
Accessible Google Colab notebooks for Anima LoRA & LoHa training, based on the work of kohya-ss, Linaqruf and hollowstrawberry

|:--|:-:|:-:|
| 🌟 **Lora Trainer Anima** | [![Open in Colab](https://raw.githubusercontent.com/hollowstrawberry/kohya-colab/main/assets/colab-badge.svg)](https://colab.research.google.com/github/ZSNonSKY/Lora_Trainer_Anima/blob/main/Lora_Trainer_Anima.ipynb) |

# 🌟 Anima Lora Trainer

A fork of [hollowstrawberry](https://github.com/hollowstrawberry)'s [XL Lora Trainer](https://github.com/hollowstrawberry/kohya-colab), rebuilt to train Loras and (Lycoris) Loha's for [Anima](https://huggingface.co/circlestone-labs/Anima) by circlestone-labs — a 2B parameter Diffusion Transformer built on NVIDIA's Cosmos-Predict2, using a Qwen3-0.6B text encoder and the Qwen-Image VAE.

Unlike the original notebook this fork trains directly against [kohya-ss/sd-scripts](https://github.com/kohya-ss/sd-scripts)'s native `anima_train_network.py`, rather than through a wrapper backend, since Anima's training needs (Rectified Flow, no conv layers, an optional LLM adapter) don't map onto the SDXL settings that trainer was built around.

Colab's free T4 GPU (15GB VRAM) is enough for this. Colab Pro with a better GPU will train faster and allow bigger batches.

This colab is possible thanks to open source code from talented people:
* [kohya-ss](https://github.com/kohya-ss/sd-scripts) for sd-scripts and its native Anima support
* [circlestone-labs](https://huggingface.co/circlestone-labs) for Anima
* [hollowstrawberry](https://github.com/hollowstrawberry/kohya-colab) for the original XL Lora Trainer this fork is based on
* [derrian-distro](https://github.com/derrian-distro/LoRA_Easy_Training_scripts_Backend/), [Linaqruf](https://github.com/Linaqruf/kohya-trainer) and [Jelosus2](https://github.com/Jelosus2/LoRA_Easy_Training_Colab), whose earlier work shaped the original notebook this one descends from
