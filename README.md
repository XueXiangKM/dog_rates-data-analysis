# dog_rates-data-analysis

对2000余条 @dog_rates 的推特数据进行清洗，提取其中的dog评分、dog名字等进行分析

## 数据集说明

> 1：WeRateDogs 的推特档案，包括推特ID、文本内容、发布时间等基础数据以及从文本中提取的dog评分、dog名字和dog stage等，该数据集存储在twitter-archive-enhanced.csv中

> 2: 推特图像的预测数据，即根据神经网络，对出现在每个推特中狗的品种（或其他物体、动物等）进行预测的结果，利用request库从https://raw.githubusercontent.com/udacity/new-dand-advanced-china/master/%E6%95%B0%E6%8D%AE%E6%B8%85%E6%B4%97/WeRateDogs%E9%A1%B9%E7%9B%AE/image-predictions.tsv
获取该数据集，并存储在image_predictions.tsv中

> 3: 每条推特的额外附加数据，包含转发数（retweet_count）和喜欢数（favorite_count）等，数据集为json格式，该数据集存储在tweet_json.txt中

## 数据评估及清洗

> 1: 对数据集进行评估，整理其中的质量问题及整洁度问题

> 2: 对所发现的整洁度问题进行清理，清理其中不需要的数据，并对数据进行合并，将数据合并为一个dataframe

> 3: 对所发现的质量问题进行清理，将数据类型转换为正确的类型，并利用正则表达式重新提取dog评分、dog名字和dog stage

> 4: 将清洗后的数据存储为twitter_archive_master.csv

## 数据分析

对dog评分、dog stage、图片预测可信度、转发数和点赞数的相关性等进行可视化分析
