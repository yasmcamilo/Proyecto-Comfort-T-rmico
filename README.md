# Proyecto-Comfort-T-rmico
Sistema de confort térmico basado en Arduino Mega 2560 con control de temperatura, humedad y PMV, validación RFID, y gestión de estados mediante una máquina de estados finitos.

# Sistema de Confort Térmico con RFID y Máquina de Estados

## Descripción general
Este proyecto implementa un **sistema de confort térmico** basado en **Arduino Mega 2560**, que permite **controlar y monitorear el ambiente térmico** de acuerdo con el índice de confort PMV (Predicted Mean Vote).  
El sistema realiza la **validación de acceso mediante tarjetas y llaveros RFID**, muestra información en pantalla LCD, y gestiona alarmas, ventilador, servo y señales luminosas a través de una **máquina de estados finitos**.

## Características principales
- **Validación RFID**: identifica a los usuarios mediante tarjeta y llavero.  
- **Control térmico**: sensores DHT11 y NTC para temperatura y humedad.  
- **Máquina de estados**: gestiona los modos de inicio, configuración, monitoreo, alarma y confort térmico (PMV alto/bajo).  
- **Interfaz LCD y teclado matricial (Keypad)** para interacción con el usuario.  
- **Sistema de alarma visual y sonora** con LED RGB y buzzer.  
- **Ventilador y servomotor** activados automáticamente según el PMV.  
- **Almacenamiento en EEPROM** de los datos del usuario y sus preferencias de temperatura.  
- **Documentación automática** generada con **Doxygen**.

## Componentes utilizados
| Componente | Descripción |
|-------------|-------------|
| Arduino Mega 2560 | Microcontrolador principal |
| Sensor DHT11 | Medición de temperatura y humedad |
| Sensor NTC analógico | Soporte adicional de temperatura radiante |
| Módulo RFID RC522 | Lectura de tarjetas y llaveros |
| LCD 16x2 | Interfaz visual para el usuario |
| Keypad 4x4 | Ingreso de clave y control manual |
| Potenciómetro | Control de contraste del LCD |
| LED RGB | Indicador de estados y alarmas |
| Buzzer activo | Señal de alarma sonora |
| Ventilador + Relay | Control de enfriamiento |
| Servomotor | Control de apertura mecánica |
| Protoboard y fuente | Ensamble y alimentación |


## Estructura del proyecto
El proyecto se compone de dos archivos principales:

1. **Confort_Termico.ino**  
   - Código principal del sistema con la máquina de estados.  
   - Control de sensores, actuadores y lógica de confort térmico.

2. **GuardarDatosTAGRFID.ino**  
   - Script auxiliar para grabar el nombre del usuario y su temperatura preferida en la tarjeta o llavero RFID.

## Documentación técnica
La documentación completa fue generada con **Doxygen**, incluyendo:
- Descripción detallada de funciones, variables y clases.
- Diagramas de dependencias y jerarquías.
- Navegación por módulos y archivos.  

Se encuentra en la carpeta:
```
/doc/html/index.html
```

## Evidencia en video
Puedes visualizar la demostración del sistema en funcionamiento en el siguiente enlace:  
[Ver video de evidencia](https://drive.google.com/file/d/1kWO-LGuVo3j3tjFcgR2cpi4Vd6uw_uBH/view?usp=sharing)


## Autores y créditos
**Yasley Mayerly Camilo Camilo y Jhon Breisman Quenguan Cuayca**  
Ingenieros de Sistemas en formación.  
Proyecto académico de arquitectura computacional.

## Licencia
Este proyecto está disponible bajo la licencia **MIT**, lo que permite su uso y modificación con fines educativos y de investigación.
