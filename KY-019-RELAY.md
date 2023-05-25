# KY-019 Relay

INFORMACIÓN 
El Módulo Relevador 5V KY-019 es un dispositivo electrónico que permite controlar dispositivos que trabajen máximo 250V /15A y 125V/10A AC y 30V/10A DC por medio de una señal de control de 5V, señalizando su activación por medio de un LED indicador en su PCB.

El Módulo Relevador 5V KY-019 es utilizado en proyectos de IoT para controlar luces, contactos, electrodomésticos y otros dispositivos electrónicos. Comúnmente son usados en circuitos de control automático con una pequeña corriente de control y una gran corriente de operación.


## CÓDIGO
```python
from machine import Pin
import utime

relay = Pin(18,Pin.OUT)

while True:
    
    relay.value(1)
    utime.sleep(0.5)
    relay.value(0)
    utime.sleep(0.5)
```
## Pruebas
![KY-019 RELAY](https://github.com/OscarTec98/37Sensores/assets/60374861/6382e809-ceda-4926-96a4-b43a5aa59f39)
