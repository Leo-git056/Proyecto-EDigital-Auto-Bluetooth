# 🚗 Auto RC con Bluetooth – PIC16F877A

Proyecto académico que consiste en la modernización de un auto a control remoto tradicional con cable, transformándolo en un vehículo inalámbrico controlado desde un teléfono celular mediante Bluetooth.

El sistema utiliza un **PIC16F877A** como unidad de control y una aplicación móvil desarrollada específicamente para este proyecto.

---

## 📌 Descripción del Proyecto

El objetivo fue reemplazar el sistema de control por cable de un auto RC convencional por un sistema inalámbrico basado en Bluetooth, permitiendo su manejo desde un smartphone Android.

El proyecto integra:

- 🔹 Microcontrolador **PIC16F877A**
- 🔹 Módulo Bluetooth (HC-05 / HC-06)
- 🔹 Control de motores DC mediante puente H
- 🔹 Aplicación móvil desarrollada a medida
- 🔹 Comunicación serial UART

---

## 🧠 Arquitectura del Sistema
Teléfono Android
│
Bluetooth
│
Módulo HC-05
│
UART (Serial)
│
PIC16F877A
│
Control de motores (Puente H)
│
Auto RC

---

## 📱 Aplicación Móvil

La aplicación Android fue desarrollada para:

- Conectar / Desconectar el módulo Bluetooth
- Enviar comandos de movimiento:
  - ⬆ Avanzar
  - ⬇ Retroceder
  - ⬅ Izquierda
  - ➡ Derecha
  - ⏹ Detener
- Seleccionar niveles de velocidad:
  - 25%
  - 50%
  - 100%
 
    

La comunicación se realiza mediante el envío de caracteres específicos por UART al microcontrolador.

---

## ⚙️ Funcionamiento

1. El usuario conecta la aplicación al módulo Bluetooth.
2. La app envía comandos mediante comunicación serial.
3. El PIC16F877A recibe los datos por UART.
4. Según el comando recibido:
   - Activa los motores correspondientes.
   - Controla la dirección del vehículo.
   - Ajusta la velocidad mediante PWM.

---

## 🛠 Tecnologías Utilizadas

### Hardware

- PIC16F877A
- Módulo Bluetooth HC-05 / HC-06
- Puente H para control de motores
- Motores DC
- Fuente de alimentación

### Software

- Lenguaje C (firmware del microcontrolador)
- MPLAB (IDE de desarrollo)
- Aplicación Android (MIT App Inventor / Android Studio)
- Comunicación UART

---

## 🎯 Objetivos Académicos

- Implementar comunicación serial UART.
- Controlar motores mediante PWM.
- Integrar hardware y software en un sistema embebido.
- Diseñar una aplicación móvil para control remoto.
- Aplicar conceptos de electrónica digital y microcontroladores.

---

## 🚀 Posibles Mejoras

- Implementar control proporcional de velocidad.
- Agregar sensores (ultrasonido, IR) para detección de obstáculos.
- Agregar telemetría (nivel de batería).
- Migrar a microcontrolador con mayor capacidad (STM32 / ESP32).

---

## 👨‍💻 Autor

**Leonardo Sánchez**  
Estudiante de Ingeniería en Computación  

---

## 📄 Licencia

Este proyecto fue desarrollado con fines académicos.
