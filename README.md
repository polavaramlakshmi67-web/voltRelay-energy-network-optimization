# VoltRelay Energy — Data-Driven Network Optimization

## Project Overview

This project focuses on **data-driven network optimization for VoltRelay Energy**, a battery-swapping network serving gig and logistics riders across major Indian cities.

The objective was to identify the major causes of service failures, understand operational patterns, analyze battery and infrastructure performance, and provide actionable recommendations.

## Objectives

- Analyze battery-swap service failures
- Identify high-failure cities and stations
- Compare charger-generation performance
- Analyze battery health and retirement patterns
- Identify battery lot-level quality signals
- Provide data-driven operational recommendations

## Data

The analysis used multiple datasets covering:

- Swap events
- Stations
- Batteries
- Riders
- Telemetry
- Support data

The analysis included nearly **3 million usable swap events**.

## Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Google Colab
- SQL
- Data Visualization

## Key Insights

### 1. Service Reliability Deteriorated Sharply in Mid-2024

The network normally operated around **4.2–4.4% failure**, but failures increased to **12.39% in May 2024**.

The largest contributors were **failed-no-charged-battery** and **abandoned queue** events.

### 2. The Problem Is Geographically Concentrated

Failure rates varied across cities:

| City | Failure Rate |
|---|---:|
| Jaipur | 6.40% |
| Delhi NCR | 5.98% |
| Bengaluru | ~4.45% |
| Mumbai | ~4.45% |

This indicates that reliability issues should be investigated at the **city and station level**.

### 3. Gen1 Infrastructure Shows Weaker Reliability

Gen1 stations recorded a **5.91% failure rate**, compared with:

- Gen2: **4.58%**
- Gen3: **4.42%**

Gen1 also showed lower charged-battery availability and longer average charging times.

### 4. Battery Retirement Is Heavily Concentrated in Kyron

Kyron batteries recorded an **87.79% retirement rate**, compared with **0% for Amptek and Cellora** in the analyzed data.

Kyron's current average State of Health (SOH) was **63.75%**, compared with approximately **81%** for the other two suppliers.

### 5. Kyron's Issue Is Concentrated in Specific Lots

The strongest concentration was observed in:

- **KY-2407**
- **KY-240
