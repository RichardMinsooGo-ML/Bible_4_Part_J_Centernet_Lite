<p align="center"><img src="https://wikidocs.net/images/page/225910/under-construction.png" width="500px"></p>

## Engilish
*  **Theory** : [https://wikidocs.net/227243](https://wikidocs.net/227243) <br>
*  **Code** : [https://wikidocs.net/227244](https://wikidocs.net/227244)

## 한글
*  **Theory** : [https://wikidocs.net/226021](https://wikidocs.net/226021) <br>
*  **Code** : [https://wikidocs.net/225910](https://wikidocs.net/225910)

This repository is folked from [https://github.com/yjh0410/CenterNet-Lite](https://github.com/yjh0410/CenterNet-Lite).
At this repository, simplification and explanation and will be tested at Colab Environment. Some bugs were fixed.


## Train
### VOC
```Shell
python train.py --cuda -d voc
```

You can run ```python train.py -h``` to check all optional argument.

### COCO
```Shell
python train.py --cuda -d coco
```

## Test
### VOC
```Shell
python test.py --cuda -d voc --trained_model [ Please input the path to model dir. ]
```

### COCO
```Shell
python test.py --cuda -d coco-val --trained_model [ Please input the path to model dir. ]
```


## Evaluation
### VOC
```Shell
python eval.py --cuda -d voc --train_model [ Please input the path to model dir. ]
```

### COCO
To run on COCO_val:

```Shell
python eval.py --cuda -d coco-val --train_model [ Please input the path to model dir. ]
```

To run on COCO_test-dev(You must be sure that you have downloaded test2017):

```Shell
python eval.py --cuda -d coco-test --train_model [ Please input the path to model dir. ]
```

