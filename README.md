# Resource-Efficient Inference: Quantization and Pruning Strategies for Obfuscated Gambling Detection

## Overview
This dataset contains images specifically curated to train and evaluate computer vision models for detecting online gambling promotions. Unlike standard datasets, these images focus on **visual obfuscation**—techniques used by malicious actors to bypass traditional keyword-based text filters (e.g., embedding deceptive text, slot machine iconography, and masked promotional banners within images).

## Dataset Structure
The dataset is categorized into a binary classification structure:
*   `1_Gambling/`: Images containing explicitly obfuscated or direct online gambling promotions.
*   `0_NonGambling/`: Control images representing normal social media content, internet memes, and standard advertisements to prevent false positives.

## Preprocessing Requirements
To replicate the experimental results achieved using the MobileNetV2 architecture in this study, the following preprocessing pipeline must be applied to all input images prior to inference:
1.  **Resize:** Scale images to exactly `224x224` pixels.
2.  **Color Space:** Ensure images are converted to `RGB` format.
3.  **Normalization:** Apply standard ImageNet tensor normalization:
    *   Mean: `[0.485, 0.456, 0.406]`
    *   Standard Deviation: `[0.229, 0.224, 0.225]`

## License

[![CC BY-NC 4.0](https://img.shields.io/badge/License-CC%20BY--NC%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc/4.0/)

This dataset is public open data scraped from the web. It is made available under the **Creative Commons Attribution-NonCommercial 4.0 International (CC BY-NC 4.0)** license. 

Under this license, you are free to:
* **Share** — copy and redistribute the material in any medium or format
* **Adapt** — remix, transform, and build upon the material

Under the following terms:
* **Attribution** — You must give appropriate credit, provide a link to the license, and indicate if changes were made.
* **NonCommercial** — You may not use the material for commercial purposes.

## Disclaimer

This dataset is provided strictly for academic and research purposes to aid in the development of automated, edge-efficient content moderation systems. Users are responsible for ensuring compliance with the source platform's Terms of Service and local data regulations.
