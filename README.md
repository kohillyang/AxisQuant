# AxisQuant

**INT8 inference engines for vision transformers, designed from the kernel side.**

AxisQuant runs the SAM 2.1, SAM 3, DINOv3, ViT and DeiT image encoders on INT8 tensor
cores at 1.2–2× the speed of TensorRT FP16 with no measurable accuracy loss at W8A8:
ImageNet top-1 within 0.05 points of fp32, SAM 3 COCO segm AP within 0.0003, zero-shot
ImageNet with the DINOv3 dino.txt head unchanged. It is the code behind the paper

> *AxisQuant: Rethinking Post-Training Quantization of Vision Transformers from the Kernel Side*
