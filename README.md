
# RSI Crossover Strategy: Detección de Señales de Compra y Venta

## Descripción
Este repositorio contiene un programa en Python diseñado para detectar señales de compra y venta en precios simulados utilizando el **Relative Strength Index (RSI)**. El código implementa una estrategia basada en el cruce de dos RSI: uno rápido (14 periodos) y uno lento (30 periodos). Además, presenta visualizaciones claras con señales únicas de compra y venta en gráficos que incluyen tanto el precio como el RSI.

## ¿Qué es el RSI?
El **Relative Strength Index (RSI)** es un indicador técnico que mide la fuerza relativa de los movimientos de precios en un periodo determinado. Se expresa en una escala de 0 a 100:

- **Por encima de 70**: El activo está considerado sobrecomprado (posible momento para vender).
- **Por debajo de 30**: El activo está considerado sobrevendido (posible momento para comprar).

En esta implementación, se utilizan dos RSI de diferentes periodos para identificar cruces y generar señales.

## Características del Programa
- **Cálculo del RSI**: Genera dos indicadores RSI (rápido y lento) para un conjunto de precios.
- **Generación de señales**: Detecta cruces entre el RSI rápido y el lento para identificar zonas de compra y venta.
- **Visualización**:
  - Un gráfico del precio con flechas verdes (compra) y rojas (venta) que se muestran solo en los momentos clave.
  - Un gráfico del RSI con líneas de sobrecompra (70) y sobreventa (30) para mayor contexto.

## Instalación
### Prerrequisitos
1. **Python 3.7 o superior**.
2. Las siguientes librerías de Python:
   - `pandas`
   - `numpy`
   - `matplotlib`

Puedes instalar las librerías necesarias con:
```bash
pip install pandas numpy matplotlib
```

### Clonación del Repositorio
Clona este repositorio en tu máquina local:
```bash
git clone https://github.com/tu_usuario/rsi-crossover.git
cd rsi-crossover
```

## Uso
1. Ejecuta el archivo principal `rsi_crossover.py`:
   ```bash
   python rsi_crossover.py
   ```
2. Observa los resultados:
   - Un gráfico que muestra el precio con las señales de compra y venta.
   - Un gráfico que muestra los valores del RSI rápido y lento, junto con las líneas de sobrecompra y sobreventa.

## Estructura del Código
- **`calculate_rsi`**: Calcula el RSI para una serie de datos y un periodo especificado.
- **Detección de transiciones**: Identifica los cruces entre el RSI rápido y el lento para generar señales únicas.
- **Visualización**: Crea dos gráficos claros y detallados que incluyen el precio, las señales y los valores del RSI.

## Ejemplo de Gráficos
### Gráfico del Precio
- **Flecha verde**: Indica el inicio de una zona de compra.
- **Flecha roja**: Indica el inicio de una zona de venta.

### Gráfico del RSI
- Muestra los valores del RSI rápido y lento, junto con líneas de referencia de sobrecompra y sobreventa.

## Mejora Potencial
1. **Datos Reales**:
   - Adaptar el programa para trabajar con datos reales obtenidos de una API (por ejemplo, Alpha Vantage, Binance o Yahoo Finance).
2. **Optimización de Parámetros**:
   - Permitir ajustar dinámicamente los periodos del RSI y los niveles de sobrecompra/sobreventa.
3. **Integración de Estrategias**:
   - Combinar el RSI con otros indicadores técnicos como medias móviles o MACD para mejorar la fiabilidad de las señales.
4. **Backtesting**:
   - Implementar una función de backtesting para evaluar la rentabilidad de la estrategia en un historial de precios.
5. **Optimización del Código**:
   - Hacer uso de operaciones vectorizadas para mejorar la eficiencia.

## Contribuciones
Contribuciones, informes de errores y solicitudes de nuevas características son bienvenidos. Por favor, abre un issue o envía un pull request.



## Contacto
Si tienes preguntas o comentarios, no dudes en ponerte en contacto:
- **Autor**: Gabriel Giuffrida
- **Correo**: gabrielgiu19@gmail.com
- **LinkedIn**: www.linkedin.com/in/gabriel-giuffrida

