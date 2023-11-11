# Helmet Detection using YOLOv5

## Overview

This repository contains the implementation of an object detection model for detecting helmets using the YOLOv5 algorithm. The model is trained on a Kaggle dataset of images containing individuals wearing helmets. This project aims to provide accurate and efficient helmet detection for safety and security applications.

## Table of Contents

- [Prerequisites](#prerequisites)
- [Dataset](#dataset)
- [Training](#training)
- [Inference](#inference)
- [Model Evaluation](#model-evaluation)
- [Results](#results)
- [Customization](#customization)
- [Dependencies](#dependencies)
- [Contributing](#contributing)
- [License](#license)

## Prerequisites

Make sure you have the following prerequisites installed:

- Python 3.x
- PyTorch
- CUDA (optional but recommended for faster training)
- Other dependencies (refer to `requirements.txt`)

```bash
# Install dependencies
pip install -r requirements.txt
```

## Dataset

The model has been trained on a Kaggle dataset comprising images of individuals wearing helmets. Ensure your dataset is organized with annotated images to facilitate effective training.

## Training

To train the YOLOv5 model on the helmet dataset, follow these steps:

1. Organize the dataset with annotated images.
2. Prepare the training configuration file, e.g., `data/helmet.yaml`.
3. Train the model using the YOLOv5 training script.

```bash
# Example training command
python train.py --data data/helmet.yaml --cfg models/yolov5s.yaml --weights yolov5s.pt
```

## Inference

To use the trained model for inference on new images, follow these steps:

1. Run the `detect.py` script with the path to the test images and the trained model weights.

```bash
# Example inference command
python detect.py --source path/to/test/images --weights path/to/trained/model.pt
```

## Model Evaluation

Evaluate the model's performance using the following steps:

1. Use the `evaluate.py` script with the data configuration and the trained model weights.

```bash
# Example evaluation command
python evaluate.py --data data/helmet.yaml --weights path/to/trained/model.pt
```

## Results

Explore the results of the model, including visualizations of detections on sample images. Refer to the `results` directory for detailed analysis and insights.

## Customization

Adapt the model for your specific use case by customizing the dataset or fine-tuning the model. You can modify configurations or train additional epochs as needed.

## Dependencies

List of dependencies can be found in the `requirements.txt` file. Install them using the following command:

```bash
pip install -r requirements.txt
```

## Contributing

Contributions are welcome! Report bugs, request features, or submit pull requests to enhance the project. Refer to the `CONTRIBUTING.md` file for more details.

## License

This project is licensed under the [MIT License](LICENSE). Feel free to use, modify, and distribute the code for your purposes.

---
Kaggle Datset : https://www.kaggle.com/datasets/raghavnanjappan/weapon-dataset-for-yolov5
colaboratory : https://colab.research.google.com/drive/1Ws_cAGbsrpncepXr56uxW1MRBEcpO816#scrollTo=1xBCoi7DAhH8
