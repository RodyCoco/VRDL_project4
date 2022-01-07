# VRDL_project4


## Acknowledge
```
swinir: https://github.com/cszn/KAIR
The folder is rewritten from the above github resources.
```

## Requirements

To install requirements:

```setup
pip install -r requirements.txt
```

## Hardware

RTX A5000 *4


## Training
run:

```
python main_train_psnr.py --opt train_swinir_sr_classical.json
```
The training result will be in the folder "superresolution" .

## Testing
(Note that model.pth is already in this repository)
run:

```
python main_test_swinir.py --model_path  model.pth --task classical_sr --scale 3 \
    --folder_lq testing_lr_images --folder_gt testing_lr_images
```
The testing result will be in the folder "results" .
