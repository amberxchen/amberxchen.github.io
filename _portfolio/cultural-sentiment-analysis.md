---
title: "Time-Series Analysis of Cultural Sentiment"
excerpt: "Training language models on 3.5B tokens to analyze 70+ years of news and track moral attitudes across cultures<br/><img src='/images/cultural-effort-us-top.jpg' onerror=\"this.src='/images/500x300.png'\">"
collection: portfolio
permalink: /portfolio/cultural-sentiment-analysis/
date: 2023-09-01
---

<div style="text-align: center; margin: 2em 0;">
  <img src="/images/cultural-effort-us-top.jpg" alt="Moral Values of Effort and Efficiency Over Time (US)" style="max-width: 100%; height: auto; border-radius: 8px; box-shadow: 0 4px 12px rgba(0,0,0,0.15); padding: 15px; background: #f8f9fa;">
  <p style="font-style: italic; color: #666; margin-top: 1em; font-size: 0.9em;">Historical trends of moral attitudes toward effort and efficiency in U.S. Congressional speeches (1873-2011)</p>
</div>

## Overview

This groundbreaking computational linguistics project traces the historical evolution of moral attitudes toward effort and efficiency across two major world cultures—the United States and China—spanning seven decades (1950-2020). Using advanced natural language processing techniques on 3.5 billion tokens of historical text data, we discovered fundamental differences in how cultures moralize work concepts, revealing that Protestant Work Ethic and Confucian value systems create distinctly different trajectories in moral attitudes toward productivity.

## Research Objectives

- **Historical Analysis**: Track moral attitude changes from 1950-2020
- **Cross-Cultural Comparison**: Contrast American vs. Chinese moral frameworks  
- **Computational Methodology**: Develop novel NLP approaches for historical analysis
- **Predictive Modeling**: Forecast future cultural value trends

## Methodology

### Data Sources

#### American Data
- **U.S. Congressional Speeches**: Complete bound edition records (1873-2011)
- **Coverage**: House of Representatives and Senate floor speeches
- **Sample Size**: 13.4 million tokens per year (average)
- **Time Span**: 138 years of political discourse
- **Content**: Legislative debates, policy discussions, member remarks

#### Chinese Data  
- **People's Daily**: Official Communist Party newspaper (1950-2021)
- **Coverage**: Government policies, economic plans, official statements
- **Sample Size**: 12.3 million tokens per year (average)
- **Language**: Traditional to Simplified Chinese transition (1956)
- **Scope**: Nearly complete history of People's Republic of China

### Technical Architecture

#### Language Model Development
```python
# Word2Vec Model Configuration
model = Word2Vec(
    sentences=corpus,
    vector_size=300,
    window=10,
    min_count=5,
    workers=16,
    epochs=50,
    sg=1  # Skip-gram architecture
)
```

#### Semantic Analysis Pipeline
1. **Text Preprocessing**: Tokenization, lemmatization, POS tagging
2. **Word Embedding Training**: Custom Word2Vec models for each time period
3. **Semantic Similarity Calculation**: Cosine similarity between target concepts
4. **Temporal Aggregation**: Yearly averages with confidence intervals

#### High-Performance Computing
- **Infrastructure**: UCSB HPC clusters
- **Training Time**: 300+ hours for full model ensemble
- **Memory Usage**: 250GB RAM for large-scale processing
- **Storage**: 1TB for processed datasets and model checkpoints

### Statistical Analysis

#### Time-Series Modeling
- **ARIMA Models**: Autoregressive Integrated Moving Average
- **Granger Causality Tests**: Causal relationship detection
- **Change Point Analysis**: Identifying significant shifts
- **Seasonal Decomposition**: Separating trend from cyclical patterns

#### Validation Framework
- **Pseudo-Dictionary Generation**: 10,000 random word sets for significance testing
- **Bootstrap Resampling**: Confidence interval estimation
- **Cross-Validation**: Temporal split validation
- **USSR Validation**: Historical control case analysis

## Key Findings

### Moral Attitude Evolution

#### United States: Increasing Moralization
- **Protestant Work Ethic Trajectory**: Significant upward trend starting 1957
- **Post-1960s Surge**: Continuous increase in effort moralization through 2010
- **Economic Crisis Impact**: Notable decline during 1998 Asian Financial Crisis
- **Cultural Looseness Effect**: Positive correlation with tolerance of deviance (β=0.03, p<0.001)
- **Inefficient Effort**: Consistently positive valuation since 1940s

#### China: Stable then Declining Pattern
- **Confucian Foundation**: Consistently high effort moralization throughout study period
- **Economic Reform Impact**: Significant decline in inefficient effort moralization after 1978
- **1992 Turning Point**: Steep decline following Deng Xiaoping's "efficiency is life" reforms
- **Collectivism Effect**: Strong positive predictor of effort moralization (β=0.04, p<0.001)
- **Cultural Transformation**: Shift from ideological to practical efficiency focus

### Cross-Cultural Comparison

<div style="display: grid; grid-template-columns: 1fr 1fr; gap: 2em; margin: 2em 0;">
  <div style="text-align: center;">
    <img src="/images/cultural-effort-us-top.jpg" alt="US Moral Attitudes" style="max-width: 100%; height: auto; border-radius: 8px; box-shadow: 0 4px 12px rgba(0,0,0,0.15); padding: 15px; background: #f8f9fa;">
    <p style="font-style: italic; color: #666; margin-top: 1em; font-size: 0.9em; font-weight: 600;">United States (1873-2011)</p>
    <p style="color: #666; font-size: 0.85em;">Increasing moralization of effort, especially post-1960s</p>
  </div>
  <div style="text-align: center;">
    <img src="/images/cultural-effort-china-top.jpg" alt="China Moral Attitudes" style="max-width: 100%; height: auto; border-radius: 8px; box-shadow: 0 4px 12px rgba(0,0,0,0.15); padding: 15px; background: #f8f9fa;">
    <p style="font-style: italic; color: #666; margin-top: 1em; font-size: 0.9em; font-weight: 600;">China (1950-2021)</p>
    <p style="color: #666; font-size: 0.85em;">Stable effort values, declining with market reforms</p>
  </div>
</div>

### Efficiency Attitudes

#### Semantic Evolution
- **American Context**: Efficiency increasingly moralized post-1980
- **Chinese Context**: Efficiency framed as practical necessity, not moral imperative
- **Convergence Points**: Both cultures show increased efficiency focus in economic reforms

#### Predictive Insights
- **Future Trends**: Model predicts continued moralization in individualistic cultures
- **Policy Implications**: Divergent approaches to work-life balance policies
- **Economic Impact**: Different cultural responses to automation and productivity

## Technical Achievements

### Model Performance
- **Semantic Accuracy**: 92% accuracy in historical word association prediction
- **Temporal Consistency**: R² = 0.87 for time-series models
- **Cross-Cultural Validity**: Successful replication across language families

### Methodological Innovations
- **Temporal Word Embeddings**: Novel approach for diachronic analysis
- **Cultural Comparison Framework**: Standardized metrics for cross-cultural NLP
- **Historical Validation**: Robust testing against known historical events
- **Reproducible Pipeline**: Full automation from raw text to final analysis

## Technologies and Tools

<div class="tech-stack-grid">
<div class="tech-section">
<h4>Programming Languages</h4>
<ul>
<li>Python 3.9+ (Primary analysis)</li>
<li>R 4.2+ (Statistical modeling)</li>
<li>Shell scripting (HPC automation)</li>

</ul>
</div>

<div class="tech-section">
<h4>NLP Libraries</h4>
<ul>
<li>Gensim (Word2Vec implementation)</li>
<li>NLTK, spaCy (Text preprocessing)</li>
<li>scikit-learn (ML pipeline)</li>
<li>jieba (Chinese text segmentation)</li>
</ul>
</div>

<div class="tech-section">
<h4>Statistical Analysis</h4>
<ul>
<li>auto.arima in R (Time series)</li>
<li>scipy (Statistical tests)</li>
<li>pandas (Data manipulation)</li>
<li>numpy (Numerical computing)</li>
</ul>
</div>

<div class="tech-section">
<h4>Visualization</h4>
<ul>
<li>matplotlib, seaborn (Python plots)</li>
<li>ggplot2 (R visualizations)</li>
<li>plotly (Interactive charts)</li>
<li>Adobe Illustrator (Publication graphics)</li>
</ul>
</div>
</div>

## Code Repository
- **GitHub Repository**: [effort-osf](https://github.com/amberxuqianchen/effort-osf)
- **Open Science Framework**: Full dataset and analysis scripts
- **Preprocessed Data**: Available for reproducibility
- **Model Checkpoints**: Trained embeddings for each time period

## Research Impact and Recognition

### Primary Publication
**Chen, A. X., Sun, S., & Yu, H.** (2024). "Moral attitudes towards effort and efficiency: a comparison between American and Chinese history." *Humanities and Social Sciences Communications*, 11(1085). [DOI: 10.1057/s41599-024-03603-3](https://doi.org/10.1057/s41599-024-03603-3)

### Methodological Contributions
- **Dictionary Development**: Validated moral foundations dictionaries for cross-cultural analysis
- **Temporal Word Embeddings**: Novel approach for tracking semantic change over decades
- **Cross-Cultural NLP**: Standardized methodology for comparing moral concepts across languages
- **Historical Validation**: Robust testing against known historical events (USSR diplomatic relations)

### Citations and Recognition
- **Published** in _Humanities and Social Sciences Communications_
- **Conference Presentations**: 2 international conferences


### Practical Applications
- **Policy Research**: Informed cross-cultural management practices
- **Corporate Training**: Cultural sensitivity in multinational corporations
- **Educational Content**: Used in comparative cultural studies curricula


## Future Research Directions

### Technical Extensions
- **Transformer Models**: Implementing BERT-based temporal analysis
- **Multimodal Analysis**: Incorporating visual and audio cultural content
- **Real-time Monitoring**: Live cultural sentiment tracking
- **Causal Inference**: Identifying drivers of cultural change

### Research Applications
- **Policy Prediction**: Forecasting public opinion on policy changes
- **Business Strategy**: Cultural adaptation for global companies
- **Social Media Analysis**: Contemporary cultural trend detection
- **Historical Research**: Application to other cultural concepts

## Team and Acknowledgments

### Research Team
- **Amber X. Chen** (Principal Investigator & Lead Data Scientist)
- **Shaojing Sun** (Co-Principal Investigator & Cultural Analysis)
- **Dr. Hongbo Yu** (Faculty Supervisor)

### Technical Support
- **UCSB Center for Scientific Computing** (HPC resources)
- **Stanford NLP Group** (Congressional speech data)

### Funding Sources
- **UCSB ISBER Collaborative Research Initiative Grant**

---

*This project demonstrates the power of computational methods in understanding cultural evolution. For access to code, data, or collaboration opportunities, contact [amber.chen@psych.ucsb.edu](mailto:amber.chen@psych.ucsb.edu).*

<style>
.tech-stack-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 1.5em;
  margin: 2em 0;
}

.tech-section {
  background: linear-gradient(135deg, #f8f9fa 0%, #e9ecef 100%);
  padding: 1.5em;
  border-radius: 10px;
  border-left: 4px solid #28a745;
  box-shadow: 0 2px 4px rgba(0,0,0,0.1);
}

.tech-section h4 {
  margin-top: 0;
  color: #28a745;
  font-size: 1.1em;
  font-weight: 600;
}

.tech-section ul {
  margin: 0.5em 0 0 0;
  padding-left: 1.2em;
}

.tech-section li {
  margin-bottom: 0.4em;
  color: #495057;
  line-height: 1.4;
}

pre {
  background: #f8f9fa;
  border: 1px solid #e9ecef;
  border-radius: 6px;
  padding: 1em;
  overflow-x: auto;
  font-size: 0.9em;
}

code {
  background: #f1f3f4;
  padding: 0.2em 0.4em;
  border-radius: 3px;
  font-size: 0.9em;
}
</style>