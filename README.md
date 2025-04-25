```mermaid
flowchart TD
  A[Data Preparation] --> B[Short-Arc Decomp]
  B --> C[Feature Eng]
  C --> D[Env Correlation]
  D --> E[ML and Clustering]
  E --> F[Diagnostics]
  F --> G[Validation]

  subgraph A1
    A1a[InSAR LOS vertical horizontal]
    A1b[Rainfall and Temperature]
    A1c[Landcover Geology DEM]
    A1d[Failure vs Intact Label]
  end
  A1a --> A
  A1b --> A
  A1c --> A
  A1d --> A

  subgraph B1[Short-Arc Decomp]
    B1a[Trend Step Breakpoint Seasonal]
    B1b[Test Stat Selection]
    B1c[Extract Tau Rates ResidVar]
  end
  B1a --> B1b --> B1c --> B

  subgraph C1[Feature Eng]
    C1a[ModelType OneHot]
    C1b[Rainfall and Temp Lag]
    C1c[Seasonal Coeff ResidVar]
    C1d[Landcover Geology Slope]
  end
  C1a & C1b & C1c & C1d --> C

  subgraph D1[Env Correlation]
    D1a[Lagged CrossCorr]
    D1b[GAM Fits]
  end
  D1a & D1b --> D

  subgraph E1[ML]
    E1a[UMAP Clustering]
    E1b[RF Classifier]
    E1c[SHAP Importances]
  end
  E1a & E1b & E1c --> E

  subgraph F1[Diagnostics]
    F1a[Metrics TauLag Accel Amp]
    F1b[MannWhitney Tests]
  end
  F1a & F1b --> F

  subgraph G1[Validation]
    G1a[Spatial Maps]
    G1b[Stats Summary]
    G1c[Expert Review]
  end
  G1a & G1b & G1c --> G
