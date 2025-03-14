# Low-Resource Machine Translation (EN-VI)

## **Project Overview**
This project focuses on **Machine Translation (MT)**, aiming to automatically translate text from one natural language to another. A key challenge in MT is handling **low-resource scenarios**, where limited bilingual data is available for model training. In this case, we aim to improve translation models using only **20,000 bilingual sentence pairs** for English-Vietnamese translation.

## **Approach**
To address the low-resource challenge, we adopt two main strategies:

1. **Pre-trained Models**  
   - Utilize state-of-the-art pre-trained models such as **mBART50** and **T5**, which are based on the Transformer architecture with stacked layers.  
   - These models are highly effective for low-resource translation tasks due to their multilingual capabilities.

2. **Data Augmentation Techniques**  
   - Collect additional bilingual data to expand the training dataset.  
   - Apply semi-supervised learning techniques to enhance model performance.

Among these, pre-trained models like **mBART50** demonstrate superior performance in low-resource translation scenarios.

## **Dataset**
The project uses the **IWSLT'15 English-Vietnamese dataset**, which includes:  
- Training set: 133,317 bilingual sentence pairs  
- Validation set: 1,553 bilingual sentence pairs  
- Test set: 1,269 bilingual sentence pairs  

The translation direction is **English-to-Vietnamese (EN-VI)**.

## **Evaluation Metric**
The model's performance is evaluated using the **SacréBLEU (BLEU)** metric, a standard for assessing translation quality.

## **Model Training**
We fine-tune the **mBART50 model**, pre-trained on 50 languages, for the EN-VI translation task. This model is particularly well-suited for this use case due to its multilingual training and robust architecture.

## **Key Features**
- Focus on low-resource machine translation.
- Use of advanced pre-trained models (mBART50 and T5).
- Application of data augmentation and semi-supervised techniques.
- Evaluation based on BLEU scores for quality assessment.
