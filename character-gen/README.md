# CharacterGen

CharacterGen: Efficient 3D Character Generation from Single Images with Multi-View Pose Canonicalization

## Overview

CharacterGen is an innovative framework for generating high-quality 3D character models from single 2D images. It addresses the challenges of diverse body poses, self-occlusion, and pose ambiguity by introducing a streamlined generation pipeline along with an image-conditioned multi-view diffusion model.

## Key Features

- Generates 3D character models in a canonical A-pose from single images with arbitrary poses
- Introduces a multi-view pose canonicalization diffusion model
- Employs a transformer-based, generalizable sparse-view reconstruction model
- Utilizes a texture-back-projection strategy for high-quality texture maps
- Processes a single image into a 3D character model in less than 1 minute

## Resources

- [GitHub Repository](https://github.com/zjp-shadow/CharacterGen)
- [arXiv Paper](https://arxiv.org/pdf/2402.17214)
- [Hugging Face Model](https://huggingface.co/zjpshadow/CharacterGen)

## Dataset

The authors curated a dataset of anime characters, Anime3D, consisting of:
- 13,746 stylized character subjects
- Multiple poses and views for each character
- Rendered using the three-vrm framework

## Method

CharacterGen's pipeline consists of two main stages:

1. Multi-view Image Generation and Pose Canonicalization
   - Uses IDUNet for transferring patch-level appearance features
   - Employs a multi-view UNet for generating consistent A-pose images
   - Incorporates pose embedding for better character layout

2. 3D Character Generation
   - Utilizes a two-stage transformer-based network for geometry and coarse appearance reconstruction
   - Applies a texture back-projection strategy for high-quality textures
   - Uses Poisson Blending to reduce seams on the texture map

## Applications

CharacterGen can be used for various applications in digital content creation, including:
- Character design for video games
- Animation pre-production
- Virtual reality (VR) avatar creation
- Rapid prototyping of 3D characters

## Citation

If you use CharacterGen in your research, please cite the paper:

```bibtex
@article{peng2024charactergen,
  title={CharacterGen: Efficient 3D Character Generation from Single Images with Multi-View Pose Canonicalization},
  author={Peng, Hao-Yang and Zhang, Jia-Peng and Guo, Meng-Hao and Cao, Yan-Pei and Hu, Shi-Min},
  journal={arXiv preprint arXiv:2402.17214},
  year={2024}
}