# RSNA Mammography Breast Cancer Detection
### Kaggle Competition: Top 68%
This project was developed for the RSNA Mammography Breast Cancer Detection competition on Kaggle, where I ranked in the top 68%. The goal was to create a deep learning pipeline capable of detecting breast cancer from mammograms. This competition challenged participants to address real-world complexities such as highly imbalanced datasets and the need for high model sensitivity.

## Key Features

- Data Preprocessing: Tailored preprocessing techniques for medical imaging, including contrast enhancement and resizing, to optimize mammogram analysis.
- Deep Learning Models: Fine-tuned state-of-the-art transferred models like EfficientNet and ResNet, leveraging pre-trained weights for medical image analysis.
- Loss Function Optimization: Utilized binary cross-entropy (BCE) loss, which proved sufficient for handling the imbalanced dataset effectively.
- Evaluation Metrics: Focused on recall, precision, and AUC-ROC to ensure the model’s predictions aligned with medical priorities.

## Challenges

The most significant challenge was the severe class imbalance in the training dataset: only 0.03% of samples represented positive cases of breast cancer.

- Detection Problem: The problem resembled a needle-in-a-haystack scenario, where the model needed to differentiate a rare true positive from overwhelming negatives.
- Systematic Bias: Without proper training, the model could default to predicting "no cancer" for all cases, achieving high accuracy but failing in real-world applicability.
- Solution: By carefully tuning the BCE loss and employing oversampling techniques, the model was trained to focus on rare positive samples while maintaining generalization.

## Key Takeaways

- Loss Function Simplicity: Surprisingly, a simple vanilla BCE loss was sufficient for effective training in this scenario.
- Pretrained Models Excel: Fine-tuned EfficientNet and ResNet outperformed other architectures, demonstrating their robustness in medical imaging tasks.
- Real-World Applicability: The model needed to "really know" when it predicted a positive case, underscoring the importance of precise model evaluation in medical AI.

## Insights

This was my first Kaggle competition in medical imaging detection, and it was a transformative experience. Tackling such a challenging real-world problem deepened my passion for AI and its applications in healthcare. The competition taught me the importance of perseverance, methodical experimentation, and understanding the domain-specific requirements of AI solutions.

## Data
Due to privacy, data is available only on [Kaggle RSNA Dataset](https://www.kaggle.com/c/rsna-breast-cancer-detection/data).
RSNA Mammography Breast Cancer Detection
