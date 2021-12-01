# LearningToCountEverything-Colaboratory-Sample
<img src="https://user-images.githubusercontent.com/37477845/144256323-fa528429-bd20-4d75-957b-5e4f3610594e.gif" width="75%"><br>
[LearningToCountEverything](https://github.com/cvlab-stonybrook/LearningToCountEverything)をColaboratory上で動かすサンプルです。<br>

# How to use
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Kazuhito00/LearningToCountEverything-Colaboratory-Sample/blob/master/LearningToCountEverything-Colaboratory-Sample.ipynb)<br>
[Open In Colab]ボタンを押し、Colaboratoryでノートブックを開き、<br>
最初のセルから順に実行してください。<br><br>
試す画像を変更する際はimread_from_url()のURLを変更してください。<br>
```
# 画像読み込み
import cv2
from imread_from_url import imread_from_url

image_list = []
cv_image = imread_from_url('XXXX')
image_list.append(cv2.cvtColor(cv_image, cv2.COLOR_BGR2RGB))
```

また、以下のセルを実行すると簡易なアノテーションツールが起動します。<br>
カウント対象をマウスで指定し「Submit」を押してください。
```
# カウント対象指定
import colab_utils

bboxes = []
colab_utils.annotate(image_list, box_storage_pointer=bboxes)
```

# Reference
* [cvlab-stonybrook/LearningToCountEverything](https://github.com/cvlab-stonybrook/LearningToCountEverything)

# Author
高橋かずひと(https://twitter.com/KzhtTkhs)
 
# License 
LearningToCountEverything-Colaboratory-Sample is under [MIT License](LICENSE).

# License(Image)
金平糖の画像は[フリー素材ぱくたそ](https://www.pakutaso.com)様の写真を利用しています。
