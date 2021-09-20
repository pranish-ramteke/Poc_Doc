# poc_doc

A diagnosis and treatment suggestion, Machine learning based Flutter application.

## Getting Started

![alt text](https://github.com/pranish-ramteke/Poc_Doc/blob/master/assets/PocDoc_bg.png "Poc-Doc")

User can input symptoms and answer follow-up questions via text or speech and get a diagnosis instantly.
Uses BioBERT for diagnosis and suggesting a treatment plan.
Chained multiple machine learning models.

Bert is fantastic for encoding medical questions and answers, and developing robust vector representations of those questions/answers.

We trained a fine-tuned version of our model which was initialized with Naver's bioBert. We also trained a version where the bioBert weights were frozen, and only trained the two FCNNs for the questions and answers. While we expected the fine-tuned version to work well, we were surprised at how robust later was. This suggests that bioBert has innate capabilities in being able to encode the means of medical questions and answers.
