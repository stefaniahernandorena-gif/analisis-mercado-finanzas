# Análisis de Mercado: Sector Tecnológico (AAPL) vs. Criptoactivos (BTC)

Este repositorio contiene la **Primera Entrega** del proyecto de Data Science, enfocado en la obtención de insights reales a partir de la visualización y el cruce de datos financieros.

---

## Abstracto y Motivación
El ecosistema financiero actual ha integrado los criptoactivos como una pieza clave de las carteras de inversión. Este análisis surge de la necesidad de entender si activos digitales como **Bitcoin (BTC)** se comportan de manera independiente, o si su movimiento está atado al rendimiento de las acciones del sector tecnológico tradicional, representado por **Apple (AAPL)**. 

**Audiencia:** Gerentes de fondos de inversión, analistas de riesgo y pequeños inversores que buscan diversificar su portafolio basándose en datos y no en suposiciones.

---

## Hipótesis de Trabajo (Preguntas de Negocio)
Para guiar el análisis, nos propusimos responder las siguientes interrogantes:

1. **Correlación de Mercados:** ¿Existe una relación directa y positiva entre el movimiento de precios de Bitcoin y las acciones de Apple?
2. **Análisis de Riesgo:** ¿Es la volatilidad diaria de las criptomonedas significativamente mayor a la de las acciones tecnológicas líderes?
3. **Validación de Movimientos:** ¿Los saltos de precio bruscos en Bitcoin están respaldados por un volumen real de transacciones o son fluctuaciones aisladas?

---

## Metodología y Origen de los Datos
Para garantizar la transparencia y reproducibilidad del análisis, se utilizaron fuentes de datos en tiempo real mediante Python:
* **API de CoinGecko:** Extracción de precios históricos y volúmenes de **Bitcoin**.
* **Yahoo Finance (`yfinance`):** Obtención de datos del mercado bursátil para **Apple Inc**.
* **Procesamiento:** Se realizó un *Inner Join* para unificar los calendarios de ambos mercados, eliminando días no hábiles y normalizando las zonas horarias.

  ---

## Principales Hallazgos (Insights)
A partir de las visualizaciones generadas en el Notebook, obtuvimos las siguientes conclusiones:

* **Independencia de Activos:** Se rechazó la hipótesis de una correlación fuerte entre BTC y AAPL. Esto confirma que combinar ambos activos es una estrategia efectiva para la **diversificación de carteras**, ya que no suelen caer al mismo tiempo.
* **Confirmación de Riesgo:** El análisis de volatilidad (Boxplot) demostró que Bitcoin presenta una fluctuación diaria un **39% mayor** que Apple. Esto define a BTC como un activo para perfiles de inversión agresivos.
* **Respaldo de Movimientos:** Los datos de volumen confirmaron que los saltos de precio mayores al 10% en Bitcoin coinciden con los picos máximos de transacciones, validando que son **movimientos de mercado reales** y no fluctuaciones vacías.

---

## Estructura del Proyecto
El repositorio se organiza de la siguiente manera para facilitar su revisión:

1.  **`notebook.ipynb`**: Código en Python con la limpieza, transformación y visualización de datos.
2.  **`dataset_mercado_btc_aapl.csv`**: El dataset final consolidado y listo para ser utilizado.
3.  **`presentacion_insights.pdf`**: Documento ejecutivo con el resumen visual y conclusiones de negocio.

  **Proyecto desarrollado para la Primera Entrega de la cursada de Data Science.**
*Hernandorena, Stefanía Micaela*

* **Yahoo Finance (`yfinance`):** Obtención de datos del mercado bursátil para **Apple Inc**.
* **Procesamiento:** Se realizó un *Inner Join* para unificar los calendarios de ambos mercados, eliminando días no hábiles y normalizando las zonas horarias.
