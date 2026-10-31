# Vehicularis edge models

Open models that Vehicularis apps download on first use and run on the device. None of them
are ours: each is an unmodified copy of a published model, redistributed under its own licence.

Each set is a release. A release's model files never change, so apps pinned to it keep working
(and they check every file's SHA-256 anyway). A new or updated model goes in a new release.

## Voice (`voice-v1`)

| File | What it is | Bytes | SHA-256 |
| --- | --- | --- | --- |
| `ggml-large-v3-turbo-q8_0.bin` | Whisper large-v3 Turbo, 8-bit, for whisper.cpp | 874188075 | `317eb69c11673c9de1e1f0d459b253999804ec71ac4c23c17ecf5fbe24e259a1` |
| `ggml-silero-v6.2.0.bin` | Silero VAD v6.2.0 (voice activity detection), for whisper.cpp | 885098 | `2aa269b785eeb53a82983a20501ddf7c1d9c48e33ab63a41391ac6c9f7fb6987` |

| File | Model by | Converted to ggml by | Source | Licence |
| --- | --- | --- | --- | --- |
| `ggml-large-v3-turbo-q8_0.bin` | [OpenAI Whisper](https://github.com/openai/whisper) | [whisper.cpp](https://github.com/ggml-org/whisper.cpp) | [Hugging Face](https://huggingface.co/ggerganov/whisper.cpp/tree/5359861c739e955e79d9a303bcbc70fb988958b1) | MIT |
| `ggml-silero-v6.2.0.bin` | [Silero VAD](https://github.com/snakers4/silero-vad) | [whisper.cpp](https://github.com/ggml-org/whisper.cpp) | [Hugging Face](https://huggingface.co/ggml-org/whisper-vad/tree/9ffd54a1e1ee413ddf265af9913beaf518d1639b) | MIT |

The full notices are in [VOICE-LICENSES.txt](VOICE-LICENSES.txt), which is also attached to the release.
