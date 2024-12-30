## Videodubber

MuseTalk: Real-Time High Quality Lip Synchronization with Latent Space Inpainting
Yue Zhang *, Minhao Liu*, Zhaokang Chen, Bin Wu†, Yingjie He, Chao Zhan, Wenjiang Zhou (*Equal Contribution, †Corresponding Author, benbinwu@tencent.com)


## Overview

**MuseTalk** is a real-time, high-quality audio-driven lip-syncing model trained in the latent space of **ft-mse-vae**, which:

- Modifies an unseen face according to the input audio, with a face region size of **256 x 256**.
- Supports audio in various languages, including **Chinese**, **English**, and **Japanese**.
- Enables real-time inference at **30fps+** on an NVIDIA Tesla V100.
- Allows modification of the center point of the face region, which **significantly affects generation results**.
- Includes a checkpoint trained on the **HDTF dataset**.
- Provides training codes (**coming soon**).

##Model Structure

MuseTalk was trained in latent spaces, where the images were encoded by a freezed VAE. The audio was encoded by a freezed whisper-tiny model. The architecture of the generation network was borrowed from the UNet of the stable-diffusion-v1-4, where the audio embeddings were fused to the image embeddings by cross-attention.
