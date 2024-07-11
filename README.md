当然，以下是所有内容放在一个代码框里的版本：

```markdown
# Orpaint: Oracle Bone Inscription Restoration

## Abstract

Oracle bone inscription rubbings, which are grayscale images copied from turtle shells and animal bones, are extremely precious materials for the study of oracle bone studies. However, due to natural and anthropogenic factors that have damaged the turtle shells and animal bones, most of the existing oracle bone inscription rubbings have been damaged to varying degrees, which has hindered subsequent research. Therefore, the research objective of this paper is to restore the damaged oracle bone inscription rubbings. The paper intends to use a generative model, specifically a diffusion model, for the restoration.

Traditional methods based on diffusion models, which couple a large number of self-attention modules and residual connection modules in the U-net denoising network, result in high computational costs and are difficult to scale up to high-resolution images. In response to this issue, this paper proposes a novel zero-shot oracle bone inscription image restoration model named Orpaint. It innovatively employs a U-net network based on a pure visual state-space model instead of the traditional denoising network, achieving a model that scales with linear complexity.

Experiments have demonstrated that Orpaint can significantly reduce model complexity and accelerate the restoration speed without sacrificing restoration performance and has good scalability for high-resolution oracle bone inscription rubbings. Moreover, under sufficient pre-training, Orpaint can be effectively transferred to other restoration tasks, exhibiting excellent generalization performance. The code for this paper has been made open-source at: [https://github.com/YMlinfeng/Orpaint](https://github.com/YMlinfeng/Orpaint).

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Experiments](#experiments)
- [Contributing](#contributing)
- [License](#license)

## Introduction
Orpaint is a groundbreaking model designed to restore damaged oracle bone inscription rubbings using a novel approach based on a pure visual state-space model within a U-net network. This method offers reduced complexity and improved scalability for high-resolution images, making it a significant advancement in the field of oracle bone studies.

## Features
- **Zero-shot Restoration**: Capable of restoring oracle bone inscriptions without requiring additional fine-tuning.
- **Linear Complexity**: Scales efficiently with image resolution, making it suitable for high-resolution images.
- **Transferability**: Effectively transferable to other image restoration tasks with excellent generalization performance.
- **Open Source**: The code is publicly available for further research and development.

## Installation
To install Orpaint, clone the repository and install the required dependencies:

```bash
git clone https://github.com/YMlinfeng/Orpaint.git
cd Orpaint
pip install -r requirements.txt
```

## Usage
To use Orpaint for restoring oracle bone inscriptions, follow the instructions in the `examples` directory. A basic usage example is provided below:

```python
import orpaint

# Load your damaged oracle bone image
image = orpaint.load_image('path_to_image')

# Restore the image
restored_image = orpaint.restore(image)

# Save the restored image
orpain.save_image(restored_image, 'path_to_save_restored_image')
```

## Experiments
Extensive experiments have been conducted to demonstrate the effectiveness of Orpaint. The experimental results can be found in the `experiments` directory, which includes detailed performance metrics and visual comparisons.

## Contributing
We welcome contributions from the community. If you would like to contribute to Orpaint, please follow these steps:
1. Fork the repository
2. Create a new branch (`git checkout -b feature_branch`)
3. Commit your changes (`git commit -am 'Add new feature'`)
4. Push to the branch (`git push origin feature_branch`)
5. Create a new Pull Request

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

For more information, please visit the [project page](https://github.com/YMlinfeng/Orpaint).
```
