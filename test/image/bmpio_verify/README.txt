为了提高扫描速度，Bitmap图像格式将像素数据分为多个scan-line，
每个scan-line包含了一行像素数据，并且对不能被4-byte整除的像素行填充0，
因此一个完整的Bitmap-Reader应该能够正确处理图片宽度模4的所有情况，
也即mod_0、mod_1、mod_2、mod_3共四个文件夹下的所有图片。
此外，每个文件夹还包含了对应宽度下的1位、4位、8位、16位、24位、32位
色彩空间的测试图片各一张，可以用来进一步测试bmp解码程序的包容性。