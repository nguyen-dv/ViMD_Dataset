# Multi-Dialect Vietnamese: Task, Dataset, Baseline Models and Challenges (Main EMNLP 2024)

## Introduction

This document presents the accompanying dataset for the paper titled **"Multi-Dialect Vietnamese: Task, Dataset, Baseline Models, and Challenges"**. The dataset, referred to as the **Vi**etnamese **M**ulti-**D**ialect (ViMD) dataset, is a comprehensive resource designed to capture the linguistic diversity represented by 63 provincial dialects spoken across Vietnam. The The paper is available at https://arxiv.org/pdf/2410.03458, and the dataset can be found at https://huggingface.co/datasets/nguyendv02/ViMD_Dataset.

## Citation

If you use this paper and its dataset in your research, please cite it as follows:

```bibtex
@misc{vandinh2024multidialectvietnamesetaskdataset,
      title={Multi-Dialect Vietnamese: Task, Dataset, Baseline Models and Challenges}, 
      author={Nguyen Van Dinh and Thanh Chi Dang and Luan Thanh Nguyen and Kiet Van Nguyen},
      year={2024},
      eprint={2410.03458},
      archivePrefix={arXiv},
      primaryClass={cs.CL},
      url={https://arxiv.org/abs/2410.03458}, 
}
```

## Overview of the Dataset

- **Source**: News programs from the broadcasting stations of the 63 provinces of Vietnam.
- **Overall Statistics**:

<p align="center">
  <img src="https://github.com/user-attachments/assets/1780741a-418a-4988-a2f3-3eb6d38fde0e" alt="Statistic" width="600"/>
</p>

- **Attributes**:

| Key        | Description                                                                |
|------------|----------------------------------------------------------------------------|
| set        | The set of audio: `{'train', 'valid', 'test'}`.                          |
| filename   | The filename follows the syntax `{province code}_{Sequence Number of Audio}`. |
| text       | Transcript of the audio.                                                  |
| length     | Length of the audio in seconds.                                          |
| province   | The provincial dialect code.                                              |
| region     | The regional dialect: `{'North', 'Central', 'South'}`.                  |
| speakerID  | The speaker identification code follows the syntax `spk_{province code}_{Sequence Number of Speaker}`. |
| gender     | Gender of the speaker (0 represents female and 1 represents male).        |

- For further details, please refer to the paper.
