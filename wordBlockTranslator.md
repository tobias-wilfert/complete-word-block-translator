# Word Block Translator

## Motors
### - Run Motor for Duration
#### - Base
![RMfD.b.png](./images/RMfD.b.png)
```python
motor = Motor('A')
motor.run_for_rotations(1, 75)
```
#### - Multiple Motors
![RMfD.m.png](./images/RMfD.m.png)
```python
motor_pair = MotorPair('A', 'E')
motor_pair.move_tank(1, 'rotations', -75, 75)
```
#### - Counterclockwise
![RMfD.c.png](./images/RMfD.c.png)
```python
motor = Motor('A')
motor.run_for_rotations(1, -75)
```
#### - Degrees
![RMfD.d.png](./images/RMfD.d.png)
```python
motor = Motor('A')
motor.run_for_degrees(1, 75)
```
#### - Seconds
![RMfD.s.png](./images/RMfD.s.png)
```python
motor = Motor('A')
motor.run_for_seconds(1, 75)
```
### - Run Motor Go to Position
### - Start Motor
### - Stop Motor
### - Set Motor Speed
### - Motor Position
### - Motor Speed
## Movement
## Light
## Sound
## Events
## Control
## Sensors
## Operators
## Variables
