# Annotation tool for binary classification data
Note
We add a new button in the tool, that is, "-1" means the annotator is not sure the label, or the image is unclear to convey the specific label.
## Environment

```
python3
```

```
PyQt5
```


## Install

```
git clone https://github.com/statusrank/annotation-tool-for-binary-classification-data
```

```
pip install -r requirements.txt
```

## Data

```
put the image folder at the same path of main.py
```

## Quick Start

```
python main.py
```

## Instructions

```
1. python3 + PyQt5
```
```
2. 将数据文件夹放置于main.py同路径下(解压后)
```
```
3. python main.py
```
```
4. 浏览并选择文件夹，开始标注，对于无爆炸图像，可以直接点击"保存并显示下一张"；
对于有爆炸图像，请先点击"标记为1：有爆炸"，再点击"保存并显示下一张"。
如果图像不够清晰，或者 有火光，又无法判断出是否为爆炸、还是灯光烟火等其他现象，可以标为"not sure -1", 再点击"保存并显示下一张"。
```
```
5. 如果标注错误但未进入下一张图像，点击"重新标注当前图像"，并重复步骤4即可；
如果标注错误且已经显示下一张图像，请点击"返回上一张"，可多次点击返回到需要的位置，重新重复步骤4。
```
```
6. 如果完成了一个文件夹下所有图像的标注，程序将自动保存结果到文件并输出提示；
【中途离开】如果对一个文件夹下内容未完成标注且有事必须关闭程序，请先点击"保存已标注结果到文件"，再关闭程序，否则结果不会被保存；
【继续标注】重新选择已标注过的文件夹，将读取对应的已有标注文件，并继续标注。
7. 标注完成后，将和main.py同目录下的对应的".txt"文件返回给我即可。
```

## Demo
```
由于本人水平有限，所以为了防止bug，导致大家浪费时间，额外提供一个test.zip文件夹，里面包含20+图片，用于测试。
请大家务必用此文件夹熟悉相关的标注步骤，并确保标注过程可以保存，再开始标注！谢谢
```
