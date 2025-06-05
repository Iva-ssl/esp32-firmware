# ESP32 Firmware Repository

Este repositorio contiene el firmware OTA para Robot Balanceador ESP32.

## Estructura del Repositorio
```
esp32-firmware/
├── firmware/
│   ├── latest/         # Ultima version del firmware
│   │   └── BAL_02.bin
│   └── vX.X.X/         # Versiones anteriores
│       └── BAL_02.bin
├── version.txt         # Version actual del firmware
└── README.md           # Este archivo
```

## Como funciona

1. La ESP32 verifica `version.txt` para ver si hay nueva version
2. Si hay nueva version, descarga de `firmware/latest/BAL_02.bin`
3. Se actualiza y reinicia automaticamente

## Para actualizar

1. Compilar nueva version en ESP-IDF
2. Ejecutar `auto_update.bat` en el proyecto
3. Commit y Push con GitHub Desktop
4. Presionar BOOT en la ESP32

## Historial de versiones

- v1.0.0 - Version inicial
