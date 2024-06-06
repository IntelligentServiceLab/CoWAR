# CoWAR：A General Complementary Web API Recommendation Framework based on Learning Model

==Note==: Because **api_representation_dict.pkl** is too large and necessary, click [here](https://pan.baidu.com/s/1ylqvs-xeQynHvq_4njE_7Q?pwd=cqq7) for the full code.



## Introduction

CoWAR is designed to recommend complementary Web APIs tailored for Mashup creation, based on the user’s selected Web APIs.



## Environment Requirement

The experiment was run in the python 3.10.0 environment, and the required packages are as follows：

- wheel == 0.37.1
- transformers == 4.31.0
- torch == 2.0.1
- numpy == 1.24.3
- nlp == 0.4.0
- pandas == 2.0.3
- scikit-learn == 1.2.2
- matplotlib == 3.7.1
- scipy == 1.11.1
- tokenizers == 0.13.3
- seaborn == 0.12.2



## Example to run CoWAR

1. Run  **convert_to_input.py** first to get the input data
2. Then run **master_method.py**



## File Introduction

- data

  - api_representation_dict.pkl

    > The API representation used in the paper can be generated and replaced in api_representation.py, but this file is recommended

  - apisData.xlsx

    > Crawled API dataset

  - mashups.xlsx

    > Crawled Mashup dataset

- data_preprocessing

  - preprocessing.py

    > A file that preprocesses the original dataset to filter out data that does not meet the requirements

- deepctr

  > Code for placing BasicFM, DeepFM, AFM, NAFM models

- drawing

  - long_tail_picture.py

    > A file that draws a long-tail graph based on the original dataset

- experiments

  - master_method.py

    > This file is used to perform the experiment

  - sanfm.py

    > Code for placing SANFM model

- sample_generation

  - api_representation.py

    > Files that save API representations

  - bert2vec.py

    > A file that generates representations of the APIs based on BERT model

  - convert_to_input.py

    > labeled dataset and the representation of APIs are transformed into input data for the learning model and saved

  - data_labeling.py

    > In this file, a labeled dataset is generated according to the proposed data labeling algorithm and based on Mashup-API interactions derived from historical Mashups and Web APIs



## Contact

Email：1302466947@qq.com / qiqichen0702@gmail.com (Qiqi Chen)

