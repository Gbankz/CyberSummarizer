# CyberSummarizer

**A Lightweight Domain-Optimized Text Summarization System for Cybersecurity Documentation**

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Hugging Face](https://img.shields.io/badge/Hugging%20Face-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)

## Overview

CyberSummarizer is a lightweight, CPU-friendly text summarization system designed specifically for cybersecurity logs, threat reports, and technical documentation. It combines semantic embeddings, custom entity recognition, and hybrid summarization techniques to produce accurate, domain-aware summaries while preserving critical security entities (CVEs, IPs, IOCs, etc.).

This project was developed as part of my Master's research in Computer Science at Rivers State University.

## Features

- **Domain-specific entity recognition** (CVEs, IP addresses, malware names, hashes, etc.)
- **Hybrid summarization**: Extractive (TextRank) + Abstractive (DistilBART)
- **Lightweight models**: DistilBERT + DistilBART (optimized for CPU)
- **Streamlit web interface** for easy interaction
- **Evaluation metrics**: ROUGE scores + Entity Preservation
- Low memory footprint (~1.18 GB)

## Key Results

- **ROUGE-1**: 0.6847 (+5.3% over baseline)
- **Entity Preservation**: 91%
- **Average Processing Time**: 2.70 seconds per document
- **Memory Usage**: 1.18 GB (26% less than heavier models)

## Technologies Used

- Python
- Hugging Face Transformers (DistilBERT, DistilBART)
- spaCy + Regex for NER
- TextRank (extractive)
- Streamlit (UI)
- MySQL (optional storage)

## Project Structure
