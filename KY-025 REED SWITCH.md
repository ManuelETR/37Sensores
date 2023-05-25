## KY-025 REED SWITCH
Informacion 

Qué es? Este KY-025 es un módulo de interruptor magnético que funciona como conmutador para detectar un campo magnético y actuar en consecuencia. Además permite configurar la sensibilidad del mismo, ya que sus contactos normalmente abiertos se cierran en la presencia de un campo magnético, por ello este módulo se puede usar para el control de gran cantidad de sistemas.

¿Para qué sirve?

El KY-025 Interruptor por Campo Magnético es un módulo que se puede usar para el control de interruptores, fotocopiadoras, lavadoras, refrigeradores, cámaras, puertas, ventanas, relés electromagnéticos, pesaje electrónico, medidor de nivel, medidor de gas, medidor de agua entre otras áreas de desarrollo.

## CÓDIGO
```python
from machine import Pin
import time

ReedSensor = Pin(18, Pin.IN)
while True:
    value = ReedSensor.value()
    print(value, end = " ")
    if value == 0:
        print("Sin Campo Magnetico")
    else:
        print("Campo Magnetico")
    time.sleep(0.5)
```
    
    
    
## PRUEBAS
![KY-025 REED SWITCH](https://github.com/ManuelETR/37Sensores/assets/60374861/6b6f2e2e-530d-400c-a783-4574c8be22ac)
