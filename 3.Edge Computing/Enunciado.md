# Práctica de _Edge Computing_

## Objetivos

Los objetivos que se persiguen son:

1. Implementar un sistema que adquiera y procese muestras de voz, partiendo de la señal proporcionada por el micrófono SPM1423 y presente en el módulo M5 Stick C Plus. 
2. Desarrollar y transferir al procesador ESP32 una red neuronal convolucional que sirva para reconocer diferentes comandos de control hablados.

## Flujo de Trabajo

```mermaid
flowchart LR
    id1[Seleccionar y 
        grabar comandos 
        de voz]

    id2[Implementar CNN]
    id3[Implementar sistema
        completo en M5 Stick C Plus]

    id1 --> id2 --> id3
```

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
