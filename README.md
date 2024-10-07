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
  <img src="https://github.com/user-attachments/assets/10697af3-6414-49d4-9c6f-a1be4df16929" alt="Statistic" width="800"/>
</p>


- **Attributes**:

<table border="1" style="border-collapse: collapse; width: 100%; text-align: left;">
  <tr>
    <th style="background-color: #f2f2f2; text-align: center;">Key</th>
    <th style="background-color: #f2f2f2; text-align: center;">Description</th>
  </tr>
  <tr>
    <td style="background-color: #f2f2f2; text-align: center;">set</td>
    <td>The set of audio: `{'train', 'valid', 'test'}`.</td>
  </tr>
  <tr>
    <td style="background-color: #f2f2f2; text-align: center;">filename</td>
    <td>The filename follows the syntax `{province code}_{Sequence Number of Audio}`.</td>
  </tr>
  <tr>
    <td style="background-color: #f2f2f2; text-align: center;">text</td>
    <td>Transcript of the audio.</td>
  </tr>
  <tr>
    <td style="background-color: #f2f2f2; text-align: center;">length</td>
    <td>Length of the audio in seconds.</td>
  </tr>
  <tr>
    <td style="background-color: #f2f2f2; text-align: center;">province</td>
    <td>The provincial dialect code.</td>
  </tr>
  <tr>
    <td style="background-color: #f2f2f2; text-align: center;">region</td>
    <td>The regional dialect: `{'North', 'Central', 'South'}`.</td>
  </tr>
  <tr>
    <td style="background-color: #f2f2f2; text-align: center;">speakerID</td>
    <td>The speaker identification code follows the syntax `spk_{province code}_{Sequence Number of Speaker}`.</td>
  </tr>
  <tr>
    <td style="background-color: #f2f2f2; text-align: center;">gender</td>
    <td>Gender of the speaker (0 represents female and 1 represents male).</td>
  </tr>
</table>


- For further statistics, please refer to the paper.
