# RiegoAutomatico
M5-Stack ESP32

# Proyecto de Riego Automático con ESP32 M5Stack

Este proyecto tiene como objetivo crear un sistema de riego automático utilizando el **ESP32 M5Stack**. El sistema utiliza un sensor de humedad para activar o desactivar un relé que controla el sistema de riego.

## Requisitos

- **Hardware**:
  - ESP32 M5Stack
  - Sensor de humedad (por ejemplo, DHT11 o similar)
  - Relé de 5V para controlar el sistema de riego
  - Cableado y componentes básicos

- **Software**:
  - **Visual Studio Code** (VS Code)
  - **PlatformIO IDE** (Extensión para VS Code)
  - **Arduino Framework** para ESP32

## Paso a Paso

### 1. Crear un nuevo Proyecto

1. Abre **Visual Studio Code** y asegúrate de tener instalada la extensión **PlatformIO IDE**.
2. Haz clic en **Create New Project** en la pantalla de inicio de PlatformIO.

   ![Create New Project](images/create_new_project.png)

3. En la ventana emergente:
   - **Project Name**: Escribe un nombre para tu proyecto (por ejemplo, **RiegoAutomático**).
   - **Board**: Selecciona **M5Stack-Core-ESP32** (es la placa que estás utilizando).
   - **Framework**: Selecciona **Arduino** (es más sencillo y compatible con la mayoría de las librerías).
   
   Haz clic en **Finish**. PlatformIO creará un proyecto en una nueva carpeta.

### 2. Abrir el Proyecto

1. En el menú de la izquierda de Visual Studio Code, podrás ver la estructura del proyecto. Asegúrate de que esté seleccionado el directorio correcto donde se creó el proyecto.

### 3. Configurar las Librerías

1. Abre el archivo **`platformio.ini`** que se encuentra en la raíz del proyecto.
2. Añade las librerías necesarias para el proyecto. Por ejemplo, si estás utilizando un sensor de humedad, añade la librería correspondiente:

   ```ini
   lib_deps = 
     DHT sensor library
     Adafruit Unified Sensor

