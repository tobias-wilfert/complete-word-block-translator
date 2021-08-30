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
## - Run Motor Go to Position
### - Base
![RMGtP.b.png](./images/RMGtP.b.png)
```python
motor = Motor('A')

motor.run_to_position(0, 'shortest path')
```
### - Multiple Motors
![RMGtP.m.png](./images/RMGtP.m.png)
```python
motor_a = Motor('A')
motor_e = Motor('E')

motor_a.run_to_position(0, 'shortest path')
motor_e.run_to_position(0, 'shortest path')
```
### - Clockwise
![RMGtP.c.png](./images/RMGtP.c.png)
```python
motor = Motor('A')

motor.run_to_position(0, 'clockwise')
```
### - Counterclockwise
![RMGtP.cc.png](./images/RMGtP.cc.png)
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
## - Set Motor Speed
## - Motor Position
## - Motor Speed
# Movement
# Light
# Sound
# Events
# Control
# Sensors
# Operators
# Variables
