# LLaMA: Open And Efficient Foundation Language Models
[Touvron et al. 2023](https://arxiv.org/pdf/2302.13971)

## 1. Introduction
- Determining optimal model size/training length tradeoff  with objective prioritizing inference cost (instead of training cost, as emphasized in Chinchilla) 
- Training set - only public data, "compatible with open sourcing"
- Modified architecture? 
## 2. Approach
- Pretraining Data
    - Common Crawl - did some preprocessing? Wikipedia classification thing? I guess for favoring reliable/professional sites? Reliability filtering emphasis
    - Other reliable/coding-related public datasets
    - 1.4T tokens
- Architecture
    - SwiGLU activations?
    - Rotary Embeddings (GPTNeo)
- Training implementation
    - Some handcoded training optimizations
## 3. Results
- 65 B model beats GPT3 and Palm in some reasoning/reading comprehension tasks
- Comparable/beats PALM at math, coding tasks