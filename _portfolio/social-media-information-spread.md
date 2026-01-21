---
title: "Information Spread on Social Media"
excerpt: "Analyzing 20M+ multilingual social media posts to track misinformation spread and predict viral content<br/><img src='/images/social-media-project.svg' onerror=\"this.src='/images/500x300.png'\">"
collection: portfolio
permalink: /portfolio/social-media-information-spread/
date: 2023-01-01
---

## Overview

This project represents a comprehensive analysis of information spread patterns across multiple social media platforms, focusing on understanding how information propagates and what makes content go viral. By analyzing over 20 million multilingual posts from X (Twitter) and Weibo, we developed predictive models for viral content identification. Our best-performing model (XGBoost with engineered features) achieved an F1-score of 0.82 and AUC-ROC of 0.89 on held-out test data, with precision of 0.79 and recall of 0.85 for the viral content class (defined as posts reaching >1000 engagements within 24 hours).

## Research Questions

- How does misinformation spread differently across cultural contexts?
- What linguistic and behavioral patterns predict viral content?
- How do user behavior patterns differ between Eastern and Western social media platforms?

## Methodology

### Data Collection
- **Scale**: 20+ million multilingual social media posts
- **Platforms**: X (Twitter) and Weibo
- **Languages**: English, Japanese, and Chinese
- **Time Period**: Multi-year longitudinal analysis
- **Behavioral Experiments**: Sharing intention experiment in the US and China (N = 400), eye-tracking (N = 100)

### Sampling Strategy

This project comprises multiple studies with different sampling approaches tailored to each research question:

**Study 1: Emotional and Moral Expression Dynamics (Twitter)**
- **Method**: Stratified random sampling—100 tweets sampled every hour for 12 months
- **Scope**: English tweets geolocated to the US; Japanese tweets geolocated to Japan
- **Purpose**: Examine how emotional and moral expressions drive information spread across cultural contexts
- **Total**: ~876,000 tweets per language

**Study 2: Controversial Topic Discourse (Weibo)**
- **Method**: Keyword-based purposive sampling targeting three controversial social topics
- **Scope**: Chinese-language posts and associated discussion threads
- **Purpose**: Analyze discourse patterns and information cascade structures around contentious issues

**Study 3: Misinformation Network Structure (Twitter)**
- **Method**: Keyword-based sampling of verified misinformation and matched true information
- **Scope**: Posts identified through fact-checking databases and matched controls
- **Purpose**: Compare network propagation structures between true and false information

### Technical Implementation

#### Natural Language Processing Pipeline
- **BERT Models**: Fine-tuned multilingual BERT for semantic understanding
- **Translation APIs**: Google Translate and Microsoft Translator for cross-language analysis
- **Sentiment Analysis**: Custom models trained on social media data
- **Topic Modeling**: Latent Dirichlet Allocation (LDA) and BERTopic

#### Machine Learning Models
- **Classification**: Random Forest, XGBoost, and neural networks for viral prediction
- **Time Series Analysis**: ARIMA models for trend prediction
- **Network Analysis**: Graph neural networks for information flow modeling
- **Feature Engineering**: 100+ linguistic, temporal, and social features

#### Infrastructure
- **Computing**: High-Performance Computing clusters
- **Storage**: Distributed database systems for large-scale data
- **Processing**: PySpark for parallel processing
- **APIs**: Custom APIs for real-time data collection

## Key Findings

### Drivers of Viral Content
We identified **two key drivers** of viral content spread:
- **Heterogeneous Emotion**: Posts expressing mixed or diverse emotional content (e.g., combining anger with hope) spread more widely than those with uniform emotional tone
- **Homogeneous Morality**: Posts with consistent moral framing (e.g., unified appeals to fairness or loyalty) achieve greater reach than those with conflicting moral messages

### Emotion Contagion
- **Western Platforms**: Emotional content spreads faster, especially positive emotions
- **Eastern Platforms**: Mixed emotional content spreads more easily
- **Language Effects**: Certain linguistic structures promote faster spread

### Misinformation Spread Patterns
- **Speed**: Consistent with prior research ([Vosoughi et al., 2018](https://www.science.org/doi/10.1126/science.aap9559)), we observed that false information spreads significantly faster than verified information in our dataset
- **Network Structure**: Misinformation creates denser, more connected networks (measured by clustering coefficient and average path length)
- **User Behavior**: False information paired with social approval cues (e.g., high like/retweet counts) showed 2.3x higher sharing intention in our behavioral experiments


## Impact and Applications

### Research Contributions
- Oral presentation at **SAS** 2022

### Practical Applications
- Social media monitoring tools for public health organizations
- Content recommendation improvements for social media platforms

### Policy Implications
- Provided evidence for regulatory discussions on information quality
- Supported digital literacy initiatives

## Technologies Used

<div class="tech-grid">
<div class="tech-category">
<h4>Programming Languages</h4>
<ul>
<li>Python (Primary)</li>
<li>SQL (Data Management)</li>
<li>JavaScript (Visualization)</li>
</ul>
</div>

<div class="tech-category">
<h4>Machine Learning</h4>
<ul>
<li>BERT, RoBERTa, XLM-R</li>
<li>PyTorch, TensorFlow</li>
<li>Scikit-learn</li>
<li>Hugging Face Transformers</li>
</ul>
</div>

<div class="tech-category">
<h4>Data Processing</h4>
<ul>
<li>PySpark</li>
<li>Pandas, NumPy</li>
<li>MongoDB, PostgreSQL</li>
</ul>
</div>

<div class="tech-category">
<h4>Visualization</h4>
<ul>
<li>D3.js</li>
<li>Plotly</li>
<li>NetworkX</li>
<li>Tableau</li>
</ul>
</div>
</div>

### Data Availability
- **Code**: Available on [OSF Repository](https://osf.io/b7rjk/overview?view_only=569f284163104f37a1b5f5af43d9386b)
- **Preprocessed Data**: Available upon request (due to privacy considerations)
- **Documentation**: Comprehensive documentation included

## Publications and Presentations

1. **Chen, Y., Chen, A. X., Yu, H., & Sun, S.** (2023). "Unraveling moral and emotional discourses on social media: a study of three cases." *Information, Communication & Society*. [DOI: 10.1080/1369118X.2023.2246551](https://www.tandfonline.com/doi/full/10.1080/1369118X.2023.2246551)

## Future Directions

### Technical Improvements
- Integration of multimodal analysis (text + images + videos)
- Real-time adaptation using online learning algorithms
- Causal inference methods for understanding information spread mechanisms

### Research Extensions
- Long-term longitudinal studies spanning multiple years
- Integration with offline behavior data
- Cross-platform analysis including emerging social media platforms

### Collaboration Opportunities
- Partnership with social media platforms for data access
- Collaboration with public health organizations
- Integration with fact-checking organizations

## Team and Acknowledgments

### Core Team
- **Amber X. Chen** (Lead Data Scientist)
- **Dr. Hongbo Yu** (Faculty Advisor, UCSB)
- **Dr. Helene Fung** (Faculty Advisor, CUHK)
- **Dr. Yibei Chen** (Research Collaborator, MIT)
- **Dr. Shaojing Sun** (Research Collaborator, Fudan University)

### Funding
- Research Grants Council of Hong Kong General Research Fund
- Interdisciplinary Research Seed Funding, CUHK

### Computing Resources
- UCSB Center for Scientific Computing
- CUHK High Performance Computing Centre
- Google Cloud Platform

---

*For more information about this project or to request access to data and code, please contact [amber.chen@psych.ucsb.edu](mailto:amber.chen@psych.ucsb.edu).*

<style>
.tech-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 1.5em;
  margin: 2em 0;
}

.tech-category {
  background: #f8f9fa;
  padding: 1.5em;
  border-radius: 8px;
  border-left: 4px solid #1976d2;
}

.tech-category h4 {
  margin-top: 0;
  color: #1976d2;
  font-size: 1.1em;
}

.tech-category ul {
  margin: 0;
  padding-left: 1.2em;
}

.tech-category li {
  margin-bottom: 0.3em;
  color: #555;
}
</style>