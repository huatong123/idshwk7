原理：采用基于LSB的信息隐藏算法，将信息嵌入图片的最低比特位
所用工具：LSB-Steganography-master
实验过程：
1)准备好载体图像chapter12-1.png；创建写有ID和name的txt文件 wk7.txt
2)在终端输入命令：python LSBSteg.py encode -i chapter12-1.png -o test.png -f wk7.txt
  将wk7.txt中的信息隐藏到图片中，输出携密图片test.png
3)在终端输入命令：python LSBSteg.py decode -i test.png -o wk7decode.txt
  将图片中的信息提取并保存到wk7decode.txt中
