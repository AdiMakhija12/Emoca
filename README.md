Project Title:
Emotion Driven Monocular Face Capture and Animation (EMOCA) Replication

Project Description:
Our project aimed to replicate and understand the EMOCA (EMOtion Capture and Animation) framework, which sets a new standard for emotion-driven, monocular 3D face reconstruction from images. EMOCA's core innovation is its ability to capture subtle and extreme emotional expressions from a single input image, producing animatable and highly realistic 3D face models.

Background:
While 3D facial avatars are increasingly being used in communication, entertainment, and AR/VR, most existing reconstruction methods struggle to faithfully reproduce emotional expressions. Traditional training losses such as landmark reprojection, photometric, and face recognition losses do not ensure that the reconstructed geometry reflects the emotional state present in the original image.

Methodology:
EMOCA tackles this challenge by introducing a novel deep perceptual emotion consistency loss during training. This loss ensures that the emotional content of the reconstructed 3D face matches that of the input image, making it possible to accurately reconstruct expressions regardless of their subtlety or extremeness. The framework builds on DECA, a state-of-the-art 3D face reconstruction platform, and augments it with an additional trainable branch responsible for facial expression prediction.

Key steps include:

Training a powerful emotion recognition model as part of the supervision.

Regulating the expression part of the model using emotion-rich datasets, while keeping the identity branch fixed to preserve state-of-the-art shape accuracy.

Directly regressing valence and arousal values, enabling the 3D model to convey nuanced emotional states.

The output is an animatable mesh with high-fidelity facial geometry and texture.

Results:
Based on our replication, EMOCA demonstrates:

Comparable identity shape reconstruction accuracy to the best existing methods.

Superior performance in reconstructing the quality and perceived emotional content in 3D facial expressions.

In-the-wild emotion recognition capability, with results matching the best image-based approaches—highlighting the utility of 3D facial geometry for automatic emotion analysis.

Potential applications in gaming, movies, VR/AR, communication, and social robotics.

Conclusion:
EMOCA represents an important advance in the intersection of 3D face reconstruction and emotion analysis. By ensuring emotional fidelity in reconstructed avatars, EMOCA opens new avenues for research and application in expressive computer vision, virtual communication, and digital human modeling.

References:

EMOCA Official Repository: [radekd91/emoca (GitHub)]

Original Paper: CVPR 2022 – Danecek et al.
