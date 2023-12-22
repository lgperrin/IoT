# Práctica de _Edge Computing_

## Objetivos

Los objetivos que se persiguen son:

* Implementar un sistema que adquiera y procese muestras de voz, partiendo de la señal proporcionada por el micrófono SPM1423 y presente en el módulo M5 Stick C Plus.
* Desarrollar y transferir al procesador ESP32 una red neuronal convolucional que sirva para reconocer diferentes comandos de control hablados.

## Flujo de Trabajo

1. Seleccionar y grabar comandos de voz
2. Implementar CNN
3. Implementar sistema completo en M5 Stick C Plus


## Material necesario

- [x] Visual Studio
- [x] Arduino IDE
- [x] Dispositivo M5 Stick C Plus

## Comandos de voz elegidos

| Comando de Voz | Descripción                                |
|----------------|--------------------------------------------|
| Encender       | Activa un dispositivo o sistema            |
| Apagar         | Desactiva un dispositivo o sistema         |
| Pausar         | Detiene temporalmente un dispositivo o sistema |
| Cancelar       | Detiene una acción o comando en curso      |
| Silenciar      | Desactiva el sonido del dispositivo        |


## Funciones implementadas

| Nombre del Método  | Descripción |
|--------------------|-------------|
| Importar Librerías | Carga las librerías necesarias como TensorFlow, librosa, NumPy, y herramientas de Keras y scikit-learn. |
| preprocess_audio   | Carga y procesa un archivo de audio, convirtiéndolo en un espectrograma. |
| create_model       | Define y compila un modelo de red neuronal convolucional para el procesamiento de audio. |
| train_model        | Entrena el modelo de red neuronal con datos de entrenamiento. |
| hyperparameter_search | Realiza una búsqueda de hiperparámetros para optimizar el modelo. |
| convert_to_tflite  | Convierte el modelo entrenado a formato TensorFlow Lite para su uso en dispositivos móviles o integrados. |
