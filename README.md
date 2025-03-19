# Cryptocurrency Trading Bot

A comprehensive automated trading system for cryptocurrency markets, built with Python and machine learning.

## Overview

This project implements an AI-driven cryptocurrency trading bot that uses machine learning algorithms to analyze market data, generate trading signals, and execute trades on the Binance exchange. The system is designed with a modular architecture that separates data collection, feature engineering, model training, signal generation, and trading execution.

## Key Components

### Data Collection
- **Historical Data**: Download historical klines (OHLCV) data from Binance
- **Real-time Data**: Collect live market data through WebSocket connections
- **Order Book Data**: Capture market depth information for enhanced analysis

### Feature Engineering
- Generate technical indicators and custom features from price data
- Support for various feature types including rolling statistics, technical indicators, and custom metrics
- Extensible framework for adding new feature generators

### Machine Learning
- Train models to predict price movements using various algorithms:
  - Gradient Boosting
  - Neural Networks
  - Support Vector Machines
  - Logistic Regression
- Evaluate model performance with metrics like AUC, precision, and recall

### Signal Generation
- Convert model predictions into actionable trading signals
- Configurable thresholds and rules for signal generation
- Backtesting framework to optimize signal parameters

### Trading Execution
- Connect to Binance API for order execution
- Support for limit and market orders
- Position management and risk control

### Notifications
- Telegram integration for trade alerts and performance updates
- Score notifications for significant prediction changes
- Visual charts of price action and prediction 

## Configuration

The system is highly configurable through JSON configuration files. Key settings include:

- Exchange API credentials
- Trading pairs and timeframes
- Feature generation parameters
- Model selection and hyperparameters
- Signal thresholds and trading rules
- Notification preferences

## Workflow

1. **Data Collection**: Gather historical and real-time market data
2. **Feature Generation**: Create features from raw market data
3. **Model Training**: Train ML models on historical data
4. **Signal Generation**: Apply models to generate trading signals
5. **Trade Execution**: Execute trades based on signals
6. **Monitoring**: Track performance and receive notifications