# 📊 Customer Churn Prediction Using Behavioral Analysis

## 📝 Project Overview

Customer Churn Prediction Using Behavioral Analysis is an AI-assisted web analytics platform designed to help users understand customer behavior and identify patterns associated with churn.

The system allows users to upload customer datasets and supporting documentation, perform automated data profiling and preprocessing, explore statistical patterns, generate context-aware business insights using Google Gemini, and visualize relationships between customer features.

The platform combines data processing, Exploratory Data Analysis (EDA), Generative AI, and interactive visualization into a unified workflow, making customer analytics more accessible to both technical and non-technical users.

> **Note:** The current implementation focuses on behavioral analysis, data preprocessing, EDA, AI-driven insights, and visualization. Integration of trained machine learning models for real-time churn prediction is planned as a future enhancement.

---

## 🎯 Key Features

- 📂 **Multi-Format Data Ingestion**
  - Supports CSV, JSON, XLSX, and PDF files.
  - Converts uploaded data into standardized formats for analysis.
  - Extracts textual information from supporting documentation.

- 🔍 **Automated Dataset Profiling**
  - Generates automated EDA reports using `ydata-profiling`.
  - Analyzes data types, missing values, distributions, and correlations.
  - Uses caching to avoid unnecessary report regeneration.

- 🧹 **Interactive Data Preprocessing**
  - Detects missing values.
  - Supports mean, median, mode, interpolation, forward-fill, and backward-fill strategies.
  - Applies appropriate handling strategies for numerical and categorical data.

- 🤖 **AI-Driven Business Insights**
  - Uses Google Gemini to analyze dataset documentation and metadata.
  - Generates context-aware churn-related insights.
  - Identifies relationships between relevant customer attributes.

- 📈 **Dynamic Visualization**
  - Automatically classifies numerical and categorical features.
  - Recommends suitable visualization types based on feature combinations.
  - Generates charts such as histograms, scatter plots, heatmaps, and categorical visualizations.

- 👁️ **Vision AI Relationship Analysis**
  - Uses Gemini's multimodal capabilities to analyze generated visualizations.
  - Determines whether relationships between features are strong, weak, or absent.
  - Provides human-readable explanations of detected relationships.

- ⚡ **FastAPI Backend**
  - Modular REST API architecture.
  - Supports asynchronous processing.
  - Handles API errors and external Gemini API rate limits.
  - Provides generated visualization files through API endpoints.

- 🖥️ **Interactive React Dashboard**
  - Provides a responsive web-based interface.
  - Allows users to upload datasets and documentation.
  - Displays dataset summaries, EDA results, AI-generated insights, and visualizations.

---

## ⚙️ System Workflow

```text
User Uploads Dataset + Documentation
                ↓
       Data Ingestion Layer
                ↓
      Dataset Profiling / EDA
                ↓
       Data Preprocessing
                ↓
     Metadata & Context Analysis
                ↓
       Google Gemini API
                ↓
     Business Insight Generation
                ↓
      Visualization Recommendation
                ↓
       Chart Generation
                ↓
       Vision AI Analysis
                ↓
     Insights + Visualizations
                ↓
          React Dashboard
