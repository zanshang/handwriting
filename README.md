# 手写字母识别挑战

![Image of digits](https://github.com/zanshang/handwriting/raw/master/example_digits.png)

数据文件里有一个train.csv文件，这个文件里包含了一系列的灰度图片，图片上有一些手写数字，数字范围是从0到9

每一张图片都是28像素高28像素宽，总共784个像素，每一个像素都用一个数值来代表，越小的数字代表颜色越浅，越大的数字代表颜色越深，数字的范围是0到255.

在训练数据里(train.csv)，每一条数据都有785列，第一列称作“label”，表示余下的数据所组成的图所代表的数字

在余下的784列里，列名从 "label0" 一直到 "label783"，表示数据的方式是先填满一行28像素，再开始填第二行的28个像素，用可视化的表示就是如下：

```
000 001 002 003 ... 026 027
028 029 030 031 ... 054 055
056 057 058 059 ... 082 083
 |   |   |   |  ...  |   |
728 729 730 731 ... 754 755
756 757 758 759 ... 782 783 
```

在最终的评测数据里(test.csv)，数据格式和上面表示的数据是一样的，只是没有label这一列

最终提交的数据需要是一个csv文件，它总共是两列，若干行（行数和评测数据一致），其中第一列数据需要填入在评测数据里的数据序号，第二列需要填入预测的数值。用可视化的表示如下：

```
ImageId,Label
1,3
2,7
3,8 
(27997 more lines)
```

最终成绩为 预测正确数/总数据量 * 100 ，比如总共5000条数据，其中正确预测1000条，那最终成绩就为 20

[训练用数据，以及最终提交文件样例](https://pan.baidu.com/s/1qY2FFqO)

达标成绩80分

奖金池：2000元/月