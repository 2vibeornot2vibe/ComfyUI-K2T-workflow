# ComfyUI-K2T-workflow

Simple ComfyUI workflow for Krea 2 Turbo.

<img width="1348" height="729" alt="K2T" src="https://github.com/user-attachments/assets/4d44946c-e3a7-45a8-ae4a-bbe5cc35bf2b" />

## Setup

### Install Custom Nodes

**1. WAS Node Suite (Revised)**: Install via ComfyUI-Manager.

**2. ComfyUI-ConditioningKrea2Rebalance ([GitHub Repository](https://github.com/nova452/ComfyUI-ConditioningKrea2Rebalance))**: Open a terminal window in the `custom-nodes` folder in ComfyUI's root directory and run
```bash
git clone https://github.com/nova452/ComfyUI-ConditioningKrea2Rebalance
```

### Download Models

**1. Download the models from your preferred source:**
[Hugging Face🤗](https://huggingface.co/Comfy-Org/Krea-2/tree/main)
[HF-Mirror🤗](https://hf-mirror.com/Comfy-Org/Krea-2/tree/main)
[ModelScope](https://modelscope.cn/models/Comfy-Org/Krea-2/files)

**2. Download one of each and save them into the corresponding folders inside ComfyUI's `models` directory:**
*   **diffusion_models** (krea2_turbo_bf16.safetensors / krea2_raw_fp8_scaled.safetensors)
*   **text_encoders** (qwen3vl_4b_bf16.safetensors / qwen3vl_4b_fp8_scaled.safetensors)
*   **vae** (qwen_image_vae.safetensors)
*   **loras (optional)**

If you have enough combined memory **(RAM+VRAM > 32GB)**, get BF16 for better quality. Otherwise, use FP8 versions.

## Use

Select your downloaded models in the `Load Models` node.

Un-bypass the `Load LoRA` node and select your downloaded LoRA if you have any.

Set image resolution in the `Image Controls` node and enable `🌽` for 🌽 ;)

Enter your prompt and generate!

## License

**DO WHATEVER YOU WANT WITH IT :D**
