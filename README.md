SpecLens AI: A Data-Driven Smartphone Decision Support System
Project Overview

SpecLens AI is a data-driven decision support system designed to help users choose smartphones through structured analysis of real-world specifications.

Rather than relying on brand popularity or sponsored rankings, the system compares devices using measurable technical attributes such as price, performance, battery, display, and connectivity. The project emphasizes data quality, feature integrity, and system design to build a reliable foundation for recommendation and decision logic.

Motivation

Smartphone data available online is often inconsistent in format, incomplete, or heavily influenced by marketing language. This project addresses these issues by:

Preserving raw data as the source of truth

Creating cleaned, purpose-specific datasets

Separating analytical logic from UI-oriented information

The objective is not to predict trends, but to support informed and transparent decision-making.

Dataset Summary

Scale: 1,268 unique smartphone models

Depth: 65+ raw specification attributes

Source: Real-world smartphone specification pages

Attributes: Pricing, availability, hardware, software, and connectivity

Key challenges handled

Inconsistent price formats and currency normalization

Missing or partial specifications across brands

Platform-specific availability (Amazon, Flipkart, official stores)

Variant-level noise in model naming and configurations

Project Structure and Design

The project follows a strict separation of concerns to ensure clarity and scalability:

Raw Data
Preserved without modification for traceability.

Analytical / ML-Ready Data
Cleaned and normalized features used for EDA and recommendation logic.

UI-Oriented Metadata
Links, images, and display-focused fields isolated from analytical features to prevent feature leakage.

This structure allows the system to evolve without redesigning core logic.

Development Stages
Stage 1: Data Acquisition & Engineering

Status: In Progress

Focus: Building a reliable data foundation.

Completed work:

Normalization of price-related fields

Standardization of launch dates

Binary availability flags for Amazon, Flipkart, and official stores

Conversion of specification strings into structured numeric formats

Stable identifier strategy using model_id

Version-controlled development with granular, meaningful commits

Stage 2: Exploratory Data Analysis (EDA)

Status: Planned

Focus:

Price vs. performance trends

Brand-wise feature distribution

Hardware and connectivity patterns

Stage 3: Recommendation Logic

Status: Planned

Focus:

Similarity-based recommendation using distance and scoring metrics

Ranking driven by user requirements rather than popularity signals

Stage 4: Interface & Interaction Layer

Status: Planned

Focus:

Web-based interface

Explainable recommendation outputs

Clear separation between logic and presentation

Design Principles

Data integrity over forced completeness
Missing values are treated as meaningful signals, not errors.

Decision support, not blind recommendation
The system is designed to explain technical trade-offs.

Static but scalable design
Current implementation is static, while supporting future incremental updates.

Tech Stack (Current)

Language: Python

Libraries: Pandas, NumPy

Environment: Jupyter Notebook, Google Colab

Version Control: Git & GitHub

Project Status

This is an active and evolving project.
The current priority is building a correct, explainable, and ML-ready data foundation before introducing modeling or user-facing components.
