# FYP

This repository contains the code for the paper **"Face De-occlusion with Deep Cascade Guidance Learning"**.

## 1. test.py
This Python file is for testing. You just need to replace the `opt.test_dir` with your own test data path or use the dataset provided by us. The test file will output three files in the `./result` folder:
- `detect_mask`: The detection result.
- `parsing_mask`: The face parsing result.
- `rec_face`: The face de-occlusion result.

## 2. models
This folder contains two Python files:
- **`generator.py`**: Consists of four parts—detection, parsing, reconstruction, and discriminator.
- **`ops.py`**: Contains the operators used in `generator.py`.

## 3. trained_models
This folder contains two trained models:
- **`detect_parsing.pth`**: For detection and parsing.
- **`reconstruction.pth`**: For reconstruction.

You can download the trained models from Google Drive using this URL:  
[Download Trained Models](https://drive.google.com/drive/folders/1zNf6HATv3QtrKqGIQBq4af5qQAJ1RUcj?usp=sharing)

After downloading, place the trained models in the `trained_models` folder.

## 4. result
This folder will store the output results from the test.

## 5. test_image
This folder contains test images we provide. You can use them to verify our method. Of course, you can also test on your own dataset.

## 6. environment
The following libraries are required to run the code:

- **numpy**: 1.17.1
- **python**: 3.6.8
- **torch**: 1.0.1.post2
- **opencv-python**: 4.1.2.30
- **Pillow**: 6.1.0
- **CUDA**: 8.0.61
- **CUDNN**: 5.1.5
