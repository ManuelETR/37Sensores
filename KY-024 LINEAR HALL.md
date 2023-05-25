# KY-024 LINEAR HALL

INFORMACIÓN 

Qué es? El módulo KY-024 Sensor de Campo Magnético Lineal se activa cuando detecta un campo magnético proveniente de un imán natural o de algún material ferromagnético, sus principales partes son un potenciometro para ajustar la sensibilidad y un sensor de Efecto Hall Lineal . Así mismo en su salida los da como resultado señales analógicas y digitales.

El sensor de campo magnético se compone de un circuito integrado 49E, comparador voltaje LM393, dos leds, seis resistencias y un header macho de ángulo de 4 pines.

¿Para qué sirve? Una aplicación típica del Sensor de Campo Magnético KY-024 es que se puede utilizar para el realizar el cálculo de la velocidad de un mecanismo en rotación o como un interruptor de proximidad. También hay sensores de tipo interruptor, que están limitados a solo intervenir para alcanzar un umbral de intensidad (ver KY003) y, por lo tanto, proporcionan solo un estado de encendido / apagado de salida.

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

## Imagen

![KY-024 Hall Sensor](https://github.com/ManuelETR/37Sensores/assets/60374861/507bab10-55b0-43da-ad92-fb83b259040d)
