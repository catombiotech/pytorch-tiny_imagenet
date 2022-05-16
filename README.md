# pytorch-tiny_imagenet
The 2nd homework for 'the basics of python and deep learning'

## File description
1. changed.py: 改动后的pytorch-main.py。
2. show_diff.ipynb: 找到两个checkpoint的不同以及与真实标记的对比。
3. commit.diff：git diff生成的文件，展示changed.py与pytorch-main.py的不同。
4. ./result 一些不同结果的图片。
5. check_1.npy, check_2.npy：两次checkpoint对验证集的预测结果，读取后均为长度为10000的np数组。

## Change description:
**按照commit.diff中的改动顺序！**
1. 根据改动添加了的调包，以及tensorboard记录writer。
2. 添加命令行参数`result_name`，方便我在evaluate更改输出npy的名字。
3. 减去图像变换中随机的翻转，防止欠拟合。
4. 利用更新后的验证集读取方式读取val_loader。
5. 原文件中不小心插入几个字母了（train_loader->train_loacondader）。
6. 
