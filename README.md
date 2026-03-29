# 📊Rendimiento Sectorial Ajustado por Riesgo de Cola (Kurtosis)

## 📌Descripción del Proyecto

Este proyecto analiza el desempeño reciente de los sectores del mercado, ajustándolo por riesgo estadístico extremo (kurtosis). El objetivo es identificar sectores que ofrecen buen rendimiento sin asumir un riesgo elevado de eventos extremos, algo clave para la asignación de capital y la gestión de carteras.

A diferencia de los rankings tradicionales basados solo en retorno, este análisis incorpora la calidad del rendimiento, penalizando sectores donde las ganancias vienen acompañadas de distribuciones con colas peligrosas.

## 🎯Objetivo Analítico

Responder a la pregunta:
- ¿Qué sector ofrece el mejor rendimiento promedio en los últimos 7 días manteniendo un nivel de riesgo de cola controlado?

Esto permite detectar sectores atractivos desde una perspectiva riesgo–retorno, evitando rendimientos inflados por volatilidad extrema.

## 🧠Insight Clave

Un sector con:
- Alto rendimiento promedio
- Kurtosis moderada o baja

Es estadísticamente más robusto que uno con retornos similares pero alto riesgo de cola, donde una sola sesión extrema puede borrar semanas de ganancias.

## 🗂️ Fuentes de Datos

El análisis se construye a partir de tres tablas principales:
- tickers: información sectorial de cada activo
- precios_diarios: precios de apertura y cierre diarios
- indicadores_tecnicos: métricas de riesgo como la kurtosis

## ⚙️Metodología

- Ventana temporal

- Últimos 7 días de datos disponibles.

- Cálculo por acción

- Rendimiento promedio diario:

(𝐶𝑙𝑜𝑠𝑒−𝑂𝑝𝑒𝑛)/𝑂𝑝𝑒𝑛

- Kurtosis promedio en el período.

- Agregación sectorial

- Promedio del rendimiento de las acciones del sector.

- Promedio de la kurtosis sectorial.

- Ranking final

- Sectores ordenados por rendimiento promedio ajustado por riesgo.

## 📈Métricas Calculadas

- Rendimiento Sectorial Promedio (%)
- Kurtosis Sectorial Promedio

Estas métricas permiten comparar sectores no solo por performance, sino también por estabilidad estadística.

## 💼Valor de Negocio

Este análisis es especialmente útil para:

📌 Asignación sectorial de carteras

📌 Rotación defensiva de capital

📌 Identificación de tendencias sostenibles

📌 Reducción del riesgo de eventos extremos

En contextos de alta incertidumbre, priorizar sectores con menor kurtosis puede marcar la diferencia entre una corrección manejable y una pérdida severa.

## 🧪Consideraciones

- La kurtosis no predice eventos, pero sí mide la probabilidad histórica de movimientos extremos.
- Resultados más confiables se obtienen con:
- Universos amplios de acciones por sector
- Datos limpios y consistentes

## 🚀Próximos Pasos (Opcional)

- Comparar contra el promedio de kurtosis del mercado
- Incorporar volatilidad (σ) para un ajuste tipo Sharpe más completo
- Analizar ventanas móviles para detectar cambios de régimen

## 👤Autora
Flavia Hepp Proyecto de SQL aplicó un análisis de riesgo basado en eventos.

***
📊 **No todo rendimiento alto es “bueno”… depende del riesgo oculto**

Algunos sectores destacan por sus retornos…
pero esconden un detalle clave: **riesgo de eventos extremos**.

👉 Analicé el rendimiento sectorial de los últimos 7 días, ajustándolo por **kurtosis** para identificar dónde el retorno es más “saludable”.

💡 **Insight clave:**
Hay sectores que logran **buen rendimiento promedio con menor riesgo de cola**, lo que los convierte en candidatos más robustos frente a shocks inesperados.

---

📈 **¿Qué medí?**

* Rendimiento promedio (7 días) por sector
* Kurtosis promedio (riesgo de eventos extremos)
* Comparación entre retorno y nivel de riesgo

---

🧠 **¿Cómo interpretarlo?**

* Alta kurtosis → mayor probabilidad de movimientos extremos
* Baja kurtosis → comportamiento más estable
* Alto retorno + baja kurtosis → **mejor calidad de rendimiento**

---

⚡ **¿Por qué importa?**

Porque no se trata solo de ganar…
sino de **evitar pérdidas extremas en el camino**.

Este enfoque permite:

* Identificar sectores más “defensivos”
* Construir portafolios más robustos
* Filtrar oportunidades con mejor perfil riesgo-retorno

---

📌 Pregunta para la comunidad:
¿Incorporan métricas de riesgo de cola en su análisis… o siguen priorizando volatilidad tradicional?

#QuantFinance #DataScience #RiskManagement #Trading #StockMarket #Analytics #MachineLearning #SQL

