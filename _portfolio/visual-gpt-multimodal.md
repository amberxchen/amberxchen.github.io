---
title: "VisualGPT: Multimodal AI for User Perception"
excerpt: "Developing dual-route models that integrate language and vision to predict user impressions, achieving +20% accuracy improvement<br/><img src='/images/visual-gpt-project.svg' onerror=\"this.src='/images/500x300.png'\">"
collection: portfolio
permalink: /portfolio/visual-gpt-multimodal/
date: 2024-01-01
---

## Overview

VisualGPT represents a breakthrough in multimodal AI that bridges the gap between computational vision models and human perception. By developing a dual-route processing framework that integrates state-of-the-art language models (GPT) with computer vision architectures (VGG, CLIP), we achieved a 20% improvement in predicting human impressions of visual content compared to baseline models.

## Project Motivation

Traditional computer vision models excel at object recognition but fail to capture the nuanced human impressions that drive real-world decisions. Our research addresses this gap by:

- **Modeling Human Perception**: Creating AI systems that predict human emotional and cognitive responses to visual content
- **Multimodal Integration**: Combining textual context with visual features for more accurate predictions
- **Practical Applications**: Enabling better user experience design, content curation, and human-AI interaction

## Theoretical Framework

### Dual-Route Processing Model

Our approach is inspired by dual-process theories in cognitive psychology, implementing two parallel processing pathways:

#### Route 1: Perceptual Processing
- **Input**: Raw visual features extracted using VGG-16/19 and ResNet architectures
- **Processing**: Direct feature mapping to impression dimensions
- **Characteristics**: Fast, automatic, bottom-up processing
- **Output**: Basic visual impression predictions

#### Route 2: Conceptual Processing  
- **Input**: Visual content described through natural language (via image captioning)
- **Processing**: GPT-based semantic understanding and contextual reasoning
- **Characteristics**: Slower, controlled, top-down processing
- **Output**: Context-aware impression predictions

#### Integration Layer
- **Fusion Strategy**: Learned attention mechanisms to weight perceptual vs. conceptual routes
- **Adaptive Weighting**: Context-dependent route importance
- **Final Prediction**: Ensemble output optimized for human impression alignment

## Technical Implementation

### Data Collection and Processing

#### Visual Content Dataset
- **Scale**: 10+ years of web news images and associated text
- **Sources**: Major news websites, social media platforms, art databases
- **Size**: 2.5 million images with corresponding textual descriptions
- **Annotations**: Human impression ratings on 20+ perceptual dimensions

#### Impression Dimensions
- Competence, Warmth, Strength, Charisma, Practicality, etc.

## Results and Performance

### Quantitative Results

#### Impression Prediction Performance
- **Baseline Model (VGG-16 only)**: R² = 0.52, Spearman r = 0.72
- **GPT-only Model**: R² = 0.47, Spearman r = 0.69
- **Dual-Route Model**: R² = 0.76, Spearman r = 0.87 (**+46% variance explained vs. baseline**)
- **Human-AI Agreement**: Pearson r = 0.84 with averaged human ratings (human inter-rater reliability: ICC = 0.81)

#### Error Analysis
- **Edge Cases**: Highly abstract or symbolic content
- **Improvement Areas**: Better handling of contextual nuances

## Technical Innovations

#### Cross-Modal Alignment
- **Contrastive Learning**: Align visual and textual representations in shared space
- **Mutual Information Maximization**: Ensure complementary route information
- **Semantic Consistency**: Maintain coherence between modalities

### Benchmark Creation
- **VisualImpression Dataset**: New benchmark for human impression prediction
- **Evaluation Metrics**: Novel metrics for multimodal impression assessment
- **Baseline Comparisons**: Systematic evaluation against existing methods

## Applications and Impact

### Real-World Applications

#### Digital Marketing
- **Ad Effectiveness Prediction**: Predict user engagement before campaign launch
- **Creative Optimization**: Automatically adjust visual content for target audiences
- **Brand Impression Management**: Monitor and optimize brand visual presence

#### User Experience Design
- **Interface Optimization**: Predict user reactions to UI/UX designs
- **Content Curation**: Personalized visual content recommendation
- **Accessibility Enhancement**: Predict usability across diverse user groups

## Future Development

### Technical Roadmap

#### Version 2.0 Enhancements
- **Video Analysis**: Extend to temporal visual content

## Technical Stack

<div class="tech-ecosystem">
<div class="tech-group">
<h4>Deep Learning Frameworks</h4>
<ul>
<li>PyTorch 2.0 (Primary framework)</li>
<li>TensorFlow 2.x (Comparison models)</li>
<li>Hugging Face Transformers</li>
<li>OpenAI API (GPT integration)</li>
</ul>
</div>

<div class="tech-group">
<h4>Computer Vision</h4>
<ul>
<li>OpenCV (Image processing)</li>
<li>Pillow (Image manipulation)</li>
<li>torchvision (Model architectures)</li>
<li>CLIP (Vision-language models)</li>
</ul>
</div>

<div class="tech-group">
<h4>Data Processing</h4>
<ul>
<li>pandas (Data manipulation)</li>
<li>numpy (Numerical computing)</li>
<li>scipy (Statistical analysis)</li>
<li>scikit-learn (ML utilities)</li>
</ul>
</div>

<div class="tech-group">
<h4>Infrastructure</h4>
<ul>
<li>CUDA 11.8 (GPU acceleration)</li>
<li>Docker (Containerization)</li>
<li>MLflow (Experiment tracking)</li>
<li>Weights & Biases (Model monitoring)</li>
</ul>
</div>
</div>

## Team and Collaboration

- **Amber X. Chen** (Principal Investigator & Lead Developer)
- **Dr. Hongbo Yu** (Faculty Advisor)
- **Dr. Ruonan Cao & Dr. Shuo Wang** (Collaborators in Neuroscience, WUSTL)

---

*VisualGPT represents a significant advancement in AI's ability to understand and predict human visual perception. For collaboration opportunities, technical discussions, or access to models and datasets, please contact [amber.chen@psych.ucsb.edu](mailto:amber.chen@psych.ucsb.edu).*

<style>
.tech-ecosystem {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 2em;
  margin: 2.5em 0;
}

.tech-group {
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  color: white;
  padding: 2em;
  border-radius: 12px;
  box-shadow: 0 4px 15px rgba(102, 126, 234, 0.3);
  transition: transform 0.3s ease;
}

.tech-group:hover {
  transform: translateY(-5px);
}

.tech-group h4 {
  margin-top: 0;
  margin-bottom: 1em;
  font-size: 1.2em;
  font-weight: 600;
  color: #ffffff;
}

.tech-group ul {
  margin: 0;
  padding-left: 1.2em;
  list-style-type: none;
}

.tech-group li {
  margin-bottom: 0.6em;
  color: #f0f0f0;
  line-height: 1.4;
  position: relative;
}

.tech-group li:before {
  content: "▶";
  color: #a8b5ff;
  position: absolute;
  left: -1.2em;
}

pre {
  background: #1e1e1e;
  color: #d4d4d4;
  border-radius: 8px;
  padding: 1.5em;
  overflow-x: auto;
  font-size: 0.9em;
  line-height: 1.4;
}

code {
  background: #f5f5f5;
  color: #d73a49;
  padding: 0.2em 0.4em;
  border-radius: 4px;
  font-size: 0.9em;
}

.highlight {
  background: linear-gradient(120deg, #a8edea 0%, #fed6e3 100%);
  padding: 0.2em 0.4em;
  border-radius: 4px;
  font-weight: 600;
}
</style>