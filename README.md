# DAPP
Distribution-Aware Federated Prompt Personalization for Robust Cross-Center Medical Image Classification

# Dataset
Link for the Dataset:

https://www.kaggle.com/competitions/aptos2019-blindness-detection/data for APTOS dataset


https://www.kaggle.com/datasets/mariaherrerot/ddrdataset to access DDR dataset


https://challenge.isic-archive.com/data/#2019 for FedISIC dataset.


# Hyperparameters Used

### Federated Training Protocol for All Datasets in DAPP (Our) Approach

| **Setting** | **FLamby ISIC 2019** | **APTOS + DDR** |
|-------------|---------------------|-----------------|
| Number of Clients | 6 | 10 (5 India + 5 China) |
| Number of Classes | 8 | 5 |
| Communication Rounds | 20 | 5 |
| Client Participation | All clients | All clients |
| Local Epochs per Round | 10 | 10 |
| Batch Size | 32 | 32 |
| Optimizer | Adam | Adam |
| Learning Rate (Prompt) | 1×10⁻² | 1×10⁻² |
| Learning Rate (Classifier) | 1×10⁻³ | 1×10⁻³ |
| Backbone | ViT-B/16 (Frozen) | ViT-B/16 (Frozen) |
| Prompt Experts (M) | 10 | 10 |
| Prompt Length (L) | 5 | 5 |
| Metric Used | Balanced Accuracy | Accuracy |
| Loss Function | Focal Loss | Cross Entropy |
| Focal Loss γ | 2 | Not Applicable |
| Aggregation Weight | Inverse Val. Loss | Inverse Val. Loss |
