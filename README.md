# 🌟 Introduction to Vietnamese Transformer-based Question Answering
This project presents a fine-tuned implementation of the **XLM-RoBERTa** base model, which is a multilingual transformer-based language model trained on 100 languages from Hugging Face. The model is specifically fine-tuned for Vietnamese language question answering task.

# 💡 Model
The XLM-RoBERTa base model, a powerful multilingual transformer-based language model that has demonstrated exceptional performance in various natural language processing tasks, is utilized in the this project. It leverages a self-attention mechanism to capture long-range dependencies and acquire knowledge of complex relationships between words and sentences. The base model offers an optimal trade-off between performance and computational resources when compared to the larger XLM-RoBERTa model

# 📚 Training Data Sources
Despite the limited amount of training data, I was able to achieve promising results thanks to the power of the XLM-RoBERTa model. To fine-tune the model, I used a combination of translated datasets of question-answer pairs, as well as a Vietnamese text dataset released by Zalo AI Challenge 2022.

| Dataset | Description | Link |
| --- | --- | --- |
| Vietnamese XSquad | Question-answer pairs dataset released by DeepMind | [Link](https://raw.githubusercontent.com/deepmind/xquad/master/xquad.vi.json) |
| Bert-Vietnamese-Question-Answering | Vietnamese language dataset for question answering | [Link](https://raw.githubusercontent.com/mailong25/bert-vietnamese-question-answering/master/dataset/train-v2.0.json) |
| E2E Question Answering data | Vietnamese text dataset released by Zalo AI Challenge 2022 | [Link](https://www.kaggle.com/datasets/ducnh279/nlp-data) |

# ⚡Optimizing Fine-tuning Process
To optimize the fine-tuning process, I used several techniques, including automatic mixed precision, dynamic loss scaling, and parallelized data loading using multiprocessing.

# 📓 Notebooks
All the code for this project is available on Kaggle notebooks. You can find the notebooks at:

| Notebook | Link |
| --- | --- |
| Prepare dataset | [Link](https://www.kaggle.com/code/ducnh279/prep-qa-dataset) |
| Set-ups & fine-tuning | [Link](https://www.kaggle.com/code/ducnh279/qa-training) |  

# 📈 Results
Here are some examples of how the XLM-RoBERTa model can effectively answer questions in Vietnamese:
| Question | Context | Model Answer |
| --- | --- | --- |
| Elon Musk là người nước nào? | Elon Reeve Musk FRS (sinh ngày 28 tháng 6 năm 1971), là một kỹ sư, nhà tài phiệt, nhà phát minh, doanh nhân công nghệ và nhà từ thiện người Mỹ gốc Nam Phi. | người Mỹ gốc Nam Phi |
| Elon Musk sinh ngày bao nhiêu? | Elon Reeve Musk FRS (sinh ngày 28 tháng 6 năm 1971), là một kỹ sư, nhà tài phiệt, nhà phát minh, doanh nhân công nghệ và nhà từ thiện người Mỹ gốc Nam Phi. | ngày 28 tháng 6 năm 1971 |
| Em trai Elon tên là gì? | Elon Musk cùng với em trai, Kimbal, đồng sáng lập ra Zip2, một công ty phần mềm web và được hãng Compaq mua lại với giá 340 triệu USD vào năm 1999. | Kimbal |
| Hãng Compaq mua lại Zip2 với giá bao nhiêu? | Elon Musk cùng với em trai, Kimbal, đồng sáng lập ra Zip2, một công ty phần mềm web và được hãng Compaq mua lại với giá 340 triệu USD vào năm 1999. | 340 triệu USD |

# Conclusion
The aim of this project is to showcase the application of XLM-RoBERTa base model in Vietnamese language question answering. It is my sincere hope that this work may encourage other researchers to delve deeper into the possibilities of transformer-based models and multilingual models for natural language processing tasks.
