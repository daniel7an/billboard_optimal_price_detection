# Optimal Price Detection for Billboard Rentals

This repository contains the code for an optimal price detection system developed during a Machine Learning Bootcamp project in 2024. The project aimed to help a fictional company, Bilboardly, maximize revenue from their 10,000 billboards distributed across the country.

## Overview

The system utilizes a combined neural network approach integrating LSTM and fully connected models to predict optimal prices for each billboard for the first week of 2024 based on historical data from 2013 to 2023. The provided dataset includes daily prices and booking ratios for each billboard over 10 years.

## Approach

1. **Data Preprocessing**: The historical data is preprocessed to prepare input-output pairs for training the neural network. `Daily prices are used as inputs for the LSTM model, while the fully connected model takes longitude, latitude, size, and light as features`.

2. **Model Training**: The neural network is trained using a combination of LSTM and fully connected layers to learn the relationship between daily prices and billboard features with booking ratios.

3. **Prediction**: Using benchmark data, the trained model predicts booking rates.

4. **Optimal Price Selection**: `We set different daily prices and multiply them with predicted booking ratios to calculate weekly revenue for each billboard. The daily price yielding the highest weekly revenue is detected as the optimal price for that billboard.`

