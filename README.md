# Box-IS
RGB-D instance segmentation box dataset 

![image](./img/img1.jpg)

```
Train   : 488 images
Val     : 55 images
Classes : 1
Size    : 1280 × 720
```

## Data preparation

Box-IS : https://huggingface.co/datasets/kasurashan/RGBD-Instance-Segmentation

```
Box-IS/
└── train2017/
└── val2017/
└── annotations/
    └── instances_train2017.json
    └── instances_val2017.json
└── train2017_depth/
└── val2017_depth/
```

## Data Format
```
annotation{
    "id": int,
    "image_id": int,
    "category_id": int,
    "segmentation": [polygon],
    "area": float,
    "bbox": [x,y,width,height],
    "iscrowd": 0 or 1,
}

categories[{
    "id": int,
    "name": str,
    "supercategory": str,
}]
```


