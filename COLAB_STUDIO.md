# Wan2.1 Cinematic Audio Studio

A Google Colab workflow that combines:
- Wan2.1 VACE 1.3B for image-conditioned cinematic motion.
- Edge TTS for spoken character dialogue and optional narration.
- MuseTalk 1.5 for audio-driven lip synchronization.
- FFmpeg for mixing dialogue, narration, and an optional ambience/music track into a final MP4.

## Open in Google Colab

[**Open Wan2.1 Cinematic Audio Studio**](https://colab.research.google.com/github/AffanNamu/Wan2.1/blob/main/notebooks/Wan2.1_Cinematic_Audio_Studio.ipynb)

## Run instructions

1. In Colab, choose Runtime → Change runtime type → GPU.
2. Run all cells.
3. Upload a scene image.
4. Enter the visual prompt and the exact character dialogue.
5. Optionally enter narration and upload a background ambience/music/sound-effects file.
6. Wait for the scene animation, TTS, MuseTalk lip-sync, and final audio mix.
7. Preview and download the MP4.

## Technical notes

- Wan2.1 VACE generates the moving visual scene; it does not generate synchronized dialogue audio in this workflow.
- MuseTalk 1.5 is a separate audio-driven lip-sync model and requires a visible, detectable face. It can struggle with profile views, occlusions, tiny faces, and complex shots.
- The notebook creates an isolated Python 3.10 environment for MuseTalk because its pinned dependencies are older than the default Colab runtime.
- Edge TTS requires an internet connection and uses Microsoft's online speech service. Voice availability depends on the selected voice locale.
- Google Colab GPU availability, quota, session lifetime, and memory are not guaranteed. This pipeline downloads multiple large model checkpoints.
- AI-generated output should be disclosed appropriately. Only use voices and likenesses with permission.

## Upstream projects

- Wan2.1: https://github.com/Wan-Video/Wan2.1
- Wan2.1 VACE weights: https://huggingface.co/Wan-AI/Wan2.1-VACE-1.3B
- MuseTalk: https://github.com/TMElyralab/MuseTalk
- Edge TTS: https://github.com/rany2/edge-tts

Follow all upstream code and model licenses.
