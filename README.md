```mermaid
flowchart TD
    A[Data Preparation] --> B[Short-Arc Signal Decomposition]
    B --> C[Feature Engineering]
    C --> D[Environmental Correlation]
    D --> E[ML Clustering & Classification]
    E --> F[Comparative Diagnostics]
    F --> G[Interpretation & Validation]

    subgraph A1
        A1a[InSAR time series (LOS or vert/horiz)]
        A1b[Rainfall & Temperature rasters]
        A1c[Land-cover, Geology & DEM]
        A1d[Failure vs. intact labels]
        A1a --> A
        A1b --> A
        A1c --> A
        A1d --> A
    end

    subgraph B1[Short-Arc Decomp]
        B1a[Model library: trend, step, breakpoint, seasonal]
        B1b[Test statistic → best model]
        B1c[Extract τ, rates, residuals]
        B1a --> B1b --> B1c
        B1c --> B
    end

    subgraph C1[Feature Eng.]
        C1a[One-hot model type]
        C1b[Rainfall & temperature lag features]
        C1c[Seasonal coeff & residual var]
        C1d[Landcover, geology & slope]
        C1a & C1b & C1c & C1d --> C
    end

    subgraph D1[Env. Correlation]
        D1a[Lagged cross-corr (rain, temp)]
        D1b[GAM fits]
        D1a & D1b --> D
    end

    subgraph E1[ML]
        E1a[UMAP + clustering]
        E1b[RF classifier: failure vs. intact]
        E1c[SHAP importances]
        E1a & E1b & E1c --> E
    end

    subgraph F1[Diagnostics]
        F1a[Metrics: τ-lag, accel, seasonal amp]
        F1b[Mann–Whitney U tests]
        F1a & F1b --> F
    end

    subgraph G1[Validation]
        G1a[Spatial maps & cluster plots]
        G1b[Statistical tests summary]
        G1c[Expert review]
        G1a & G1b & G1c --> G
    end
