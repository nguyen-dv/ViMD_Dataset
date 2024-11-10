# Multi-Dialect Vietnamese: Task, Dataset, Baseline Models and Challenges (Main EMNLP 2024)

## Introduction

This document presents the accompanying dataset for the paper titled **"Multi-Dialect Vietnamese: Task, Dataset, Baseline Models, and Challenges"**. The dataset, referred to as the **Vi**etnamese **M**ulti-**D**ialect (ViMD) dataset, is a comprehensive resource designed to capture the linguistic diversity represented by 63 provincial dialects spoken across Vietnam. The The paper is available at https://arxiv.org/pdf/2410.03458, and the dataset can be found at https://huggingface.co/datasets/nguyendv02/ViMD_Dataset.

## Citation

If you use this paper and its dataset in your research, please cite it as follows:

```bibtex
@inproceedings{dinh-etal-2024-multi,
    title = "Multi-Dialect {V}ietnamese: Task, Dataset, Baseline Models and Challenges",
    author = "Dinh, Nguyen  and
      Dang, Thanh  and
      Thanh Nguyen, Luan  and
      Nguyen, Kiet",
    editor = "Al-Onaizan, Yaser  and
      Bansal, Mohit  and
      Chen, Yun-Nung",
    booktitle = "Proceedings of the 2024 Conference on Empirical Methods in Natural Language Processing",
    month = nov,
    year = "2024",
    address = "Miami, Florida, USA",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2024.emnlp-main.426",
    pages = "7476--7498",
    abstract = "Vietnamese, a low-resource language, is typically categorized into three primary dialect groups that belong to Northern, Central, and Southern Vietnam. However, each province within these regions exhibits its own distinct pronunciation variations. Despite the existence of various speech recognition datasets, none of them has provided a fine-grained classification of the 63 dialects specific to individual provinces of Vietnam. To address this gap, we introduce Vietnamese Multi-Dialect (ViMD) dataset, a novel comprehensive dataset capturing the rich diversity of 63 provincial dialects spoken across Vietnam. Our dataset comprises 102.56 hours of audio, consisting of approximately 19,000 utterances, and the associated transcripts contain over 1.2 million words. To provide benchmarks and simultaneously demonstrate the challenges of our dataset, we fine-tune state-of-the-art pre-trained models for two downstream tasks: (1) Dialect identification and (2) Speech recognition. The empirical results suggest two implications including the influence of geographical factors on dialects, and the constraints of current approaches in speech recognition tasks involving multi-dialect speech data. Our dataset is available for research purposes.",
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
