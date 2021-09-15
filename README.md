### Reference
(1) Code : https://github.com/sgrvinod/a-PyTorch-Tutorial-to-Image-Captioning  
(2) Paper : https://arxiv.org/abs/1502.03044

### Data setup
#### Data
```shell
wget http://images.cocodataset.org/zips/train2014.zip
wget http://images.cocodataset.org/zips/val2014.zip
wget http://images.cocodataset.org/zips/test2014.zip
```
#### Annotation
Download splits and captions in this [***link***](https://www.kaggle.com/shtvkumar/karpathy-splits)

### Quick implementation
```shell
python create_input_files.py
python train.py
python eval.py
python caption.py --img='path/to/img.jpg' \
--model='path/to/model.pth.tar' \
--word_map='path/to/WORDMAP.json' --beam_size=5
```
