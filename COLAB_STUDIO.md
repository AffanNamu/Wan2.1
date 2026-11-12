# Wan2.1 Cinematic Colab Studio

A one-run Google Colab notebook for turning a still film-scene image into a short cinematic video using the official Wan2.1 VACE 1.3B model.

## Open the notebook in Google Colab

[**Open Wan2.1 Cinematic Colab Studio**](https://colab.research.google.com/github/AffanNamu/Wan2.1/blob/main/notebooks/Wan2.1_Cinematic_Colab_Studio.ipynb)

## How to use

1. Open the Colab link.
2. In Colab select **Runtime → Change runtime type → T4 GPU** (or another available GPU).
3. Click **Runtime → Run all**.
4. When asked, upload a scene image.
5. Enter the motion/camera prompt when prompted.
6. Wait for generation; the notebook previews and downloads the MP4.

## Important notes

- Uses Wan2.1 **VACE 1.3B** reference-to-video mode, suitable for animating a still reference image.
- The model weights are downloaded automatically from Hugging Face during the run.
- The notebook installs dependencies and runs inference; no manual Python editing is required.
- Google Colab free GPU access, session length, memory, and quotas are controlled by Google and are not guaranteed. A GPU runtime is required.
- 480p output and 81 frames (~5 seconds) are the configured defaults.
- If the session runs out of GPU memory, try a higher-memory GPU runtime if available.
- This repository is a user fork of the official project: https://github.com/Wan-Video/Wan2.1
- Model: https://huggingface.co/Wan-AI/Wan2.1-VACE-1.3B
- Official project license and model terms apply. Review the upstream license before commercial use.

