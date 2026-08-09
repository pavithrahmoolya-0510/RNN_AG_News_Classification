# AG News Classification using RNN Models

## Project Overview

This project performs text classification on the AG News dataset using recurrent neural network architectures.

## Models Used

- Simple RNN
- LSTM
- GRU
- Bi-LSTM

## Dataset

The AG News dataset contains news articles belonging to four categories.

## Preprocessing

The text data was processed using:

- Tokenization
- Vocabulary limitation
- Sequence conversion
- Padding
- Maximum sequence length of 100

## Model Comparison

| Model | Test Accuracy | Training Time |
|---|---:|---:|
| Simple RNN | 68.20% | 280.75 sec |
| LSTM | 89.83% | 535.55 sec |
| GRU | 91.00% | 459.12 sec |
| Bi-LSTM | 90.22% | 675.13 sec |

## Gradient Clipping

The LSTM was also evaluated with and without gradient clipping.

| Model | Test Accuracy | Training Time |
|---|---:|---:|
| LSTM Without Clipping | 90.895% | 406.24 sec |
| LSTM With Clipping | 91.000% | 450.35 sec |

## Result

The GRU achieved the highest test accuracy of 91.00% among the four main models.

## Project Structure

```text
RNN_AG_News_Classification/
│
├── RNN_AG_News_Classification.ipynb
├── model_comparison.csv
├── gradient_clipping_comparison.csv
├── README.md
├── .gitignore
└── plots/