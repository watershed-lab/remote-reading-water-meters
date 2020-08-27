## DEMOSTRACIÓN DE USO DE RED NEURONAL LSTM PARA PREDICCIÓN DE CONSUMOS INDIVIDUALES

Modelo didáctico que utiliza un modelo de aprendizaje profundo mediante una red neuronal LSTM para predecir consumos de un contador de agua.

Ejecutable en pc's domésticos. Recomendado i5 de 4 procesadores o superior y memoria RAM de 8Gb o superior.

Los datos reales de un contador se descomponen en componentes temporales para buscar patrones de repetición, determinando la estacionalidad de los consumos y los valores residuales.

Se normalizan los datos en el rango 0-1 y se formatean para su introducción como ventanas temporales en un modelo de red neruonal sencillo, con 3 capas LSTM y tres dropout.

El entrenamiento se realiza con reducción automática de la tasa de apendizaje, y muestra la reducción de las pérdidas durante su aprendizaje.

Para interpretar las predicciones se invierte el reescalado de los datos. Las métricas de calidad obtienen un error medio en torno al 3%... aunque las predicciones de consumo instantaneo para un cuarto de hora concreto no son tan fiables, debido al uso de un conjunto limitado de registros. Sin embargo, sí ajustan de manera efectiva las horas aproximadas de los consumos.

### Rutas para la ejecución

Los archivos con de cuaderno y las imágenes de prueba se deben ponerse en la carpeta de usuario.

