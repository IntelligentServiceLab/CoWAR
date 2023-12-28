# CWARM

### 一、data文件夹下的文件说明

1. 文件说明
   - apiData.xlsx：爬取的所有api数据，且为已处理过可直接使用的数据集
   - mashups.csv：爬取的所有mashup数据，且为已进行过预处理的数据集，所以样本数只有2230
   - combination.csv：在mashups.csv基础上得出的data labeling数据集
   - dict_api.pkl：基于apiData.xlsx以及BERT模型得出的数据，但是只是选取了在mashups.csv中使用过的数据。
   - dict_combination.pkl：基于combination.csv所得数据集
2. 注意事项
   - dict_api.pkl和dict_combination.pkl这些文件的键值对是经过处理的，也就是说将原本的名称由编号进行替代。所以在dict_combination中的键对应的是每个data labeling的编号，值对应的是其所包含api的编号，其中最后一个是推荐api编号。
   - dict_api.pkl中的键对应的api的编号，值对应的是基于BERT得到的768维的特征向量。

### 二、py文件说明

1. 文件说明

   - baselines.py：实验中的基线方法运行文件
   - bert2vec.py：BERT模型运行文件
   - CWARW.py：CWARW推荐模型运行文件
   - SANFM.py：SANFM学习模型文件

2. 注意事项

   运行环境为：python3.x（实验环境为3.10，一般情况下python3.x应该都是可以的）



### Contact

Email: [1302466947@qq.com](mailto:1302466947@qq.com) (陈琪琪)