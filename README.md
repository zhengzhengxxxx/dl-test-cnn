CNN图片分类测试项目：

1.首先执行create_processed_data
此文件遍历mingren文件夹下的全部名人照片,将这些照片转换为[向量=>标签]的npy文件,此文件用于后期的模型训练

2.执行training.py
此脚本自动将150张图片划分出训练集，测试机，验证集，在执行300轮训练以后，最终得到了92.3%的泛化误差
(运行此脚本，会在文件夹下产生save_model的文件，用于以后直接读取这些参数模型)


(由于github限制不允许上传100m以上的文件，谷歌预训练的inception_v3.ckpt文件需自行下载,并放到项目根目录下
地址：http://www.download.tensorflow.org/models/inception_v3_2016_08_28.tar.gz
)
