# CDRL-SA

## Update Note
* This repository will be completed on the date of the #### presentation.

> [**Unsupervised Change Detection Based on Image Reconstruction Loss with Segment Anything**](-)
> 
> [Hyeoncheol Noh](https://scholar.google.co.kr/citations?user=XTmafQgAAAAJ&hl), [Jingi Ju](https://scholar.google.co.kr/citations?user=hlJYrqAAAAAJ&hl), Minwoo Kim, Yuhyun Kim, [Minseok Seo](https://scholar.google.co.kr/citations?user=pOygDIIAAAAJ&hl), [Dong-Geol Choi](https://scholar.google.co.kr/citations?user=1498JWoAAAAJ&hl)
> 
> *[arXiv](-)*
> 
> *[Project Page](-)*

## Getting Started

Dataset download link : 
* [LEVIR-CD](https://drive.google.com/file/d/18RGfTqPo1atw_IMm6xPOnND-Vl4ok_o3/view?usp=sharing) (Our multi-class LEVIR dataset is included in that link.)
* [LEVIR-CD_A2B_B2A](https://drive.google.com/file/d/1-LERpM7GOxviKna47bbO_mLQON3Q0YcA/view?usp=sharing)
* [CLCD-CD](https://drive.google.com/file/d/1F4RfWSvoghmIrir_2YlBYfgrJt-flzY8/view?usp=sharing)
* [CLCD-CD_A2B_B2A](https://drive.google.com/file/d/1Q9COBNxg7r5PhgNzY60GTugotbS8AzUg/view?usp=sharing)

```angular2html
CDRL-SA
    └──datasets
        ├── LEVIR-CD
            ├── val
            ├── test
            └── train
                ├── A
                ├── B
                └── label
        ├── LEVIR-CD_A2B_B2A
            └── train
                ├── A
                └── B
        ├── CLCD-CD
        └── CLCD-CD_A2B_B2A
```

## Train
```bash
python main.py --root_path ./datasets/ --dataset_name LEVIR-CD --save_name levir
```

## Eval
```bash
python test.py --root_path ./datasets/ --dataset_name LEVIR-CD --save_name levir
```

