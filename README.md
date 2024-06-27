# SPRINT 11: Evaluación de Impacto del Cambio de Fuentes en una Aplicación

## Descripción del Proyecto

En este proyecto, evaluamos el impacto de un cambio de fuentes en una aplicación móvil mediante un experimento A/A/B. El objetivo es determinar si el cambio de fuentes afecta el comportamiento del usuario en términos de interacción con diferentes pantallas de la aplicación.

## Objetivos del Proyecto

- Evaluar la consistencia de los grupos de control (A/A) en el experimento.
- Determinar el impacto del cambio de fuentes (grupo B) en el comportamiento del usuario.
- Proveer recomendaciones basadas en los resultados del experimento.

## Pasos Realizados en el Proyecto

### Paso 1: Descarga y Preparación de los Datos

- **Archivos de Datos:**
  - Datos sobre eventos de usuarios en la aplicación móvil.
  
- **Preparación de Datos:**
  - Cargamos los datos en DataFrames de pandas.
  - Revisamos y optimizamos los tipos de datos.
  - Filtramos y limpiamos los datos para análisis posteriores.

### Paso 2: Análisis de Consistencia entre Grupos de Control

- **Métricas Analizadas:**
  - Proporción de usuarios que realizaron el evento `MainScreenAppear` en los grupos de control (246 y 247).
  - Comparación de los resultados entre los grupos de control para asegurar la consistencia del diseño experimental.

- **Resultados:**
  - No se encontraron diferencias significativas entre los grupos de control, validando la consistencia del diseño experimental.

### Paso 3: Análisis del Impacto del Cambio de Fuentes

- **Eventos Analizados:**
  - `MainScreenAppear`
  - `OffersScreenAppear`
  - `CartScreenAppear`
  - `PaymentScreenSuccessful`

- **Métricas Analizadas:**
  - Proporción de usuarios que realizaron cada evento en el grupo de prueba (248) y en los grupos de control (246 y 247).
  - Comparación de los resultados entre el grupo de prueba y los grupos de control.

- **Resultados:**
  - No se encontraron diferencias significativas en la proporción de usuarios que realizaron los eventos analizados entre el grupo de prueba y los grupos de control.
  - Se utilizó la corrección de Bonferroni para ajustar el nivel de significación y asegurar la validez de los resultados.

### Paso 4: Conclusiones y Recomendaciones

- **Conclusiones:**
  - **Consistencia entre Grupos de Control:** La ausencia de diferencias significativas entre los grupos de control valida la metodología del experimento.
  - **Impacto del Cambio de Fuentes:** El cambio de fuentes no tuvo un impacto significativo en el comportamiento de los usuarios en términos de los eventos analizados.

- **Recomendaciones:**
  - **Implementar el Cambio de Fuentes:** Se puede proceder a implementar el cambio de fuentes en toda la aplicación, ya que no se encontraron impactos negativos significativos.
  - **Monitoreo Continuo:** Continuar monitoreando el comportamiento del usuario para asegurar que no haya efectos adversos a largo plazo.
  - **Pruebas Adicionales:** Realizar pruebas adicionales en otros aspectos del diseño de la aplicación para seguir optimizando la experiencia del usuario.

## Conclusión General del Proyecto

Este informe resume los hallazgos clave y proporciona recomendaciones basadas en un análisis exhaustivo de los datos de usuarios y los resultados del experimento A/A/B. La implementación cuidadosa y el monitoreo continuo ayudarán a asegurar una experiencia óptima para los usuarios de la aplicación.

## Contribución

Si deseas contribuir a este proyecto, realiza un fork del repositorio y crea una pull request con tus mejoras. Asegúrate de que tu código sigue los lineamientos del proyecto y está bien comentado.

## Licencia

Este proyecto está bajo la licencia MIT. Para más detalles, consulta el archivo LICENSE.
