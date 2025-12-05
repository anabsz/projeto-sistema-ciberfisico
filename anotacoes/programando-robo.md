# Anotações da programação do robô
[Documentação da Hiwonder](https://docs.hiwonder.com/projects/MasterPi/en/latest/docs/6.motion_control_course.html#)

## Códigos e suas explicações
Código base para execução do robô
```python
#!/usr/bin/python3
# coding=utf8
import sys
sys.path.append('/etc/MasterPi/')
import time
import signal
import HiwonderSDK.mecanum as mecanum

if sys.version_info.major == 2:
    print("Use o python3 para executar esse programa")
    sys.exit(0)

chassis = mecanum.MecanumChassis()
start = True

def stop(signum, frame):
    global start
    start = False
    print("Parando...")
    chassis.set_velocity(0, 0, 0,)
signal.signal(signal.SIGINT, stop)

if __name__ == "__main__":
    while start:
        chassis.set_velocity(50, 90, 0) # set_velocity(motor_speed, car_direction, rotation_speed)
        time.sleep(1)
        print("Andando...")
    chassis.set_velocity(0, 0, 0)
    print("Parou")

```

### chassis.set_velocity()
- Primeiro parâmentro: velocidade do motor
- Segundo parâmentro: direção do carro
  - 90°: para frente
  - 180°: para esquerda
  - 270°: para trás
- Terceiro parâmetro: sentido das rodas (horário/antihorário)