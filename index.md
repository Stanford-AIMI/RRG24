# Shared task on Large-Scale Radiology Report Generation

## 0. Paper submission

**In response to multiple requests, the leaderboard will remain open until the very end. Please ensure that the results in your overview paper match your submission on the online leaderboard.**

> System papers due date: May 17th (Friday), 2024

All papers will be submitted at:
> https://softconf.com/acl2024/BioNLP2024-ST

In the submission form, choose:
> Submission Categories: Please enter the categories under which the submission should be reviewed.
> Task (*):   
> ST_1A

Your paper should respect the format:
> TeamA at RRG24: Title
> 

Please read these instructions:

- We do not run a double blinded review. **Your paper must not be anonymous.**
- You can choose to submit a short (4 pages) or a long paper (8 pages).
- The shared task paper will undergo a "light" review process, focusing on aspects such as understandability, articulation, formatting, and overall style.
- Send a one-paragraph summary to jbdel [at] stanford dot edu about your best system, as well as your paper name, so it can be included in the overview paper.
- Make sure your paper contains the proper reference to:
- 
**1) The overview paper:**
```bibtex
@inproceedings{xu-etal-2024-overview,
    title = "Overview of the First Shared Task on Clinical Text Generation: RRG24 and {``}Discharge Me!{''}",
    author = "Xu, Justin  and
      Chen, Zhihong  and
      Johnston, Andrew  and
      Blankemeier, Louis  and
      Varma, Maya  and
      Langlotz, Curtis  and
      Delbrouck, Jean-Benoit",
    booktitle = "The 23rd Workshop on Biomedical Natural Language Processing and BioNLP Shared Tasks",
    month = aug,
    year = "2024",
    address = "Bangkok, Thailand",
    publisher = "Association for Computational Linguistics",
}
```
**2) The metrics:**
  - BLEU4
```bibtex
@inproceedings{papineni2002bleu,
  title={Bleu: a method for automatic evaluation of machine translation},
  author={Papineni, Kishore and Roukos, Salim and Ward, Todd and Zhu, Wei-Jing},
  booktitle={Proceedings of the 40th annual meeting of the Association for Computational Linguistics},
  pages={311--318},
  year={2002}
}
```
  - ROUGEL
```bibtex
@inproceedings{lin2004rouge,
  title={Rouge: A package for automatic evaluation of summaries},
  author={Lin, Chin-Yew},
  booktitle={Text summarization branches out},
  pages={74--81},
  year={2004}
}
```
  - Bertscore
```bibtex
@inproceedings{zhang2019bertscore,
  title={BERTScore: Evaluating Text Generation with BERT},
  author={Zhang, Tianyi and Kishore, Varsha and Wu, Felix and Weinberger, Kilian Q and Artzi, Yoav},
  booktitle={International Conference on Learning Representations},
  year={2019}
}
```
  - F1-cheXbert	
```bibtex
@inproceedings{smit2020combining,
  title={Combining Automatic Labelers and Expert Annotations for Accurate Radiology Report Labeling Using BERT},
  author={Smit, Akshay and Jain, Saahil and Rajpurkar, Pranav and Pareek, Anuj and Ng, Andrew Y and Lungren, Matthew},
  booktitle={Proceedings of the 2020 Conference on Empirical Methods in Natural Language Processing (EMNLP)},
  pages={1500--1519},
  year={2020}
}
```
  - F1-RadGraph	
```bibtex
@inproceedings{delbrouck2022improving,
  title={Improving the Factual Correctness of Radiology Report Generation with Semantic Rewards},
  author={Delbrouck, Jean-Benoit and Chambon, Pierre and Bluethgen, Christian and Tsai, Emily and Almusa, Omar and Langlotz, Curtis},
  booktitle={Findings of the Association for Computational Linguistics: EMNLP 2022},
  pages={4348--4360},
  year={2022}
}
```
**3) The datasets:**
  - Mimic-cxr
```bibtex
@article{johnson2019mimic,
  title={MIMIC-CXR, a de-identified publicly available database of chest radiographs with free-text reports},
  author={Johnson, Alistair EW and Pollard, Tom J and Berkowitz, Seth J and Greenbaum, Nathaniel R and Lungren, Matthew P and Deng, Chih-ying and Mark, Roger G and Horng, Steven},
  journal={Scientific data},
  volume={6},
  number={1},
  pages={317},
  year={2019},
  publisher={Nature Publishing Group UK London}
} 
```
  - Chexpert
```bibtex
@article{chambon2024chexpert,
  title={CheXpert Plus: Hundreds of Thousands of Aligned Radiology Texts, Images and Patients},
  author={Chambon, Pierre and Delbrouck, Jean-Benoit and Sounack, Thomas and Huang, Shih-Cheng and Chen, Zhihong and Varma, Maya and Truong, Steven QH and Chuong, Chu The and Langlotz, Curtis P.},
  year={2024}
}

```
  - Padchest
```bibtex
@article{bustos2020padchest,
  title={Padchest: A large chest x-ray image dataset with multi-label annotated reports},
  author={Bustos, Aurelia and Pertusa, Antonio and Salinas, Jose-Maria and De La Iglesia-Vaya, Maria},
  journal={Medical image analysis},
  volume={66},
  pages={101797},
  year={2020},
  publisher={Elsevier}
}
```
  - BIMCV COVID-19
```bibtex
@article{vaya2020bimcv,
  title={BIMCV COVID-19+: a large annotated dataset of RX and CT images from COVID-19 patients},
  author={Vay{\'a}, Maria De La Iglesia and Saborit, Jose Manuel and Montell, Joaquim Angel and Pertusa, Antonio and Bustos, Aurelia and Cazorla, Miguel and Galant, Joaquin and Barber, Xavier and Orozco-Beltr{\'a}n, Domingo and Garc{\'\i}a-Garc{\'\i}a, Francisco and others},
  journal={arXiv preprint arXiv:2006.01174},
  year={2020}
}
```
**4) The metric packages and the leaderboard that made this challenge possible were provided thanks to ViLMedic. Please include it in your submission:**
```bibtex
@inproceedings{delbrouck2022vilmedic,
  title={ViLMedic: a framework for research at the intersection of vision and language in medical AI},
  author={Delbrouck, Jean-benoit and Saab, Khaled and Varma, Maya and Eyuboglu, Sabri and Chambon, Pierre and Dunnmon, Jared and Zambrano, Juan and Chaudhari, Akshay and Langlotz, Curtis},
  booktitle={Proceedings of the 60th Annual Meeting of the Association for Computational Linguistics: System Demonstrations},
  pages={23--34},
  year={2022}
}
```
<hr/>



> <b>Submission are now open at [https://vilmedic.app/misc/bionlp24/leaderboard](https://vilmedic.app/misc/bionlp24/leaderboard)</b>
> <b>Submission are now open at [https://vilmedic.app/misc/bionlp24/leaderboard](https://vilmedic.app/misc/bionlp24/leaderboard)</b>
> <b>Submission are now open at [https://vilmedic.app/misc/bionlp24/leaderboard](https://vilmedic.app/misc/bionlp24/leaderboard)</b>

An important medical application of natural language generation (NLG) is to build assistive systems that take X-ray
images of a patient and generate a textual report describing clinical observations in the images. This is a clinically
important task, offering the potential to reduce radiologists’ repetitive work and generally improve clinical
communication.

## 1. Task Overview

Given one or multiple chest X-rays from one study, the participants must generate the corresponding radiology report.
In the scope of this task, two sections are considered: findings and impressions. Each section will have its own separate
evaluation and leaderboard. These sections may be produced using either a single system or two distinct systems.

### 1.1 Rules

> All participants will be invited to submit a paper describing their solution to be included in
>
the [Proceedings of the 23rd Workshop on Biomedical Natural Language Processing (BioNLP) at ACL 2024](https://aclanthology.org/venues/bionlp/).
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
- <span style="color: red;">Using the information in the official MIMIC-CXR and CheXpert validation and test sets is *
  <b>strictly prohibited</b>, including their labels and reports.</span>

## 1.2 Timeline

- **Release of the training and validation datasets:** February 22nd (Tuesday), 2024
- **Release of the public and hidden test dataset:** April 19th (Friday), 2024
- **System submission deadline:** May 15th (Wednesday), 2024
- **System papers due date:** May 17th (Friday), 2024
- **Notification of acceptance:** June 17th (Monday), 2024
- **Camera-ready system papers due:** July 1st (Monday), 2024
- **BioNLP Workshop Date:** August 16th (Friday), 2024

All deadlines are 11:59 PM ("Anywhere on Earth").

## 2. Data

Below are the data used for the challenge. Please note:

- The training and validation sets are grouped by study, but **not** grouped by subjects.
- The studies in the test sets will be unseen studies.
- The official language of PadChest and BIMCV-COVID19 is Spanish, where their reports have been translated using GPT-4.
- <span style="color: red;">Using the information in the official MIMIC-CXR and CheXpert validation and test sets is *
  <b>strictly prohibited</b>, including their labels and reports.</span>

### 2.1 Training

| Dataset       | Findings Count | Impressions Count |
|---------------|----------------|-------------------|
| PadChest      | 101,752        | -                 |
| BIMCV-COVID19 | 45,525         | -                 |
| CheXpert      | 45,491         | 181,619           |
| OpenI         | 3,252          | 3,628             |
| MIMIC-CXR     | 148,374        | 181,166           |
| **Total**     | **344,394**    | **366,413**       |

### 2.2 Validation

| Dataset       | Findings Count | Impressions Count |
|---------------|----------------|-------------------|
| CheXpert      | 1,112          | 4,589             |
| BIMCV-COVID19 | 1,202          | -                 |
| PadChest      | 2,641          | -                 |
| OpenI         | 85             | 92                |
| MIMIC-CXR     | 3,799          | 4,650             |
| **Total**     | **8,839**      | **9,331**         |

### 2.3 Test

Please see [https://huggingface.co/datasets/StanfordAIMI/interpret-cxr-public/discussions](https://huggingface.co/datasets/StanfordAIMI/interpret-cxr-public/discussions)

### 2.4 Access

Here are the steps to access the dataset of this challenge with the correct splits:

1) The datasets (image and findings/impression pairs) of CheXpert, BIMCV-COVID19 (en), PadChest (en) and OpenI can be
   access through
   the <img src="https://huggingface.co/front/assets/huggingface_logo-noborder.svg" width="15"> huggingface dataset at
   the
   following
   url: [https://huggingface.co/datasets/StanfordAIMI/interpret-cxr-public](https://huggingface.co/datasets/StanfordAIMI/interpret-cxr-public).
   Once you have been granted access, you can invoke the dataset using the following:

```python
from datasets import load_dataset

dataset = load_dataset("StanfordAIMI/interpret-cxr-public")
```

2) You'll have to handle the MIMIC-CXR processing on your own by
   utilizing the [make-interpret-mimic-cxr.py](https://storage.googleapis.com/vilmedic_dataset/RRG24/make-interpret-mimic-cxr.py)
   script.
   It's crucial to use this script as it ensures the proper splits are defined. Please have the following structure
   ready (files folder is from [mimic-cxr-jpg](https://physionet.org/content/mimic-cxr-jpg/2.0.0/)):

```bash
.
├── files
│   ├── p10
│   ├── p11
│   ├── ...
│   └── p19
├── make-interpret-mimic-cxr.py
├── mimic-cxr-2.0.0-metadata.csv
├── mimic-cxr-2.0.0-split.csv
└── mimic_cxr_sectioned.csv
```

And run `python make-interpret-mimic-cxr.py`. If you have a hash error (i.e. 
the created files arent what was expected), please email me at jbdel at stanford dot edu.<br/>

Then, you can then collate both datasets as such:

```python
from datasets import load_dataset, Sequence, Image, DatasetDict, concatenate_datasets

dataset = load_dataset("StanfordAIMI/interpret-cxr-public")
dataset_mimic = load_dataset(
    "json",
    data_files={"train": "train_mimic.json", "validation": "val_mimic.json"},
).cast_column("images", Sequence(Image()))
dataset_final = DatasetDict({"train": concatenate_datasets([dataset["train"], dataset_mimic["train"]]),
                             "validation": concatenate_datasets([dataset["validation"], dataset_mimic["validation"]])})
dataset_final.save_to_disk("path/to/dataset/directory")
```
Please note that the save_to_dict operation can take time:<br/>
`
Saving the dataset (147/147 shards): 100%|██████████| 550395/550395 [7:28:42<00:00, 20.44 examples/s]
`

The final dataset should be as detailed below:

```bash
DatasetDict({
    train: Dataset({
        features: ['source', 'findings', 'images', 'impression', 'images_path'],
        num_rows: 550395
    })
    validation: Dataset({
        features: ['source', 'findings', 'images', 'impression', 'images_path'],
        num_rows: 14111
    })
})
```

3) One more dataset, VinDr-CXR, can be used as training data if you wish, but we do not process on our end. You will
   need to do it
   yourself at [https://vindr.ai/datasets/cxr](https://vindr.ai/datasets/cxr).

### 3. Metrics

The submissions will be automatically evaluated with the following metrics:

- [Bertscore](https://github.com/jbdel/vilmedic/blob/main/vilmedic/blocks/scorers/NLG/bertscore/bertscore.py) [1]
- BLEU [2]
- ROUGEL [3]
- [F1-RadGraph](https://github.com/jbdel/vilmedic/blob/main/vilmedic/blocks/scorers/scores.py#L103) ([pypi package](https://pypi.org/project/radgraph/)) [4]
- [F1-CheXbert](https://github.com/jbdel/vilmedic/blob/main/vilmedic/blocks/scorers/scores.py#L90) ([pypi package](https://pypi.org/project/f1chexbert/))

Also, the top participants will be evaluated against CheXagent [5].

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

