---
layout: default
---

# Shared task on Large-Scale Radiology Report Generation

An important medical application of natural language generation (NLG) is to build assistive systems that take X-ray
images of a patient and generate a textual report describing clinical observations in the images. This is a clinically
important task, offering the potential to reduce radiologists’ repetitive work and generally improve clinical
communication.

## 1. Task Overview

Given one or multiple chest x-rays from one study, the participants must generate the corresponding radiology report.

In the scope of this task, two sections are considered: findings and impression. Each section will have their own separate evaluation and leaderboard. These sections may be produced using either a single system or two distinct systems.

### 1.1 Rules

> All participants will be invited to submit a paper describing their solution to be included in
> the [Proceedings of the 23rd Workshop on Biomedical Natural Language Processing (BioNLP) at ACL 2024](https://aclanthology.org/venues/bionlp/).
> If you do not wish to write a paper, you must at least provide a thorough description of your system which will be
> included in the overview paper for this task. Otherwise, your submission (and reported scores) will not be taken into
> account.

- Participants must agree to sign and follow the data access agreements for the provided dataset.
- Participants may use private data to train (or pre-train) their systems, make a submission, and write a technical
  paper describing their solution. However, their score will not be counted towards the general leaderboard. In order to
  validate your leaderboard ranking, all the data used for the submission must be in some way available to other
  researchers.
- If participants employ LLMs, generated data and the prompting strategies must be provided and described clearly so
  that results can be reproduced.

## 1.2 Timeline

- **Release of the training and validation datasets:** February 22nd (Tuesday), 2024
- **Release of the public and hidden test dataset:** April 12th (Friday), 2024
- **System submission deadline:** May 10th (Friday), 2024
- **System papers due date:** May 17th (Friday), 2024
- **Notification of acceptance:** June 17th (Monday), 2024
- **Camera-ready system papers due:** July 1st (Monday), 2024
- **BioNLP Workshop Date:** August 16th (Friday), 2024

All deadlines are 11:59 PM ("Anywhere on Earth").

## 2. Data

Below are the data used for the challenge. Please note:

- The training and validation set are not grouped by study.
- The studies in the test sets will be unseen studies.
- The official language of PadChest and BIMCV-COVID19 is Spanish, where their reports have been translated using GPT-4.
- Using the information in the official MIMIC-CXR and CheXpert validation and test sets is **strictly prohibited**,
  including their labels and reports.

### 2.1 Training

| Category   | MIMIC-CXR | CheXpert | BIMCV-COVID19 (en) | CANDID-PTX | PadChest (en) | OpenI | Total   |
|------------|-----------|----------|--------------------|------------|---------------|-------|---------|
| Findings   | 148,253   | 45,495   | 45,580             | -          | 101,835       | 3,261 | 344,424 |
| Impression | 178,073   | 181,524  | -                  | 17,767     | -             | 3,631 | 380,995 |

### 2.2 Validation

| Category   | MIMIC-CXR | CheXpert | BIMCV-COVID19 (en) | CANDID-PTX | PadChest (en) | OpenI | Total |
|------------|-----------|----------|--------------------|------------|---------------|-------|-------|
| Findings   | 3,874     | 1,108    | 1,147              | -          | 2,558         | 76    | 8,763 |
| Impression | 4,600     | 4,684    | -                  | 464        | -             | 89    | 9,837 |

### 2.3 Test

The ground-truth of the test-set will be provided at the end of the challenge.

### 2.4 Access

The full dataset (image and report pairs) can be access through 
the <img src="https://huggingface.co/front/assets/huggingface_logo-noborder.svg" width="15"> huggingface dataset at the following url: [https://huggingface.co/datasets/StanfordAIMI/interpret-cxr](https://huggingface.co/datasets/StanfordAIMI/interpret-cxr).

### 3. Metrics

Participants submission will be automatically evaluated with the following metric:

- Bertscore [1]
- BLEU [2]
- ROUGEL [3]
- F1-RadGraph ([pypi package](https://pypi.org/project/radgraph/)) [4]
- F1-CheXbert-XL

Also top participant will be evaluated against CheXagent [5].

# Organizers

<table style="border-collapse: collapse; border: none;">
  <tr>
    <td style="border: none;" align="center">
      <img src="https://aimi.stanford.edu/sites/g/files/sbiybj20451/files/styles/medium_square/public/media/image/image5_0.png?h=f4e62a0a&itok=euaj9VoF" alt="JB Delbrouck" style="border-radius: 50%; width: 160px;"><br>
      <a href="https://jbdel.github.io/">Jean-Benoit Delbrouck</a>
    </td>
    <td style="border: none;" align="center">
      <img src="https://pbs.twimg.com/profile_images/1732290523657076736/fixg-DOd_400x400.jpg" alt="Zhihong Chen" style="border-radius: 50%; width: 160px;"><br>
      <a href="https://zhjohnchan.github.io/">Zhihong Chen</a>
    </td>
    <td style="border: none;" align="center">
      <img src="https://maya-varma.com/maya3.png" alt="Maya Varma" style="border-radius: 50%; width: 160px;"><br>
      <a href="https://maya-varma.com/">Maya Varma</a>
    </td>
    <td style="border: none;" align="center">
      <img src="https://aimi.stanford.edu/sites/g/files/sbiybj20451/files/styles/medium_square/public/media/image/curtis-langlotz_profilephoto_0.jpeg?h=b4e301e9&itok=AqV0_THq" alt="Curtis Langlotz" style="border-radius: 50%; width: 160px;"><br>
      <a href="https://profiles.stanford.edu/curtis-langlotz">Curtis Langlotz</a>
    </td>
  </tr>
</table>

# References

[1]

```bib
@inproceedings{zhang2019bertscore,
  title={BERTScore: Evaluating Text Generation with BERT},
  author={Zhang, Tianyi and Kishore, Varsha and Wu, Felix and Weinberger, Kilian Q and Artzi, Yoav},
  booktitle={International Conference on Learning Representations},
  year={2019}
}
```

[2]

```bib
@inproceedings{papineni2002bleu,
  title={Bleu: a method for automatic evaluation of machine translation},
  author={Papineni, Kishore and Roukos, Salim and Ward, Todd and Zhu, Wei-Jing},
  booktitle={Proceedings of the 40th annual meeting of the Association for Computational Linguistics},
  pages={311--318},
  year={2002}
}
```

[3]

```bib
@inproceedings{lin2004rouge,
  title={Rouge: A package for automatic evaluation of summaries},
  author={Lin, Chin-Yew},
  booktitle={Text summarization branches out},
  pages={74--81},
  year={2004}
}
```

[4]

```bib
@inproceedings{delbrouck2022improving,
  title={Improving the Factual Correctness of Radiology Report Generation with Semantic Rewards},
  author={Delbrouck, Jean-Benoit and Chambon, Pierre and Bluethgen, Christian and Tsai, Emily and Almusa, Omar and Langlotz, Curtis},
  booktitle={Findings of the Association for Computational Linguistics: EMNLP 2022},
  pages={4348--4360},
  year={2022}
}
```

[5]

```bib
@article{chen2024chexagent,
  title={CheXagent: Towards a Foundation Model for Chest X-Ray Interpretation},
  author={Chen, Zhihong and Varma, Maya and Delbrouck, Jean-Benoit and Paschali, Magdalini and Blankemeier, Louis and Van Veen, Dave and Valanarasu, Jeya Maria Jose and Youssef, Alaa and Cohen, Joseph Paul and Reis, Eduardo Pontes and others},
  journal={arXiv preprint arXiv:2401.12208},
  year={2024}
}
```
