# NLP-based Literature Review of Aging-in-Place and Smart Home Health Technologies
Topic modeling analysis of 250+ research papers on smart home and Ambient Assisted Living (AAL) technologies for older adults. This repository explores major research themes using LDA and BERTopic to identify gaps related to user acceptance, privacy, and dashboard design.

A corpus of approximately 250 academic papers related to smart homes, AAL systems, and aging-in-place technologies was analyzed using Latent Dirichlet Allocation (LDA).

The analysis aims to answer questions such as:

- What major research themes exist in the smart home / AAL literature?
- Which areas are most heavily studied?
- Where might research gaps exist, particularly regarding older adults’ perspectives, technology acceptance, and privacy concerns?


# Dataset 
The dataset consists of approximately 250 research papers related to:

- Smart home technologies
- Ambient Assisted Living (AAL)
- AgeTech
- Remote health monitoring
- Aging in place
- Assistive technologies for older adults

For each paper, the following information was collected:
- Title
- Abstract

Titles and abstracts were combined into a single document for topic modeling.


# Methods
## Preprocessing 
The following preprocessing steps were applied:

- Lowercasing text
- Removing punctuation and numbers
- Removing stopwords
- Phrase normalization (e.g., smart home, older adults, activity recognition)
- Removing duplicate titles

The title and abstract were combined into a single document for analysis.

## Topic Modelling with Latent Dirichlet Allocation (LDA) 
After several rounds of hyperparameter tuning for optimal results, the key parameters were decided to be as the following: 
- max_features = 1000
- ngram_range = (1, 2)
- min_df = 3
- max_df = 0.6
- n_topics = 5

Each paper was assigned a dominant topic, allowing papers to be grouped into thematic clusters. 

## Key Findings 
The analysis revealed several major themes within the literature:

1. Ambient Assisted Living system infrastructure --> 
Development of smart home platforms, IoT frameworks, and monitoring architectures.

2. Sensor-based activity recognition and monitoring --> 
Machine learning systems detecting daily activities, falls, and behavioral patterns.

3. Health interventions using smart home technologies --> 
Applications related to nutrition monitoring, loneliness detection, and health promotion.

4. Technology acceptance and adoption among older adults --> 
Studies examining trust, perceived usefulness, and behavioral intentions toward smart home systems.

5. Care ecosystems and aging-in-place support --> 
Smart home systems supporting caregivers, dementia care, and independent living.

Overall, the results suggest that technical system development and sensing technologies dominate the literature, while comparatively fewer studies focus on older adults’ perceptions, trust, and adoption of smart home technologies. Such results influenced me into deciding my MSc thesis topic to be about technology acceptance and trust, where I develop smart home dashboards that are more accepted among older adults. 


