# 🌸 Flower Classification using CNN & Transfer Learning

This project focuses on classifying flower images into five categories using deep learning techniques including custom CNNs and transfer learning with ResNet50 and EfficientNetB0.

---

## 🎯 Objective

To accurately classify flower images into:
**Daisy**, **Dandelion**, **Rose**, **Sunflower**, and **Tulip**.

---

## 📁 Dataset

- **Total Images**: ~4,500
- **Classes**: 5
- **Source**: Manually organized into folders per class
- **Processing**: Loaded with `image_dataset_from_directory`, resized to `(224, 224)`, normalized
- **Splits**: Training, validation, and test sets

---

## 🔄 Data Augmentation

Applied to increase generalization and robustness:
- `RandomFlip`
- `RandomRotation`
- `RandomZoom`
- `RandomContrast`
- `RandomTranslation`

---

## 🧠 Models Evaluated

| Model                 | Validation Accuracy |
|-----------------------|---------------------|
| Basic CNN             | ~86%                |
| VGG16-based CNN       | ~90%                |
| EfficientNetB0        | 93.28%              |
| ResNet50 (Fine-tuned) | 93.63%              |

---

## 📊 Model Evaluation

Each model was evaluated using validation and test datasets.  
Accuracy and loss curves were tracked across training epochs.

---

## 🧠 Download Trained Models

The trained models (best performing) are available here:

- [Model 3 – EfficientNetB0](https://drive.google.com/file/d/1rNjTh05HMzC42ac4wkDx2V8ZYDDyrYf3/view?usp=sharing)
- [Model 4 – Fine-tuned ResNet50](https://drive.google.com/file/d/1uJHMmi8NGfTyJyenN10FujpTJbej3Xg_/view?usp=sharing)

📌 **Note:** Download and place them in the same directory as your `.ipynb` file (or as expected in your notebook).

---

## 📝 Conclusion

Transfer learning (ResNet50 & EfficientNetB0) significantly improved classification accuracy compared to traditional CNNs. The fine-tuned models achieved over **93% accuracy**, making them suitable for real-world flower classification tasks.

---
