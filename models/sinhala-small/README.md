# Sinhala Whisper Small (browser build)

8-bit ONNX conversion of [SinhaSpeech/whisper-small-sinhala-run12-best](https://huggingface.co/SinhaSpeech/whisper-small-sinhala-run12-best)
(Apache-2.0; reported 15.52% WER / 4.36% CER on its Sinhala test set), for use with transformers.js.
The .onnx files are split into 45 MB parts (see parts.json) to fit GitHub's file size limit; the app joins them while loading.
