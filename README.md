![Typing SVG](https://readme-typing-svg.demolab.com/?lines=Working+on+it+right+now!&center=true&width=500&height=50)

# Automated Detection of Vulnerable Code Snippets in Open Source Repositories Using NLP

## Project Overview
Open-source software is extensively used across industries, but it can contain vulnerabilities that malicious actors can exploit. This project aims to develop an NLP-based system to automatically detect vulnerable code snippets in large open-source repositories, specifically focusing on platforms like GitHub. By leveraging datasets such as MUSE and Google BigQuery GitHub Data, alongside the CVE (Common Vulnerabilities and Exposures) database, we aim to create an early warning system that helps developers identify and address potential security issues.

## Features
- **Vulnerability Detection**: Automatically detects common vulnerabilities such as SQL injection, buffer overflow, and hard-coded credentials.
- **NLP Techniques**: Utilizes models like CodeBERT for vulnerability pattern detection in code comments, function names, and documentation.
- **Supervised Learning**: Employs models like SVM, Random Forest, LSTM, and CNN to classify code snippets as vulnerable or secure.
- **Named Entity Recognition (NER)**: Identifies sensitive data such as API keys and passwords embedded in code.
- **Contextual Analysis**: Uses transformer architectures to capture dependencies within code snippets for detecting subtle vulnerabilities.
- **Code Dependency Graphs**: Analyzes data flow through functions to flag insecure data handling.
- **API Call Analysis**: Flags potentially dangerous API calls and third-party libraries associated with vulnerabilities.

## Datasets
- **MUSE Dataset**: Contains various open-source software projects including code snippets, comments, and function names.
- **Google BigQuery GitHub Data**: Provides a vast pool of open-source repositories for analysis.
- **CVE Database**: Used for identifying and validating known vulnerabilities.
- **The Cybernative.ai**: Code Vulnerability and Security Dataset is a dataset of synthetic Data Programming by Demonstration (DPO) pairs, focusing on the intricate relationship between secure and insecure code across a variety of programming languages.

## How It Works
1. **Data Collection**: 
   - Collect data from open-source repositories using APIs and web scraping.
   - Use datasets like MUSE, Google BigQuery GitHub Data, and CVE to build a comprehensive training and validation dataset.
   
2. **NLP-Based Vulnerability Detection**: 
   - Preprocess text data by cleaning and tokenizing comments and function names.
   - Apply TF-IDF to highlight keywords linked to vulnerabilities.
   - Use CodeBERT to detect patterns indicative of security issues.

3. **Machine Learning Models**: 
   - Train SVM, Random Forest, LSTM, and CNN models for vulnerability classification.
   - Apply transformer architectures to capture code dependencies and analyze contextual vulnerability indicators.

4. **Feature Engineering**:
   - Generate code dependency graphs to visualize function-level data flow.
   - Perform API call analysis to flag potentially unsafe third-party library calls.

5. **Clustering Vulnerabilities**: 
   - Use K-means clustering to group vulnerabilities based on shared characteristics across different codebases.
