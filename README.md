# 🍽️ Food101 Image Classification with ViT (Vision Transformer)

This project fine-tunes the powerful **ViT (Vision Transformer)** model from Hugging Face on a subset of the Food101 dataset to classify food images into 101 categories.

✅ **Validation Accuracy Achieved**: **95%**  
📦 **Model on Hugging Face Hub**: [ZiadElkafoury/food_model](https://huggingface.co/ZiadElkafoury/food_model)

---

## 🚀 Project Steps

1. **Dataset**: Used `datasets` library to load 5,000 samples from the [Food101](https://huggingface.co/datasets/food101) dataset.
2. **Preprocessing**: Applied resizing, normalization, and augmentations using the processor from `google/vit-base-patch16-224`.
3. **Model**: Fine-tuned `google/vit-base-patch16-224` with custom label mappings.
4. **Training**:
   - 15 epochs
   - Validation accuracy: **95%**
   - Batch size: 16
   - Optimized with weight decay and evaluation on each epoch.
5. **Inference**: Deployed the model in the form of FastAPI so it can classify new food images into one of the 101 classes.
