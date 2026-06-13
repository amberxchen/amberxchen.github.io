---
title: "Deep Learning Health Prediction"
excerpt: "Designing neural networks for biological age prediction achieving 4.09 years MAE, revealing psychological factors' impact on aging<br/><img src='/images/health-prediction-project_full.png' onerror=\"this.src='/images/500x300.png'\">"
collection: portfolio
permalink: /portfolio/health-aging-prediction/
date: 2022-07-01
project:
  order: 4
  categories: "health ml"
  image: /images/health-prediction-project_full.png
  description: "Designed deep neural networks for longitudinal health data analysis, achieving 4.09 years mean absolute error on aging prediction with 2,000+ participants."
  tech: [Deep Learning, TensorFlow, Medical Data, Feature Engineering]
  links:
    - label: Paper
      url: "https://doi.org/10.18632/aging.204264"
    - label: Press Release
      url: "https://www.nmn.com/news/study-finds-poor-psychological-states-accelerate-aging-more-than-smoking"
  status: completed
  status_label: "Completed"
  badge: "Published in 2022"
---

<div style="text-align: center; margin: 2em 0;">
  <img src="/images/health-prediction-project_full.png" alt="Deep Learning Health Prediction Overview" style="max-width: 100%; height: auto; border-radius: 8px; box-shadow: 0 4px 12px rgba(0,0,0,0.15);">
</div>

## Overview

This groundbreaking project applies deep learning to longitudinal health data, creating an AI-powered "aging clock" that predicts biological age with unprecedented accuracy. Our deep neural network achieved a mean absolute error of 4.09 years while revealing that psychological factors substantially contribute to biological aging—with effects comparable to or exceeding traditional risk factors like smoking.

## Research Significance

### Scientific Impact
- **First study** to quantify psychological aging effects using deep learning
- **Novel methodology** for integrating biomarkers with behavioral data
- **Policy relevance** for public health strategies and mental health prioritization

### Key Discovery
> "Psychological factors substantially contribute to biological aging: Evidence from the aging rate in Chinese older adults"

Our research demonstrates that mental health isn't just correlated with physical health—it directly impacts the biological aging process in measurable and quantifiable ways.

## Methodology

### Dataset: China Health and Retirement Longitudinal Study (CHARLS)

- **Sample Size**: 2,000+ participants
- **Age Range**: 45-85 years old
- **Geographic Coverage**: 28 provinces across China
- **Data Points**: 12,000+ individual measurements

### Deep Learning Architecture

Our aging clock employs a multi-layer neural network designed to capture complex, non-linear relationships between biomarkers and chronological age, while identifying deviations that represent accelerated or decelerated aging.

<div style="text-align: center; margin: 2em 0;">
  <img src="/images/health-prediction-project_1.png" alt="Deep Learning Health Prediction Architecture" style="max-width: 100%; height: auto; border-radius: 8px; box-shadow: 0 4px 12px rgba(0,0,0,0.15);">
  <p style="font-style: italic; color: #666; margin-top: 1em; font-size: 0.9em;">Deep neural network architecture for biological age prediction using biomarkers and biometric data</p>
</div>

- Network Architecture
  - **Input Layer**: 24 biomarker features with batch normalization
  - **Hidden Layers**: Progressive dimensionality reduction (128 → 64 → 32 neurons)
  - **Regularization**: Dropout layers to prevent overfitting
  - **Output Layer**: Single neuron predicting biological age
  - **Optimization**: Xavier weight initialization and Adam optimizer

- Training Strategy
  - **Loss Function**: Mean Absolute Error (L1 Loss) for robust age prediction
  - **Optimizer**: Adam optimizer with weight decay for regularization
  - **Learning Rate**: Adaptive scheduling with plateau detection
  - **Early Stopping**: Prevents overfitting with 20-epoch patience
  - **Cross-Validation**: 5-fold validation for robust performance assessment
  - **Data Split**: 80% training, 20% validation with stratified sampling

## Key Findings

### Model Performance Metrics

- **Mean Absolute Error (Cross-Validation)**: 4.18 years  
- **Mean Absolute Error (Test Set)**: 4.09 years
- **Mean Absolute Percentage Error (CV)**: 7.57%
- **Mean Absolute Percentage Error (Test)**: 6.37%
- **Sample Size**: 4,846 participants (CV), 4,451 participants (Test)


### Psychological and social factors on biological aging:

| Factor Category | Variable | Coefficient | Standard Error | Effect |
|----------------|----------|-------------|----------------|---------|
| **Psychological** | Rarely feels lonely | +0.05 | 0.03 | Loneliness accelerates aging |
| **Psychological** | Rarely feels happy | +0.35 | 0.02 | **Low happiness accelerates aging** |
| **Psychological** | Rarely hopeful | +0.28 | 0.01 | **Hopelessness accelerates aging** |
| **Psychological** | Rarely depressed | -0.09 | 0.02 | Depression accelerates aging |
| **Psychological** | Rarely fearful | -0.29 | 0.02 | Fear accelerates aging |
| **Psychological** | Restless sleep is rare | -0.44 | 0.01 | **Sleep problems accelerate aging** |
| **Social** | Is married | -0.59 | 0.04 | **Marriage protective** |
| **Social** | Is rural | +0.39 | 0.01 | Rural living accelerates aging |
| **Behavioral** | Currently smoking | +1.25 | 0.02 | **Smoking accelerates aging** |

## Clinical and Practical Applications

### Healthcare Implementation

- **Risk Stratification**: Identify individuals at high risk for accelerated aging
- **Intervention Targeting**: Prioritize mental health interventions for aging prevention
- **Treatment Monitoring**: Track biological age changes in response to treatments
- **Prevention Strategies**: Early identification of aging acceleration

### Public Health Implications
- **Mental Health Priority**: Psychological interventions show measurable anti-aging effects
- **Healthcare Resource Allocation**: Target mental health services for aging prevention
- **Policy Development**: Evidence-based support for mental health integration in aging care
- **Prevention Programs**: Community-based interventions to reduce psychological aging

## Publications and Recognition


### Primary Publication
**Galkin, F., Kochetov, K., Koldasbayeva, D., Fung, H. H, Chen, A. X., & Zhavoronkov, A.** (2022). "Psychological factors substantially contribute to biological aging: Evidence from the aging rate in Chinese older adults." *Aging*, 14(18), 7206-7222. [DOI: 10.18632/aging.204264](https://doi.org/10.18632/aging.204264)

### Media Coverage
- **Scientific Recognition**: Featured in *Aging* journal (50+ citations till mid 2025)
- **Press Coverage**: [Press release](https://www.aging-us.com/news-room/Psychological-factors-substantially-contribute-to-biological-aging-evidence-from-the-aging-rate-in-Chinese-older-adults) highlighting clinical significance
- **Health News Coverage**: [Study finds poor psychological states accelerate aging more than smoking](https://www.nmn.com/news/study-finds-poor-psychological-states-accelerate-aging-more-than-smoking)
- **Research Impact**: [Stanford researchers propose psychological stress as a crucial hallmark of aging](https://www.nad.com/news/stanford-researchers-propose-psychological-stress-as-a-crucial-hallmark-of-aging)
- **Industry Impact**: Referenced in healthcare AI development strategies

## Future Research Directions
- **Longitudinal Modeling**: RNN/LSTM for temporal progression tracking
- **Multi-omics Integration**: Incorporate genomic and proteomic data
- **Causal Inference**: Move beyond correlation to causal aging mechanisms

---

*This project demonstrates the potential of AI to revolutionize our understanding of aging and health. The discovery that psychological factors substantially impact biological aging opens new avenues for intervention and prevention.*

<style>
.tech-infrastructure {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 1.5em;
  margin: 2em 0;
}

.tech-category {
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  color: white;
  padding: 1.8em;
  border-radius: 10px;
  box-shadow: 0 4px 12px rgba(102, 126, 234, 0.3);
}

.tech-category h4 {
  margin-top: 0;
  margin-bottom: 1em;
  font-size: 1.1em;
  font-weight: 600;
}

.tech-category ul {
  margin: 0;
  padding-left: 1.2em;
  list-style-type: none;
}

.tech-category li {
  margin-bottom: 0.5em;
  color: #f0f0f0;
  line-height: 1.3;
  position: relative;
}

.tech-category li:before {
  content: "•";
  color: #a8b5ff;
  position: absolute;
  left: -1.2em;
  font-size: 1.2em;
}

table {
  width: 100%;
  border-collapse: collapse;
  margin: 1.5em 0;
  background: white;
  box-shadow: 0 2px 8px rgba(0,0,0,0.1);
}

th, td {
  padding: 0.8em;
  text-align: left;
  border-bottom: 1px solid #e0e0e0;
}

th {
  background: #f8f9fa;
  font-weight: 600;
  color: #495057;
}

tr:hover {
  background: #f8f9fa;
}

.highlight {
  background: linear-gradient(120deg, #f093fb 0%, #f5576c 100%);
  color: white;
  padding: 0.2em 0.5em;
  border-radius: 4px;
  font-weight: 600;
}
</style>