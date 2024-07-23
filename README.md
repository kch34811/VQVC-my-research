![POSTECH](https://img.shields.io/badge/POSTECH-%239a034c)
<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white"/>

# One-Shot Voice Conversion Using VQVC Model
This research was conducted based on the prior work <a href="https://github.com/Jackson-Kang/VQVC-Pytorch">Jackson-Kang/VQVC-Pytorch</a>.

## Overview
This repository contains the implementation of a one-shot voice conversion model using the VQVC framework. The model aims to transform a source speaker's voice into a target speaker's voice using only a single example, leveraging minimal data for practical and scalable applications. The model separates content and speaker information to enhance speech processing technology, enabling precise control and generalization to new speakers.

## Key Features
* One-shot Voice Conversion: Transform voices with minimal data.
* VQVC Model: Utilizes Vector Quantization for separating content and speaker information.
* WavLM Integration: Generates SSL features directly from waveforms for high-quality embeddings.
* Vocoder (VocGAN): Converts Mel-spectrograms to final audio waveforms.
* Loss Functions: Includes Reconstruction Loss and Latent Loss to ensure model stability and efficiency.

## Dataset
CSTR VCTK Corpus: Audio data from 110 English speakers with various accents.

## Model Components
Encoder: Extracts features from input speech.
Vector Quantization (VQ): Separates content and speaker identity.
Decoder: Reconstructs the speech from quantized features.

## Performance Evaluation
Subjective Listening Tests: Evaluated using Mean Opinion Score (MOS) and Speaker Mean Opinion Score (SMOS).
Comparative Analysis: The proposed model outperforms the baseline VQVC model in both audio quality and speaker similarity.

## Limitations
Validation limited to English speakers.
Evaluation primarily based on subjective listening tests.

## References
1. Van Den Oord, A., & Vinyals, O. (2017). Neural discrete representation learning. Advances in neural information processing systems, 30.
2. Chen, S., et al. (2022). Wavlm: Large-scale self-supervised pre-training for full stack speech processing. IEEE Journal of Selected Topics in Signal Processing, 16(6), 1505-1518.
3. Wan, L., et al. (2018). Generalized end-to-end loss for speaker verification. In 2018 IEEE International Conference on Acoustics, Speech and Signal Processing (ICASSP) (pp. 4879-4883). IEEE.
