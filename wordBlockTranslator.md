# Word Block Translator

# Motors
## - Run Motor for Duration
### - Base
![RMfD.b.png](images/Motor/RMfD.b.png)
```python
motor = Motor('A')

motor.run_for_rotations(1, 75)
```
### - Multiple Motors
![RMfD.m.png](images/Motor/RMfD.m.png)
```python
motor_pair = MotorPair('A', 'E')

motor_pair.move_tank(1, 'rotations', -75, 75)
```
### - Counterclockwise
![RMfD.c.png](images/Motor/RMfD.c.png)
```python
motor = Motor('A')

motor.run_for_rotations(1, -75)
```
### - Degrees
![RMfD.d.png](images/Motor/RMfD.d.png)
```python
motor = Motor('A')

motor.run_for_degrees(1, 75)
```
### - Seconds
![RMfD.s.png](images/Motor/RMfD.s.png)
```python
motor = Motor('A')

motor.run_for_seconds(1, 75)
```
## - Motor Go to Position
### - Base
![MGtP.b.png](images/Motor/MGtP.b.png)
```python
motor = Motor('A')

motor.run_to_position(0, 'shortest path')
```
### - Multiple Motors
![MGtP.m.png](images/Motor/MGtP.m.png)
```python
motor_a = Motor('A')
motor_e = Motor('E')

motor_a.run_to_position(0, 'shortest path')
motor_e.run_to_position(0, 'shortest path')
```
### - Clockwise
![MGtP.c.png](images/Motor/MGtP.c.png)
```python
motor = Motor('A')

motor.run_to_position(0, 'clockwise')
```
### - Counterclockwise
![MGtP.cc.png](images/Motor/MGtP.cc.png)
```python
motor = Motor('A')

motor.run_to_position(0, 'counterclockwise')
```
## - Start Motor
### - Base
![SaM.b.png](images/Motor/SaM.b.png)
```python
motor = Motor('A')

motor.start(75)
```
### - Multiple Motors
TODO: Check if start_tank or just start is correct  
![SaM.m.png](images/Motor/SaM.m.png)
```python
motor_pair = MotorPair('A', 'E')

motor_pair.start_tank(75, -75)
```
### - Counterclockwise
![SaM.c.png](images/Motor/SaM.c.png)
```python
motor = Motor('A')

motor.start(-75)
```
## - Stop Motor
### - Base
![SoM.b.png](images/Motor/SoM.b.png)
```python
motor = Motor('A')

motor.stop()
```
### - Multiple Motors
![SoM.m.png](images/Motor/SoM.m.png)
```python
motor_pair = MotorPair('A', 'E')

motor_pair.stop()
```
## - Set Motor Speed
### - Base
TODO: Check that this works  
![SMS.b.png](images/Motor/SMS.b.png)
```python
motor = Motor('A')

motor.set_default_speed(75)
```
### - Multiple Motors
![SMS.m.png](images/Motor/SMS.m.png)
```python
motor_pair = MotorPair('A', 'E')

motor_pair.set_default_speed(75)
```
## - Motor Position
![MP.png](images/Motor/MP.png)
```python
motor = Motor('A')

motor.get_position()
```
## - Motor Speed
![MS.png](images/Motor/MS.png)
```python
motor = Motor('A')

motor.get_speed()
```
# Movement
## - Move for Duration
### - Base
![MfD.b.png](images/Movement/MfD.b.png)
```python
motor_pair = MotorPair('A', 'B')

motor_pair.move(10, 'cm')
```
### - Backwards 
![MfD.bw.png](images/Movement/MfD.bw.png)
```python
motor_pair = MotorPair('A', 'B')

motor_pair.move(-10, 'cm')
```
### - Counterclockwise
![MfD.ccw.png](images/Movement/MfD.ccw.png)
```python
motor_pair = MotorPair('A', 'B')

motor_pair.move(10, 'cm', -100)
```
### - Clockwise
![MfD.cw.png](images/Movement/MfD.cw.png)
```python
motor_pair = MotorPair('A', 'B')

motor_pair.move(10, 'cm', 100)
```
### - Inches
![MfD.i.png](images/Movement/MfD.i.png)
```python
motor_pair = MotorPair('A', 'B')

motor_pair.move(10, 'in')
```
### - Rotations
![MfD.r.png](images/Movement/MfD.r.png)
```python
motor_pair = MotorPair('A', 'B')

motor_pair.move(10, 'rotations')
```
### - Degrees
![MfD.d.png](images/Movement/MfD.d.png)
```python
motor_pair = MotorPair('A', 'B')

motor_pair.move(10, 'degrees')
```
### - Seconds
![MfD.s.png](images/Movement/MfD.s.png)
```python
motor_pair = MotorPair('A', 'B')

motor_pair.move(10, 'seconds')
```
## - Move with Steering for Duration
### - Base
![MwSfD.b.png](images/Movement/MwSfD.b.png)
```python
motor_pair = MotorPair('A', 'B')

motor_pair.move(10, 'cm', 42)
```
### - Inches
![MwSfD.i.png](images/Movement/MwSfD.i.png)
```python
motor_pair = MotorPair('A', 'B')

motor_pair.move(10, 'in', 42)
```
### - Rotations
![MwSfD.r.png](images/Movement/MwSfD.r.png)
```python
motor_pair = MotorPair('A', 'B')

motor_pair.move(10, 'rotations', 42)
```
### - Degrees
![MwSfD.d.png](images/Movement/MwSfD.d.png)
```python
motor_pair = MotorPair('A', 'B')

motor_pair.move(10, 'degrees', 42)
```
### - Seconds
![MwSfD.s.png](images/Movement/MwSfD.s.png)
```python
motor_pair = MotorPair('A', 'B')

motor_pair.move(10, 'seconds', 42)
```
## - Start Moving with Steering
![SMwS.png](images/Movement/SMwS.png)
```python
motor_pair = MotorPair('A', 'B')

motor_pair.start(42)
```
## - Stop Moving
![SM.png](images/Movement/SM.png)
```python
motor_pair = MotorPair('A', 'B')

motor_pair.stop()
```
## - Set Movement Speed
![SMS.png](images/Movement/SMS.png)
```python
motor_pair = MotorPair('A', 'B')

motor_pair.set_default_speed(50)
```
## - Set Movement Motors
![SMM.png](images/Movement/SMM.png)
```python
motor_pair = MotorPair('A', 'B')
```
## - Set 1 Motor Rotation to Distance Moved
### - Base
![S1MRtDM.b.png](images/Movement/S1MRtDM.b.png)
```python
motor_pair = MotorPair('A', 'B')

motor_pair.set_motor_rotation(17.5, 'cm')
```
### - Inches
![S1MRtDM.i.png](images/Movement/S1MRtDM.i.png)
```python
motor_pair = MotorPair('A', 'B')

motor_pair.set_motor_rotation(17.5, 'in')
```
# Light
## - Start Animation
## - Play Animation until Done
## - Turn On 5x5 Light Matrix for Seconds
## - Turn On 5x5 Light Matrix
## - Write on 5x5 Matrix
## - Turn off Pixels
## - Set Pixel Brightness
## - Set Pixel
## - Rotate Orientation
## - Set Orientation
## - Set Center Button Light
## - Light Up Distance Sensor
# Sound
# Events
# Control
# Sensors
# Operators
# Variables
