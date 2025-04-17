# Metatrader Analytics

## 🔹 Overview 
This repository contains a Python-based tool for comprehensive analysis of MetaTrader 5 trading accounts. The project provides advanced statistical metrics, performance visualization, for traders seeking to optimize their strategies through data-driven insights.

## 🔹 Features
- Secure login into MT5 accounts
- Advanced statistical analysis of trade operations
- Real-time and historical profit/loss tracking
- Aggregated results by symbol, day of week, hour, and session
- Drawdown, Sharpe ratio, recovery factor and expectancy metrics
- Consistency and accuracy analysis

## 🔹 Tech Stack

- Python 3.10+
- MetaTrader5 (official MT5 Python API)
- `logging` for internal audit and debugging

## 🔹 Project Structure

```
platform_metatrader/
├── LICENSE
├── README.md
├── requirements.txt
├── setup.py
├── docs/                    # Project documentation (architecture, design decisions, how-to guides, etc.)
│   └── index.md
├── platform_metatrader/     # The core package
│   ├── __init__.py
│   ├── config.py            # Centralized configuration (e.g. logging, constants)
│   ├── auth.py              # Contains the MT5Authenticator class
│   ├── collector.py         # Contains the MT5DataCollector class
│   ├── analytics.py         # Contains MT5Analytics and OperationAnalyzer classes
│   ├── service.py           # Contains MT5Service that orchestrates the interactions
│   ├── graph.py             # Contains MT5GraphGenerator and related plotting functions
│   └── report.py            # Contains PDFGenerator and ReportCompiler classes 
└── tests/                   # Unit/integration tests for your modules
    ├── __init__.py
    ├── test_auth.py
    ├── test_collector.py
    ├── test_analytics.py
    └── test_service.py

```
