# Proyecto de Análisis de Datos Educativos Mundiales

## Pasos Principales

### 1. Limpieza y Transformación en Python
- **Carga de datos:** Los datos fueron cargados desde un archivo CSV utilizando la biblioteca `pandas`.
- **Eliminación de duplicados:** Se eliminaron filas duplicadas para garantizar la calidad de los datos.
- **Manejo de valores nulos:** Se rellenaron valores nulos en algunas columnas específicas y se eliminaron filas con valores faltantes críticos.

### 2. Limpieza y Transformación en R
- **Transferencia de datos:** Los datos limpios de Python fueron exportados a un archivo CSV y luego cargados en R utilizando el paquete `dplyr`.
- **Filtrado:** Se eliminaron filas con valores faltantes en columnas importantes, como `lit_rate_adult_pct`.
- **Transformaciones:** Se creó una nueva columna calculada (`new_column`) basada en una transformación matemática de `lit_rate_adult_pct`.
- **Eliminación de duplicados:** Se aseguraron datos únicos en las filas restantes.

### 3. Integración de Python y R
- Se utilizó `reticulate` para interactuar entre Python y R, facilitando la transferencia de datos y el uso de bibliotecas específicas de cada entorno.

## Resultados
- **Indicadores clave:** 
  - Las tasas de alfabetización de adultos (`lit_rate_adult_pct`) se analizaron para identificar patrones relevantes.
  - Se creó una nueva métrica derivada que ayuda a explorar relaciones entre variables educativas.
- **Calidad de los datos:** Los datos finales son más consistentes y listos para análisis más profundos.

## Tecnologías Utilizadas
- **Python:** Pandas para limpieza inicial y exportación de datos.
- **R:** dplyr para manipulación avanzada y transformación de datos.
