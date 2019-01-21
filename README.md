# Classify-flowers

训练：train.py
测试：eval.py



## 注意：

问：更换了图片，为什么**accuracy总是为0**的问题？怎么解决？
答：\detection_flowers\runs\1548061861，在你自己的目录下去找一个**label.txt**的文件
`0 -> tulips   1 -> roses     2 -> daisy     3 -> dandelion      4 -> sunflowers`
这个标签对应的就是你要测试的图片的标签，如果你选用的是roses，那么你的标签就为1。y_test = [1]，1是标签，意思就是测试的图片是这一类，也就是roses 。如果你的标签与你的图片不是对应的，那么就会出现一直是0的情况，意思就是测试错误。
