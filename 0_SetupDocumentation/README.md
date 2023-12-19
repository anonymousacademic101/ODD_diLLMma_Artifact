# Setup Documentation

This section contains essential setup instructions for the tools used in our study: openpilot and MiniGPT4. Each folder (`OpenPilot_Setup` and `MiniGPT4_Setup`) includes detailed READMEs to guide you through the setup process.

## Openpilot Setup
- **Purpose:** [Openpilot](https://github.com/commaai/openpilot), our base Driving Automation System openpilot, was given data the `0_Datasets` folder. The steering angle produced was then used to identify both passing and failing inputs.
- **Setup Instructions:** For detailed setup steps, please refer to the README in the `OpenPilot_Setup` folder.

Here is an example of openpilot whose setup is described in `2023_03` running on data from the comma.ai 2k19 dataset.

![openpilot running on the data from 2023_03](../Misc/2023_03.gif)

## MiniGPT4 Setup
- **Overview:** We used [MiniGPT4](https://github.com/Vision-CAIR/MiniGPT-4), commit X. MiniGPT4 integrates a vision encoder with a pretrained ViT, Q-Former, and advanced Vicuna and Llama 2 language models.
- **Custom Usage:** Our study utilized custom code to process large datasets through MiniGPT4 without the GUI. This code is provided for efficiency and scalability.
- **Setup Instructions:** Follow the standard setup guidelines in the MiniGPT4 README and consult our custom instructions for dataset processing in the `MiniGPT4` folder.

(insert image)

## Suggested Hardware Requirements

### MiniGPT 4

MiniGPT 4 was run on a [System 76 Thelio Mega](https://system76.com/desktops/thelio-mega) desktop with Ubuntu 20.04 using Nvidia Driver version (insert)

The desktop has:
* X
* X
* X

### Openpilot

Openpilot was run a [MSI GE75 Raider 10SE](https://www.msi.com/Laptop/GE75-Raider-10SE/Specification) laptop with a freshly installed version of Ubuntu 20.04 using the default Nvidia Drivers.

The laptop has:
* 10th Generation i7 - 10750H 
* 16GB Ram
* NVIDIA GeForce RTX™ 2060 with 6GB GDDR6
