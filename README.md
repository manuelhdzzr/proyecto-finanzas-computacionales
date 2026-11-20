# Optimización de Carteras con Predicción de Retornos (Random Forest / KNN + Markowitz)

Proyecto Final Integrador – CO-2067-3 Finanzas Computacionales – Opción 2.

Autor: Manuel Hernández Rivera – Matrícula 669394

## Descripción
Se predice el retorno diario de 6 acciones (AAPL, MSFT, AMZN, GOOGL, JPM, XOM) con Random Forest y KNN, se compara contra un modelo base, se valida con el test de Diebold-Mariano y se construyen carteras con la Frontera Eficiente de Markowitz (máximo Sharpe), evaluadas con Sharpe y Sortino frente a una cartera de pesos iguales.

## Contenido
- `proyecto_finanzas_opcion2.ipynb` – notebook completo (datos, features, modelos, métricas, Diebold-Mariano, carteras).
- `Informe_Tecnico_Finanzas.pdf` – informe técnico.
- `metricas_modelos.csv`, `diebold_mariano.csv`, `metricas_carteras.csv`, `hiperparametros.csv` – resultados.
- `matrices_confusion.png`, `carteras_acumulado.png`, `frontera_eficiente.png` – gráficas.

## Cómo ejecutarlo
1. Abrir el notebook en Google Colab.
2. Entorno de ejecución → Ejecutar todo (tarda ~3–5 min). Requiere internet (yfinance).

## Resultados principales
- Ningún modelo supera significativamente al modelo base (Diebold-Mariano, p > 0.05).
- Markowitz + KNN obtuvo el mayor Sharpe (1.084) vs. cartera igualitaria (0.936); Markowitz + Random Forest quedó en 0.774.

## Librerías
pandas, numpy, scikit-learn, scipy, matplotlib, yfinance. Semilla fija = 42.
