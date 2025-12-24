Just my personal workflow, consisting of:

* **Wan 2.2 14B Architecture**: High-Noise and Low-Noise Model.
* **4-Step Turbo Generation**: accelerated using the `Lightx2v` 4-step LoRA for rapid inference.
* **Optimization**: Uses `SageAttention2` and Implements `PatchSageAttentionKJ` and `ModelPatchTorchSettings` for better memory efficiency.
* **Post-Processing Pipeline**:
    * **Sharpening**: Contrast Adaptive Sharpening `ImageCASharpening+` for detail enhancement.
    * **Upscaling**: 4x upscale using the `Remacri` model.
    * **Interpolation**: RIFE TensorRT implementation for faster and smooth frame rate doubling.
