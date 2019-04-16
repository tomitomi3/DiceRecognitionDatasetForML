# Dice Recognition Datasets for Machine Learning
# サイコロの目認識のための教師用画像データセット

![dicepic](https://raw.githubusercontent.com/tomitomi3/DiceRecognitionDatasetForML/master/_img/pic_dice.jpg)

# Introduction
[MNIST](https://en.wikipedia.org/wiki/MNIST_database)(LeCun 1998) is a digital handwritten image dataset. This is a very famous image dataset used for benchmarking machine learning. We have created a new image dataset that can be used to practice machine learning for classification such as MNIST. It is an image data set of dice that everyone knows. Image datasets are created and annotated using [Dice Recognition System](https://github.com/tomitomi3/DiceRecognizeSystem).

画像認識（分類）のための教師用画像データセットとして手書き数字の[MNIST](https://en.wikipedia.org/wiki/MNIST_database)が有名です。ちょっと変わったサイコロの目の画像データセットを準備しました。サイコロの目の認識などにいかがでしょうか？ご自由にお使いください。[このシステム](https://github.com/tomitomi3/DiceRecognizeSystem)でサイコロの目を認識し、画像データセットを作成しました。

# Detail of Face of Dice image dataset

* Dataset Download

[Download](https://github.com/tomitomi3/DiceRecognitionDatasetForML/raw/master/dataset/DiceDataset.zip)

* Dice

We used two different size and color of dice. / サイズと色が異なる2種類のサイコロを使用しています。

* Image

| category | detail |
----|---- 
| Image Format | BMP |
| size | 128 x 128 |
| channel | 1 (Gray scale) |
| depth | 8 |

* labeld dataset

| Labeld Dice | count |
----|---- 
| 1 | 400 |
| 2 | 400 |
| 3 | 400 |
| 4 | 400 |
| 5 | 400 |
| 6 | 400 |

## Exhibition Information
We exhibited this project at [NT加賀2018](http://wiki.nicotech.jp/nico_tech/index.php?NT%E5%8A%A0%E8%B3%802018) for the first time.

### A sequel to the NT加賀2018
[@うえぽん](https://twitter.com/TomohiroUenoML) created a dice classification model using deep learning. However, the image data captured from the real world had a low recognition rate due to the effects of fluorescent lights flicker and shadows. We thought that augmentation for deep learning and in addition learning according to the real world was necessary. I think that it is domain knowledge or learning in HW on the real world side.

# Recognition Challenge
| Name | Remark |
----|----
| [@tomit3](https://twitter.com/tomit3) | Recognize the face of dice by counting circles using image processing and Hough transform. Co-author of this project. |
| [@うえぽん](https://twitter.com/TomohiroUenoML)/[llDataSciencell](https://github.com/llDataSciencell) | He is the first person in the world who made the model of dice recognition using Deep Learning. The training code using DNN is written below. Co-author of this project. |
| [@ミクミンP/Kazuhiro Sasao](https://twitter.com/ksasao) | Recognized the face of dice by transfer learning. He has written an article on transfer learning techniques in an offline using Windows. Articale is "[Windows PCかつオフライン環境でお気軽に画像認識する](https://qiita.com/ksasao/items/8a76d6048e28defeb39a)" |

# Source code for training using DNN
The source code for training this dataset is uploaded on this site.(Author [llDataSciencell](https://github.com/llDataSciencell))
- https://github.com/llDataSciencell/DiceRecognitionKeras/
