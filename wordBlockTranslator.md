# Word Block Translator

# Motors
## - Run Motor for Duration
### - Base
![RMfD.b.png](./images/RMfD.b.png)
```python
motor = Motor('A')

motor.run_for_rotations(1, 75)
```
### - Multiple Motors
![RMfD.m.png](./images/RMfD.m.png)
```python
motor_pair = MotorPair('A', 'E')

motor_pair.move_tank(1, 'rotations', -75, 75)
```
### - Counterclockwise
![RMfD.c.png](./images/RMfD.c.png)
```python
motor = Motor('A')

motor.run_for_rotations(1, -75)
```
### - Degrees
![RMfD.d.png](./images/RMfD.d.png)
```python
motor = Motor('A')

motor.run_for_degrees(1, 75)
```
### - Seconds
![RMfD.s.png](./images/RMfD.s.png)
```python
motor = Motor('A')

motor.run_for_seconds(1, 75)
```
## - Motor Go to Position
### - Base
![MGtP.b.png](./images/MGtP.b.png)
```python
motor = Motor('A')

motor.run_to_position(0, 'shortest path')
```
### - Multiple Motors
![MGtP.m.png](./images/MGtP.m.png)
```python
motor_a = Motor('A')
motor_e = Motor('E')

motor_a.run_to_position(0, 'shortest path')
motor_e.run_to_position(0, 'shortest path')
```
### - Clockwise
![MGtP.c.png](./images/MGtP.c.png)
```python
motor = Motor('A')

motor.run_to_position(0, 'clockwise')
```
### - Counterclockwise
![MGtP.cc.png](./images/MGtP.cc.png)
```python
motor = Motor('A')

motor.run_to_position(0, 'counterclockwise')
```
## - Start Motor
### - Base
![SaM.b.png](./images/SaM.b.png)
```python
motor = Motor('A')

motor.start(75)
```
### - Multiple Motors
TODO: Check if start_tank or just start is correct  
![SaM.m.png](./images/SaM.m.png)
```python
motor_pair = MotorPair('A', 'E')

motor_pair.start_tank(75, -75)
```
### - Counterclockwise
![SaM.c.png](./images/SaM.c.png)
```python
motor = Motor('A')

motor.start(-75)
```
## - Stop Motor
### - Base
![SoM.b.png](./images/SoM.b.png)
```python
motor = Motor('A')

motor.stop()
```
### - Multiple Motors
![SoM.m.png](./images/SoM.m.png)
```python
motor_pair = MotorPair('A', 'E')

motor_pair.stop()
```
## - Set Motor Speed
### - Base
TODO: Check that this works  
![SMS.b.png](./images/SMS.b.png)
```python
motor = Motor('A')

motor.set_default_speed(75)
```
### - Multiple Motors
![SMS.m.png](./images/SMS.m.png)
```python
motor_pair = MotorPair('A', 'E')

motor_pair.set_default_speed(75)
```
## - Motor Position
![MP.png](./images/MP.png)
```python
motor = Motor('A')

motor.get_position()
```
## - Motor Speed
![MS.png](./images/MS.png)
```python
motor = Motor('A')

motor.get_speed()
```
# Movement
## - Move for Duration
## - Move with Steering for Duration
## - Start Moving with Steering
## - Stop Moving
## - Set Movement Speed
## - Set Movement Motors
## - Set 1 Motor Rotation to Distance Moved
# Light
# Sound
# Events
# Control
# Sensors
# Operators
# Variables
