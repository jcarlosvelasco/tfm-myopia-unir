# Categorización de los errores de refracción del ojo humano a partir del análisis de datos biométricos, mediante algoritmos predictivos. / Categorization of refractive errors in the human eye based on the analysis of biometric data using predictive algorithms.

*[English version below](#english-version)*

## Versión Español

### Descripción del Proyecto

Este Trabajo Fin de Máster (TFM) desarrolla un sistema computacional para analizar la miopía desde una perspectiva estructural del ojo humano. Utilizando un modelo físico basado en el esquema óptico de Le Grand y redes neuronales informadas por la física (PINNs), el proyecto busca categorizar los errores de refracción a partir de parámetros biométricos oculares.

### Objetivos Principales

- **Implementación de modelo físico-computacional**: Basado en el modelo óptico de Le Grand para calcular el error refractivo teórico
- **Desarrollo de PINNs**: Redes neuronales que integran conocimiento físico para predecir estructuras oculares y dioptrías
- **Análisis de agrupamiento**: Identificación de perfiles estructurales diferenciados de miopía
- **Interpretabilidad médica**: Uso de técnicas SHAP para explicar las decisiones del modelo

### Metodología

#### Modelo Físico de Le Grand
- Cálculo de potencia dióptrica total del ojo
- Estimación del error refractivo basado en parámetros biométricos
- Generación de etiquetas sintéticas para entrenamiento

#### Redes Neuronales Informadas por la Física (PINNs)
- **Enfoque 1**: Predicción de estructuras oculares (AXL, LENS, Paq, RaK, ACD) a partir de dioptrías
- **Enfoque 2**: Predicción de dioptrías a partir de parámetros biométricos

#### Función de Pérdida Híbrida
```
L_total = λ_data × L_data + λ_physics × L_physics
```

### Datos Utilizados

- **Fuente**: Pacientes reales del Hospital Universitario de Burgos
- **Tamaño**: ~1000 pacientes
- **Variables**: Parámetros biométricos oculares obtenidos mediante biómetro
- **Tipo**: Pacientes pre-operatorios para implantación de lentes intraoculares

### Tecnologías Utilizadas

- **Python 3.12**
- **TensorFlow/Keras**: Implementación de PINNs
- **SHAP**: Interpretabilidad de modelos
- **Scikit-learn**: Métricas y validación
- **Pandas/NumPy**: Manipulación de datos
- **Matplotlib/Seaborn**: Visualización

### Autores

- Juan Carlos Velasco Sánchez
- Rubén Casal Ferrero  
- Manuel García González

**Director**: Rodrigo Gil-Merino y Rubio, Jesús Torres Pérez

**Universidad**: Universidad Internacional de la Rioja (UNIR)  
**Programa**: Máster en Inteligencia Artificial  
**Fecha**: Septiembre 2025

### Licencia

[MIT License](LICENSE)

---

## English Version

### Project Description

This Master's Thesis (TFM) develops a computational system to analyze myopia from a structural perspective of the human eye. Using a physical model based on Le Grand's optical scheme and Physics-Informed Neural Networks (PINNs), the project seeks to categorize refractive errors from ocular biometric parameters.

### Main Objectives

- **Physical-computational model implementation**: Based on Le Grand's optical model to calculate theoretical refractive error
- **PINNs development**: Neural networks integrating physical knowledge to predict ocular structures and diopters
- **Clustering analysis**: Identification of differentiated structural profiles of myopia
- **Medical interpretability**: Use of SHAP techniques to explain model decisions

### Methodology

#### Le Grand Physical Model
- Calculation of total dioptric power of the eye
- Refractive error estimation based on biometric parameters
- Generation of synthetic labels for training

#### Physics-Informed Neural Networks (PINNs)
- **Approach 1**: Prediction of ocular structures (AXL, LENS, Paq, RaK, ACD) from diopters
- **Approach 2**: Prediction of diopters from biometric parameters

#### Hybrid Loss Function
```
L_total = λ_data × L_data + λ_physics × L_physics
```

### Data Used

- **Source**: Real patients from University Hospital of Burgos
- **Size**: ~1000 patients
- **Variables**: Ocular biometric parameters obtained via biometer
- **Type**: Pre-operative patients for intraocular lens implantation

### Technologies Used

- **Python 3.12**
- **TensorFlow/Keras**: PINNs implementation
- **SHAP**: Model interpretability
- **Scikit-learn**: Metrics and validation
- **Pandas/NumPy**: Data manipulation
- **Matplotlib/Seaborn**: Visualization

### Authors

- Juan Carlos Velasco Sánchez
- Rubén Casal Ferrero  
- Manuel García González

**Director**: Rodrigo Gil-Merino y Rubio, Jesús Torres Pérez

**University**: International University of La Rioja (UNIR)  
**Program**: Master's in Artificial Intelligence  
**Date**: September 2025

### License

[MIT License](LICENSE)

---

### Citation

```bibtex
@mastersthesis{velasco2025myopia,
  title={Categorización de los errores de refracción del ojo humano a partir del análisis de datos biométricos, mediante algoritmos predictivos},
  author={Velasco Sánchez, Juan Carlos and Casal Ferrero, Rubén and García González, Manuel},
  year={2025},
  school={Universidad Internacional de la Rioja (UNIR)},
  type={Master's thesis}
}
```
