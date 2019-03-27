# Chinese Machine Reading Comprehension Datasets

**Note that, this repository will be updated irregularly.**

## Statement
**If you find this repository helpful, please press the star button. Moreover, if you would like to use or repost the content in this repository, please indicate the orignal author and source link.**

## Chinese Reading Comprehension Datasets
Here I list several Chinese reading comprehension datasets that are PUBLICLY available (with appropriate technical report or paper). If I missed something, feel free to inform me. Unless indicated, the datasets are in simplified Chinese.

| Dataset  | Genre | Query Type | Answer Type |  Document # | Query # | Download |
| :------ | :-----: | :-----: | :-----: | :-----: | :-----: | :-----: |
| People Daily & Children's Fairy Tale [1] | news & tale | Cloze | word | 28K | 100K | [link](https://github.com/ymcui/Chinese-Cloze-RC) |
| WebQA [2] | Web | User log | entity | - | 42K | [link](http://paddlepaddle.bj.bcebos.com/dataset/webqa/WebQA.v1.0.zip) |
| CMRC 2017 [3] | news | Cloze & Query | word | - | 364K | [link](https://github.com/ymcui/cmrc2017) | 
| DuReader [4] | Web | User log | free form | 1M | 200K | [link](https://github.com/baidu/DuReader) |
| CMRC 2018 [5] | Wiki | Query | Span | - | 18K | [link](https://github.com/ymcui/cmrc2018) |
| DRCD [6]<sup>(tranditional Chinese)</sup> | Wiki | Query | Span | - | 34K | [link](https://github.com/DRCSolutionService/DRCD) |

> [1] (Cui et al., 2016) Consensus Attention-based Neural Networks for Chinese Reading Comprehension. In COLING 2016. https://aclanthology.info/papers/C16-1167/c16-1167

> [2] (Li et al., 2016) Dataset and Neural Recurrent Sequence Labeling Model for Open-Domain Factoid Question Answering. In arXiv. https://arxiv.org/abs/1607.06275

> [3] (Cui et al., 2018) Dataset for the First Evaluation on Chinese Machine Reading Comprehension. In LREC 2018. http://www.lrec-conf.org/proceedings/lrec2018/summaries/32.html

> [4] (He et al., 2018) DuReader: a Chinese Machine Reading Comprehension Dataset from Real-world Applications. In ACL 2018 MRQA Workshop. https://aclanthology.info/papers/W18-2605/w18-2605

> [5] (Cui et al., 2018) A Span-Extraction Dataset for Chinese Machine Reading Comprehension. In arXiv. https://arxiv.org/abs/1810.07366

> [6] (Shao et al., 2018) DRCD: a Chinese Machine Reading Comprehension Dataset. In arXiv. https://arxiv.org/abs/1806.00920


## Chinese Reading Comprehension Evaluation / Competition
Along with the release of these datasets, there are also several Chinese Reading Comprehension evaluation workshops or competitions which further accelerate the research on this topic.

 1. [The First Evaluation Workshop on Chinese Machine Reading Comprehension (CMRC 2017)](https://hfl-rc.github.io/cmrc2017/)
 2. [The Second Evaluation Workshop on Chinese Machine Reading Comprehension (CMRC 2018)](https://hfl-rc.github.io/cmrc2018/)
 3. [2018 NLP Challenge on Machine Reading Comprehension](http://mrc2018.cipsc.org.cn/)
 4. [The Third Evaluation Workshop on Chinese Machine Reading Comprehension (CMRC 2019)](https://hfl-rc.github.io/cmrc2019/)
 5. [2019 NLP Language and Intelligence Challenge](http://lic2019.ccf.org.cn)
 

## State-of-the-art Systems
Here I list several state-of-the-art systems (published / unpublished) for these datasets. There is a big chance that I missed something. So feel free to inform me new entries on `Issue` tab.

### People Daily & Children's Fairy Tale
| System  | PD-DEV | PD-TEST | CFT-TEST-AUTO | CFT-TEST-HUMAN | Note |
| :------ | :-----: | :-----: | :-----: | :-----: | :-----: | :-----: |
| [CAS Reader](https://aclanthology.info/papers/C16-1167/c16-1167) | 65.2 | 68.1 | 41.3 | 35.0 | - |
| [AS Reader](https://aclanthology.info/papers/C16-1167/c16-1167) | 64.1 | 67.2 | 40.9 | 33.1 | - | 


### CMRC 2017
Leaderboard: https://hfl-rc.github.io/cmrc2017/leaderboard/

#### Cloze Track 
| System  | DEV | TEST | Note |
| :------ | :-----: | :-----: | :-----: |
| 6ESTATES PTE LTD (ensemble) | 81.85 | 81.90 | - |
| SJTU BCMI-NLP (ensemble) | 78.35 | 80.67 | - | 
| YunSiChuangZhi (ensemble) | 79.20 | 80.27 | - | 

#### User Query Track
| System  | DEV | TEST | Note |
| :------ | :-----: | :-----: | :-----: |
| ECNU (ensemble) | 90.45 | 69.53 | - |
| SXU-3 (single model) | 47.80 | 49.07 | - | 
| ZZU (single model) | 31.10 | 32.53 | - | 

### DuReader
Leaderboard: http://ai.baidu.com/broad/leaderboard?dataset=dureader

| System  | ROUGE-L | BLEU-4 | Note |
| :------ | :-----: | :-----: | :-----: |
| AliReader | 63.48 | 61.54 | - |
| NI-Reader (ensemble) | 63.38 | 59.23 | - |
| mrc_try_mingyan (single model) | 62.20 | 59.72 | - |
| [Match-LSTM](https://aclanthology.info/papers/W18-2605/w18-2605) | 39.2 | 31.9 | - |
| [BiDAF](https://aclanthology.info/papers/W18-2605/w18-2605) | 39.0 | 31.8 | - |


### CMRC 2018
Leaderboard: https://hfl-rc.github.io/cmrc2018/open_challenge/

| System  | TEST-EM | TEST-F1 | CHALLENGE-EM | CHALLENGE-EM | Note |
| :------ | :-----: | :-----: | :-----: | :-----: | :-----: | :-----: |
| GM-Reader (ensemble) | 64.045 | 83.046 | 15.675 | 37.315 | - |
| MCA-Reader (ensemble) | 71.175 | 88.090 | 15.476 | 37.104 | - | 
| Z-Reader (single model) | 74.178 | 88.145 | 13.889 | 37.422 | - |

*More detailed results can be obtained in [CMRC 2018 Overview](https://arxiv.org/abs/1810.07366).


### DRCD

| System  | DEV-EM | DEV-F1 | TEST-EM | TEST-EM | Note |
| :------ | :-----: | :-----: | :-----: | :-----: | :-----: | :-----: |
| r-net (single model) | - | - | 29.1 | 44.4 | - |


## Contact
For any problems, please leave a message in the `Github Issues`.


## Disclaimer
Any subjective comments in this repository only represents the idea of the owner (ymcui), and does not represent the claims of any organizations.
