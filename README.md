# Dataset

| Dataset |
| :-: | 
| [**VinAI**](https://github.com/VinAIResearch/dict-guided#dataset) | 
| [**VietOCR**](https://github.com/pbcquoc/vietocr) | 
| [**VietOCR-github**](https://github.com/dotrannhattuong/datasetOCR) |



# Description

## Data Detection
```
dataset_det/
folder
  ├── test_image/ - Testing Set VinAI
  ├── train_images/ - Training Set VinAI
  ├── unseen_test_images/ - Unseen Set VinAI
  ├── Data Menu_Đề 1_AI Hackathon/ - Label Data Menu
  
txt files
  ├── test_label.txt - Testing Set VinAI
  ├── train_label.txt - Training Set VinAI
  ├── unseen_label.txt - Unseen Set VinAI        
  ├── label_menu.txt - Label Data Menu for char
  ├── datadet.txt - Merge VinAI and Menu Dataset
  ├── train_datadet.txt - Training Set datadet (80%)
  ├── val_datadet.txt - Validation Set datadet (20%)
```

## Data Recognition
```
dataset_rec/
folder
  ├── test_image/ - Testing Set VinAI
  ├── train_images/ - Training Set VinAI
  ├── unseen_test_images/ - Unseen Set VinAI
  ├── train_images_char/ - Label Data Menu for char
  ├── train_images_menu/ - Label Data Menu for sentences
  
txt files
  ├── vinai.txt - Total Dataset VinAI
  ├── crop_test_label.txt - Testing Set VinAI
  ├── crop_label.txt - Training Set VinAI
  ├── crop_unseen_label.txt - Unseen Set VinAI        
  ├── crop_label_char.txt - Label Data Menu for char
  ├── crop_label_menu.txt - Label Data Menu for sentences
  ├── datacrop.txt - Merge VinAI and Menu Dataset
  ├── train_datacrop.txt - Training Set datacrop (80%)
  ├── val_datacrop.txt - Validation Set datacrop (20%)
```

## Dictionary
```
ppocr_dict.txt: Merge dictionary VietOCR, Menu, VinAI
vi_vietnam.txt: for VietOCR
vn_dictionary.txt: for VinAI
```

## Training
```
Text Detection:
    All: datadet.txt
    Training Set: train_datadet.txt
    Validation Set: val_datadet.txt
Text Recognition:
    All: datacrop.txt
    Training Set: train_datacrop.txt
    Validation Set: val_datacrop.txt
```