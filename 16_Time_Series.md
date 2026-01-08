```
Time-Series Models
│
├── State-Space Models
│   │
│   ├── Structural Time-Series Models
│   │   │
│   │   ├── Trend Models
│   │   │   │
│   │   │   ├── Deterministic Trend
│   │   │   ├── Local Level
│   │   │   └── Local Linear Trend
│   │   │
│   │   ├── Seasonal Models
│   │   │   │
│   │   │   ├── Deterministic Seasonality
│   │   │   └── Stochastic Seasonality
│   │   │
│   │   ├── Trend + Seasonality Models
│   │   │   │
│   │   │   ├── Local Level + Seasonal
│   │   │   └── Local Linear Trend + Seasonal
│   │   │
│   │   ├── Cyclical Models
│   │   │
│   │   ├── Intervention / Structural Break Models
│   │   │
│   │   ├── Regression-Based Structural Models
│   │   │   │
│   │   │   ├── Static Regression
│   │   │   └── Time-Varying Regression
│   │   │
│   │   └── Bayesian Structural Time-Series (BSTS)
│   │
│   └── Other State-Space Models
│       │
│       ├── ARIMA (state-space form)
│       ├── Dynamic Factor Models
│       └── Hidden Markov Models
│
└── Non-State-Space Time-Series Models
    │
    ├── ETS (Exponential Smoothing)
    ├── Machine Learning Models
    └── Deep Learning Models

```
    
#### How to Read This Hierarchy
- State-Space Models are the big umbrella
- Structural models are a subset focused on interpretation
- Trend, seasonality, cycles, and regressions are building blocks
- Most real models are combinations of these blocks

| Real-World Problem                 | Model in Hierarchy            |
| ---------------------------------- | ----------------------------- |
| Monthly sales with changing growth | Local Linear Trend + Seasonal |
| Policy change impact               | Intervention + Regression     |
| Economic indicators                | Cyclical Structural Model     |
| Marketing impact over time         | Time-Varying Regression       |
| Causal impact analysis             | BSTS                          |
