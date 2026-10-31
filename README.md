# Vehicularis edge models

Open models that Vehicularis apps download on first use and run on the device. The ones released
here are not ours: each is an unmodified copy of a published model, redistributed under its own
licence. Models we train ourselves are released from their own repositories and listed under
[Our own models](#our-own-models).

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

## Read aloud (`tts-v1`)

| File | What it is | Bytes | SHA-256 |
| --- | --- | --- | --- |
| `config.json` | Phonon 31M configuration | 4634 | `b5d0f88353638370d94035b7d73d7d6577c0554d78f8d7ecfd40490aae39ae85` |
| `tokenizer.json` | Phonon 31M tokenizer | 277967 | `691a00068fa7b989f2f3e5ae5daa2d1a5bb319f2d5360deafcfb19a8bb6e7936` |
| `model.q8.gguf` | Phonon 31M weights, 8-bit | 64512352 | `a7d9aad2cd6dc66473f24a08bc6d2939030ef4d751ef82349361fbef3272dbae` |
| `easton.safetensors` | The Easton voice (American English, male) | 256136 | `45c582673cb20edb04ddcca2b5a8865ddfb0a82599efadb269021e87d20fbdd4` |

| Files | Model by | Source | Licence |
| --- | --- | --- | --- |
| `config.json`, `tokenizer.json`, `model.q8.gguf` | [Gradium Phonon](https://huggingface.co/gradium/phonon-31m-en), built on Kyutai's Pocket TTS and Mimi | [Hugging Face](https://huggingface.co/gradium/phonon-31m-en/tree/92741c5b07d085ff840e26fea8ce43110b87852f) | Apache-2.0 |
| `easton.safetensors` (`voices/LMDIYE0Oa377Qh6Z.safetensors` upstream) | [Gradium Phonon voices](https://huggingface.co/gradium/phonon-voices) | [Hugging Face](https://huggingface.co/gradium/phonon-voices/tree/0ee17205f254b5abc43b266c8a0f215565c352f7) | Apache-2.0 |

All unmodified apart from the voice file's name. The notices are in [TTS-LICENSES.txt](TTS-LICENSES.txt), which is also attached to the release.

## Our own models

| Model | What it is | Release | Licence |
| --- | --- | --- | --- |
| TabTasker Workflow AI 0.6B | Qwen3-0.6B fine-tuned to write TabTasker workflow graphs, ONNX 4-bit for Transformers.js | [`v1` in tabtasker-workflow-0.6b](https://github.com/vehicularis/tabtasker-workflow-0.6b/releases/tag/v1) | Apache-2.0 |

`model_q4.onnx` in that release: 996522547 bytes, SHA-256 `bac4a8c7802d31a93aa18ea8a839d7a71a3ba95f3c40d8675f279baee689b614`.
