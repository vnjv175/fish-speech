# Fish Speech

Text-to-speech (TTS) synthesis framework from Fish Audio, supporting high-quality voice cloning and multilingual speech generation with PyTorch and Gradio.

## Tech Stack

- **Language:** Python 3.10+
- **Framework:** PyTorch 2.8, Lightning, Hydra
- **Other:** Gradio (web UI), transformers, librosa, TensorBoard, WandB, gRPC, uvicorn, tiktoken

## Development

```bash
# Install (with uv, recommended)
uv pip install -e .

# Install with specific CUDA version
uv pip install -e ".[cu128]"

# CPU only
uv pip install -e ".[cpu]"

# Run inference server
python -m fish_speech.serve
```

## Project Structure

- `fish_speech/` -- Core TTS package
- `tools/` -- Training and inference utilities
- `configs/` -- Hydra configuration files

## Conventions

- uv for dependency management with multiple CUDA extras
- setuptools build backend
- Fish Audio Research License
