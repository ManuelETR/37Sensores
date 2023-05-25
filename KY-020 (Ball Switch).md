# KY-020 Relay (Ball Switch)

## INFORMACIÓN 

Para el sensor de ball switch despliega resultados al momento de que el usuario agite el sensor una vez que se haya conectado a la Raspberry Pi Pico W; al igual que el sensor de inclinación literalmente lleva a cabo las mismas conexiones: señal, voltaje y tierra, por lo que para su elaboración no es nada complicado de realizar, y del lado del código se utilizan las mismas librerías (Pin y time).

## CÓDIGO
```python
from machine import Pin
import time

BallSensor = Pin(17, Pin.IN)

while True:
    value = BallSensor.value()
    print(value, end = " ")
    if  value== 0:
        print("The ball is moving...")
    else:
        print("The ball isn't moving...")
    time.sleep(0.1)
```

## Imagen
![KY-020](https://github.com/ManuelETR/37Sensores/assets/60374861/759985b2-73b7-4f5f-8446-029c3d69c3f8)

## Pruebas
