## Videodubber

MuseTalk: Real-Time High Quality Lip Synchronization with Latent Space Inpainting
Yue Zhang *, Minhao Liu*, Zhaokang Chen, Bin Wu†, Yingjie He, Chao Zhan, Wenjiang Zhou (*Equal Contribution, †Corresponding Author, benbinwu@tencent.com)


#Overview
MuseTalk is a real-time high quality audio-driven lip-syncing model trained in the latent space of ft-mse-vae, which

modifies an unseen face according to the input audio, with a size of face region of 256 x 256.
supports audio in various languages, such as Chinese, English, and Japanese.
supports real-time inference with 30fps+ on an NVIDIA Tesla V100.
supports modification of the center point of the face region proposes, which SIGNIFICANTLY affects generation results.
checkpoint available trained on the HDTF dataset.
training codes (comming soon).
