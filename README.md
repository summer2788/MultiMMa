# Enhanced MultiMAE: Multi-modal Multi-task Masked Autoencoders with Prompt Tuning

Enhanced MultiMAE introduces the integration of prompt tuning into the Multi-modal Multi-task Masked Autoencoders (MultiMAE) framework for more efficient and adaptable multi-modal, multi-task learning, particularly focusing on vision tasks such as depth estimation and semantic segmentation.

## Table of Contents

- [Introduction](#introduction)
- [Installation](#installation)
- [Usage](#usage)
- [Features](#features)
- [Data](#data)
- [Methodology](#methodology)
  - [Pre-training](#pre-training)
  - [Fine-tuning](#fine-tuning)
  - [Prompt Tuning](#prompt-tuning)
- [Experiments and Results](#experiments-and-results)
- [Future Research Directions](#future-research-directions)
- [Acknowledgements](#acknowledgements)
- [License](#license)
- [Citations](#citations)

## Introduction

Building upon the original MultiMAE, this version extends its capabilities by incorporating prompt tuning to efficiently apply pre-trained models to downstream tasks. This approach enables effective parameter tuning without the need for extensive re-training, particularly addressing the challenges of applying traditional natural language processing techniques to vision tasks.

## Installation

Refer to the original MultiMAE setup instructions in [SETUP.md](SETUP.md) for basic environment setup.

## Usage

Usage instructions remain consistent with the original MultiMAE documentation. See [USAGE.md](USAGE.md) for comprehensive guidelines on pre-training, fine-tuning, and utilizing the models.

## Features

- **Multi-modal, Multi-task Learning:** Leverage pre-trained models across different tasks including depth estimation and semantic segmentation.
- **Prompt Tuning Integration:** Introduces the ability to fine-tune models for specific tasks with minimal parameter adjustments.
- **Efficient Learning:** Reduces the need for extensive computational resources, enabling faster adaptation to new tasks.

## Data

Utilizes the NYU Depth Dataset V2 (NYUv2), a benchmark for segmentation and depth estimation in various indoor environments.

## Methodology

### Pre-training

Follows the MultiMAE's approach, pre-training on the ImageNet dataset with masked autoencoder models to learn rich feature representations.

### Fine-tuning

Includes task-specific fine-tuning for depth estimation and semantic segmentation, employing task-specific decoders and evaluation metrics.

### Prompt Tuning

Introduces deep prompt tuning and prompt pool strategies to adapt the model to various tasks with minimal adjustments, significantly reducing the number of parameters needed for effective learning.

## Experiments and Results

Conducted experiments demonstrate the effectiveness of prompt tuning in multi-task settings, achieving competitive performance with reduced model complexity and training time.

## Future Research Directions

Suggests further exploration into task-specific prompt pooling and efficient normalization techniques to enhance model adaptability and performance across diverse tasks.

## Acknowledgements

Credits to the original MultiMAE project and its contributors. This enhancement also builds upon foundational works in prompt tuning and multi-task learning in the vision domain.

## License

This project is licensed under the same terms as the original MultiMAE project. See [LICENSE](LICENSE) for more details.

## Citations

Refer to the original MultiMAE citation and additional references related to prompt tuning and its application to vision tasks as documented in the research document.


