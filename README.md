# some-bug

### nomalize引发的bug
nomalize库设置html line-hight：1.15，这个属性被自动继承了，我们的font-size是12px，12*1.15 = 13.8；本身去除文字高度之后呢，剩余高度文字上分一半，下分一半；本身浏览器分了之后上边0.8，下边1，但是浏览器会对小数做类似math.floor的操作，上边就变为0，导致文字上移