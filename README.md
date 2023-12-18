# ODD-diLLMma: Leveraging LLMs for Test Suite Analysis and Comparison with Debugging Support

This repository has the code and supplemental materials for our research paper focused on enhancing the validation of Advanced Driver Assistance Systems (ADAS) and Autonomous Driving Systems (ADS). Our work critically examines the limitations of current systems, particularly their reliance on Operational Design Domains (ODD) defined in natural language, which often leads to validation challenges like false positives and unseen failures. Central to our approach is the innovative use of Large Language Models (LLMs) for analyzing and aligning real-world data sets with the ODD specifications of ADAS/ADS systems. Our contributions include identifying LLMs as a key technology for bridging the gap between ODD specification and data, defining the ODD-diLLMma framework for leveraging LLMs in test suite analysis, and implementing a study using state-of-the-art LLMs on openpilot. 

## Repository Structure

This repository is organized into several folders, each serving a specific purpose in our study. Below is a table detailing each folder, its contents, and a link to the corresponding ReadMe for more in-depth information.

| Folder Name       | Description | ReadMe Link |
|-------------------|-------------|-------------|
| `0_Datasets`      | Contains the datasets used in our study. This includes three datasets (Open Pilot 2k19, Open Pilot Comma AI, JUtah) with steering data from openpilot, identified passing and failing scenarios, and descriptions of these scenarios using three LLMs (Vicuna, Llama, ChatGPT) and human analysis. | [ReadMe](./0_Datasets/README.md) |
| `1_ProcessData`   | Houses the code to convert the original datasets into formats compatible with openpilot. It also includes scripts for identifying passing and failing tests based on openpilot's steering angles and selecting tests based on the identified scenarios. | [ReadMe](./1_ProcessData/README.md) |
| `2_GenerateCaption`| Contains the code for generating captions using three LLMs (Vicuna, Llama, ChatGPT) and establishing a human baseline for comparison. | [ReadMe](./2_GenerateCaption/README.md) |
| `3_GenerateResults`| Includes the code for parsing the results and generating the data presented in the study. This folder is integral for understanding the study's outcomes and conclusions. | [ReadMe](./3_GenerateResults/README.md) |
| `Misc`| This include the data for both running the Vicuna and Llama models, as well as setting up OpenPilot | [ReadMe](./Misc/README.md) |

Please refer to the individual ReadMe files in each folder for detailed information about the contents and their usage.