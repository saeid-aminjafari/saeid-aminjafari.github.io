```mermaid
flowchart TD
  A[Data Preparation] --> B[Short-Arc Signal Decomposition]
  B --> C[Feature Engineering]
  C --> D[Environmental Correlation]
  D --> E[ML Clustering & Classification]
  E --> F[Comparative Diagnostics]
  F --> G[Interpretation & Validation]

  subgraph A1 [ ]
    A1a[InSAR time series (LOS or vert/horiz)]
    A1b[Rainfall, Temperature rasters]
    A1c[Land-cover, Geology, DEM]
    A1d[Failure vs. intact labels]
    A1a --> A
    A1b --> A
    A1c --> A
    A1d --> A
  end

  subgraph B1 [Short-Arc Decomp]
    B1a[Model library: trend, step, breakpoint, seasonal]
    B1b[Test statistic → best model]
    B1c[Extract τ, rates, residuals]
    B1a --> B1b --> B1c
    B1c --> B
  end

  subgraph C1 [Feature Eng.]
    C1a[One-hot model type]
    C1b[Rainfall lag features]
    C1c[Temp & seasonal coeffs]
    C1d[Static features: landcover, geology, slope]
    C1a & C1b & C1c & C1d --> C
  end

  subgraph D1 [Env Corr.]
    D1a[Lagged cross-corr (rain, temp)]
    D1b[GAM fits]
    D1a & D1b --> D
  end

  subgraph E1 [ML]
    E1a[UMAP + clustering → patterns]
    E1b[RF classifier: failure vs. intact]
    E1c[SHAP feature importances]
    E1a & E1b & E1c --> E
  end

  subgraph F1 [Diagnostics]
    F1a[Tabulate τ-lags, accel, seasonal amp]
    F1b[Statistical tests vs. peers]
    F1a & F1b --> F
  end

  subgraph G1 [Validation]
    G1a[Spatial maps]
    G1b[Mann–Whitney U]
    G1c[Expert review]
    G1a & G1b & G1c --> G
  end

