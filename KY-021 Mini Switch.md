## KY-021 Mini Switch

INFORMACIÓN
Este sensor funciona llevando a cabo una misma acción con el Reed Switch, el cual al captar un campo magnético puede activar o desactivar circuitos de manera que podamos crear un circuito con condiciones como estas, en caso de detectar un campo magnético active un sensor y cuando no haya active otro.

## CÓDIGO
```python
from machine import Pin
import utime

pin=16
sensor=Pin(pin, Pin.IN)
utime.sleep(1)

while True:
    if sensor.value()==1:
        print("Switch Apagado")
        utime.sleep(1)    
    else:
        print("Switch Encendido")
        utime.sleep(1)
utime.sleep(1)
```

## Pruebas
![KY-021 MiniSwitch](https://github.com/ManuelETR/37Sensores/assets/60374861/cf26549d-bad3-4c47-a6bb-d0dbc29be51d)
