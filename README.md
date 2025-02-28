# Final Project Report: Financial Question Answering with RAG and LLMs
Competition Link: https://tbrain.trendmicro.com.tw/Competitions/Details/37
This repository contains our final project report for AI CUP 2024 Yushan Artificial Intelligence Open Challenge. Our project focuses on leveraging advanced AI techniques—specifically, Retrieval-Augmented Generation (RAG) and Large Language Models (LLMs)—to address financial question answering. The system we developed is designed to identify and retrieve the most relevant document numbers from a collection of PDF documents that span three categories: insurance, finance, and FAQ.

## Project Overview

- **Objective:**  
  Build a system that, given a financial query, can accurately retrieve relevant document numbers from a set of PDF documents. This is achieved by combining deep learning, robust OCR, and advanced text retrieval methods.

- **Challenges:**  
  - Financial documents often include complex tables, financial symbols, and mixed-format content that make traditional text processing difficult.
  - Enhancing text understanding for finance documents required specialized pre-processing techniques to clean and structure the OCR output.

- **Approach:**  
  - **Pre-Processing & Feature Engineering:**  
    - **OCR & Summarization:** Use Google OCR for text extraction and ChatGPT to refine and summarize the extracted text.
    - **Context Cleaning:** Apply regular expressions, word segmentation (using CKIP Tagger), and n-gram techniques to improve text quality.
  - **Model Training & Retrieval:**  
    - Implement statistical methods (BM25 and TF-IDF) for initial text retrieval.
    - Develop a deep learning pipeline using a RAG-based approach (incorporating bert-base-chinese and OpenAI embeddings) to capture semantic relationships and improve document relevance.
  - **Experimental Results:**  
    - Through extensive experiments across insurance, finance, and FAQ datasets, our RAG-based approach achieved a final accuracy of 0.8836.
  - **Competition Strategy:**  
    - We adopt a multi-model output comparison strategy to select the most reliable retrieval results.

## Report Contents

- **Introduction & Problem Description:**  
  Overview of the financial question answering challenge and the unique difficulties of processing finance documents.
- **Related Works:**  
  Reviews of BM25, LLMs, RAG, BERT, and OCR technologies as applied to financial document analysis.
- **Methodology:**  
  Detailed explanation of our pre-processing pipeline, feature engineering, and model training methods.
- **Experiments and Results:**  
  Comparative evaluation of different approaches and their performance across document categories.
- **Discussions and Future Works:**  
  Analysis of the challenges encountered, lessons learned, and directions for further improvement.
- **Group Contributions:**  
  Breakdown of each team member’s role in data preprocessing, feature engineering, model training, documentation, and presentation.

For a complete and detailed explanation—including mathematical formulations, pseudocode, experimental results, and further discussions—please refer to the attached PDF report: [Final Project Report.pdf](Final Project Report.pdf).
