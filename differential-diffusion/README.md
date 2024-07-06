# Differential Diffusion

Differential Diffusion: Giving Each Pixel Its Strength

Differential Diffusion is a groundbreaking framework in the field of image generation and editing. It enhances the capabilities of existing diffusion models by allowing customization of the amount of change per pixel or image region. This framework operates solely during inference, requiring no model training or fine-tuning.

## Key Features

- **Granular Control**: Allows different regions of an image to be edited by varying degrees according to a given map and text prompt.
- **Seamless Blending**: Facilitates the reproduction of gradual processes and smooth transitions between varying edit strengths.
- **Soft-Inpainting**: Enhances inpainting by subtly adjusting surrounding areas for seamless integration.
- **Efficiency**: Operates during inference with minimal memory overhead and no need for model training.

## Resources

- [Differential Diffusion Website](https://differential-diffusion.github.io/)
- [GitHub Repository](https://github.com/exx8/differential-diffusion)
- [Research Paper (PDF)](https://differential-diffusion.github.io/paper.pdf)

## Abstract from the Research Paper

Diffusion models have revolutionized image generation and editing, producing state-of-the-art results in both conditioned and unconditioned image synthesis. Current techniques enable user control over the degree of change in an image edit but are limited to global changes over an entire edited region. This paper introduces a novel framework that enables customization of the amount of change per pixel or per image region, enhancing existing diffusion models with this capability. Granular control of the quantity of change opens up a diverse array of new editing capabilities, such as control of the extent to which individual objects are modified and the ability to introduce gradual spatial changes.

Our framework operates solely during inference, requiring no model training or fine-tuning. We demonstrate our method with the current open state-of-the-art models, validating it via both quantitative and qualitative comparisons, and a user study.

## Example Applications

- **Fire Simulation**: Gradual introduction of fire into different regions of a photo, creating a realistic simulation of fire spreading.
- **Fantasy Art**: Create intricate fantasy scenes with varying levels of detail and transformation.
- **Depth Edits**: Control the extent of modifications to individual objects in a scene, preserving the overall structure while making targeted changes.

## Contributions

- Introduction of the "change map" concept, generalizing the traditional "mask" used in image editing.
- Extension of the framework to achieve better soft-inpainting.
- Introduction of a tool for visualizing the effects of different edit strengths, called the "Strength Fan".
- Development of new evaluation metrics for comparing techniques based on adherence to a change map.

Feel free to explore the provided resources for a deeper understanding of Differential Diffusion. More detailed explanations and insights will be added here as the content is reviewed and understood.
