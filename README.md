# Tasador Digital de Viviendas: Análisis Inmobiliario Predictivo

## Descripción del Proyecto
Este proyecto desarrolla un modelo de aprendizaje automático para predecir el precio de venta de propiedades inmobiliarias. A través de un proceso de Ciencia de Datos de principio a fin, transformamos datos crudos en una herramienta de tasación precisa, capaz de identificar las variables que realmente impactan el valor de mercado.

## Estructura del Notebook
El flujo de trabajo se divide en 6 fases estratégicas:

1. **Validación de errores:** Análisis exploratorio inicial, detección de nulos, sesgos y multicolinealidad.
2. **Tratamiento de nulos:** Imputación inteligente diferenciando entre "ausencia de característica" y "datos faltantes".
3. **Tratamiento de Outliers:** Filtrado de anomalías críticas (ej. grandes áreas con precios bajos) para mejorar la estabilidad del modelo.
4. **Transformación de la variable objetivo:** Aplicación de logaritmo para normalizar la distribución de `SalePrice`.
5. **Limpieza general:** Codificación de variables categóricas, eliminación de redundancias y ajuste de tipos de datos.
6. **Verificación:** Auditoría final de integridad, asegurando un dataset limpio y listo para el entrenamiento.

## Fase de Modelado (Fase 5)
Comparamos dos algoritmos de ensamble:
* **Random Forest Regressor:** Modelo de promediado para reducir varianza.
* **Gradient Boosting Regressor:** Modelo secuencial enfocado en la corrección de errores, obteniendo el mejor desempeño.

## Ingeniería de Variables Destacadas
* `TotalSF`: Área habitable total (sótano + niveles superiores).
* `HouseAge`: Antigüedad de la propiedad al momento de la venta.
* `TotalBathrooms`: Conteo consolidado de baños completos y medios.

## Tecnologías Utilizadas
* Python (Pandas, NumPy, Scikit-Learn)
* Seaborn & Matplotlib (Visualización)
* Técnicas: One-Hot Encoding, Log-Transformation, Feature Engineering.

---
*Desarrollado por: Juan Esteban Hernández y Santiago Andrés Pineda.*
