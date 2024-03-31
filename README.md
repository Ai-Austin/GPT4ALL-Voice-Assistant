# GPT4ALL-Voice-Assistant
This is a 100% offline GPT4ALL Voice Assistant. Completely open source and privacy-friendly. Use any language model on GPT4ALL. Background process voice detection. Watch the full YouTube tutorial for the setup guide: https://youtu.be/6zAk0KHmiGw
## Setup
I would highly suggest you watch the YouTube tutorial to use this code. You will need to modify the OpenAI whisper library to work offline and I will walk through that in the video and set up all the other dependencies to function properly.

To use piper-tts neural voices, you need to download both model and config for the voice of your choice from [their Github page](https://github.com/rhasspy/piper/blob/master/VOICES.md) and extract both `.onnx` and `.onnx.json` files in the same folder. Take note of the path; you'll need to replace it in the `main.py` to work correctly.

If you're planning on installing it on Arch-based distros, you need to install `espeak` and `python-espeak` packages from the AUR. You can install them using `yay` utility by running:
```bash
yay -S espeak python-espeak
```
## Improvements to think about adding to yours
Give a system prompt. These open-source models perform far better when you send a system prompt as specified in the GPT4ALL documentation: https://docs.gpt4all.io/gpt4all_python.html#introspection
