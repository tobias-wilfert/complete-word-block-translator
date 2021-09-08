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
![SA.png](images/Light/SA.png)  
TODO: Needs custom python code
## - Play Animation until Done
![SAuD.png](images/Light/SAuD.png)  
TODO: Needs custom python code
## - Turn On 5x5 Light Matrix for Seconds
![TOLMfS.png](images/Light/TOLMfS.png)  
```python
hub = MSHub()

hub.light_matrix.show_image('HAPPY') 
wait_for_seconds(2)
hub.light_matrix.off()
```
## - Turn On 5x5 Light Matrix
![TOLM.png](images/Light/TOLM.png)  
```python
hub = MSHub()

hub.light_matrix.show_image('HAPPY') 
```
## - Write on 5x5 Matrix
![WoM.png](images/Light/WoM.png)  
```python
hub = MSHub()

hub.light_matrix.write('Hello')
```
## - Turn off Pixels
![ToP.png](images/Light/ToP.png)  
```python
hub = MSHub()

hub.light_matrix.off()
```
## - Set Pixel Brightness
![SPB.png](images/Light/SPB.png)  
TODO: Check if this block effects the 'Write' block   
Python equivalent is to set the brightness when calling the methods
## - Set Pixel
![SP.png](images/Light/SP.png)  
```python
hub = MSHub()

hub.light_matrix.set_pixel(1, 1, 100)
```
## - Rotate Orientation
![RO.png](images/Light/RO.png)  
TODO: Only possible with Mindstorms internal library
## - Set Orientation
![RO.png](images/Light/SO.png)  
TODO: Only possible with Mindstorms internal library
## - Set Center Button Light
![SCBL.png](images/Light/SCBL.png)  
```python
hub = MSHub()

hub.status_light.on('red')
```
## - Light Up Distance Sensor
![LUPDS.png](images/Light/LUDS.png)  
```python
distance_sensor = DistanceSensor('A')

distance_sensor.light_up(100, 100, 100, 100)
```
# Sound
## - Play Sound until Done
![PSuD.png](images/Sound/PSuD.png)  
```python

```
## - Start sound
![Ss.png](images/Sound/Ss.png)  
```python

```
## - Play Beep for Seconds
![PBfS.png](images/Sound/PBfS.png)  
```python

```
## - Start Playing Beep
![SPB.png](images/Sound/SPB.png)  
```python

```
## - Stop All Sounds
![SAS.png](images/Sound/SAS.png)  
```python

```
## - Change Pitch Effect by
### - Base
![CPEb.b.png](images/Sound/CPEb.b.png)  
```python

```
### - Pan
![CPEb.p.png](images/Sound/CPEb.p.png)  
```python

```
## - Set Pitch Effect to
### - Base
![SPEt.b.png](images/Sound/SPEt.b.png)  
```python

```
### - Pan
![SPEt.p.png](images/Sound/SPEt.p.png)  
```python

```
## - Clear Sound Effects
![CSE.png](images/Sound/CSE.png)  
```python

```
## - Change Volume
![CV.png](images/Sound/CV.png)  
```python

```
## - Set Volume
![SV.png](images/Sound/SV.png)  
```python

```
## - Volume
![V.png](images/Sound/V.png)  
```python

```
# Events
## - When Program Starts
![WPS.png](images/Events/WPS.png)  
```python

```
## - When Color Is
![WCI.png](images/Events/WCI.png)  
```python

```
TODO: Add Button Pressed
## - When Closer Than
### - Base
![WCT.b.png](images/Events/WCT.b.png)  
```python

```
### - Farther than
![WCT.f.png](images/Events/WCT.f.png)  
```python

```
### - Exactly at
![WCT.e.png](images/Events/WCT.e.png)  
```python

```
### - Centimeters
![WCT.c.png](images/Events/WCT.c.png)  
```python

```
### - Inches
![WCT.i.png](images/Events/WCT.i.png)  
```python

```
## - When Hub Orientation Is Up
### - Base
![WHOIU.b.png](images/Events/WHOIU.b.png)  
```python

```
### - Back
![WHOIU.back.png](images/Events/WHOIU.back.png)  
```python

```
### - Top
![WHOIU.t.png](images/Events/WHOIU.t.png)  
```python

```
### - Bottom
![WHOIU.bo.png](images/Events/WHOIU.bo.png)  
```python

```
### - Right side
![WHOIU.r.png](images/Events/WHOIU.r.png)  
```python

```
### - Left side
![WHOIU.l.png](images/Events/WHOIU.l.png)  
```python

```
## - When Hub Shaken
### - Base
![WHS.b.png](images/Events/WHS.b.png)  
```python

```
### - Tapped
![WHS.t.png](images/Events/WHS.t.png)  
```python

```
### - Falling
![WHS.f.png](images/Events/WHS.f.png)  
```python

```
## - When Hub Button Pressed
### - Base
![WHBP.b.png](images/Events/WHBP.b.png)  
```python

```
### - Right
![WHBP.ri.png](images/Events/WHBP.ri.png)  
```python

```
### - Released
![WHBP.re.png](images/Events/WHBP.re.png)  
```python

```
## - When
![W.png](images/Events/W.png)  
```python

```
## - When I Receive Message
![WIRM.png](images/Events/WIRM.png)  
```python

```
## - Broadcast Message
![BM.png](images/Events/BM.png)  
```python

```
## - Broadcast Message and Wait
![BMaW.png](images/Events/BMaW.png)  
```python

```
## - When Timer
![WT.png](images/Events/WT.png)  
```python

```
## - When Key Pressed
![WKP.png](images/Events/WKP.png)  
```python

```
# Control
## - Wait for Seconds
![WfS.png](images/Control/WfS.png)  
```python

```
## - Wait Until
![WU.png](images/Control/WU.png)  
```python

```
## - Repeat Loop
![RL.png](images/Control/RL.png)  
```python

```
## - Forever Loop
![FL.png](images/Control/FL.png)  
```python

```
## - Repeat Until Loop
![RUL.png](images/Control/RUL.png)  
```python

```
## - If Then
![IT.png](images/Control/IT.png)  
```python

```
## - If Then Else
![ITE.png](images/Control/ITE.png)  
```python

```
## - Stop other stacks
![Sos.png](images/Control/Sos.png)  
```python

```
## - Stop
### - Base  
![S.b.png](images/Control/S.b.png)  
```python

```
### - This stack  
![S.t.png](images/Control/S.t.png)  
```python

```
### - Exit Program  
![S.e.png](images/Control/S.e.png)  
```python

```
# Sensors
## - Is color?
![Ic.png](images/Sensors/Ic.png)  
```python

```
## - Color
![C.png](images/Sensors/C.png)  
```python

```
## - Is reflected light?
### - Base
![Irl.b.png](images/Sensors/Irl.b.png)  
```python

```
### - Equal
![Irl.e.png](images/Sensors/Irl.e.png)  
```python

```
### - Greater than
![Irl.g.png](images/Sensors/Irl.g.png)  
```python

```
## - Reflected Light
![RL.png](images/Sensors/RL.png)  
```python

```
## - Is distance?
### - Base
![Id.b.png](images/Sensors/Id.b.png)  
```python

```
### - Farther than
![Id.f.png](images/Sensors/Id.f.png)  
```python

```
### - Exactly at
![Id.e.png](images/Sensors/Id.e.png)  
```python

```
### - Centimeters
![Id.c.png](images/Sensors/Id.c.png)  
```python

```
### - Inches
![Id.i.png](images/Sensors/Id.i.png)  
```python

```
## - Distance
### - Base
![D.b.png](images/Sensors/D.b.png)  
```python

```
### - Centimeters
![D.c.png](images/Sensors/D.c.png)  
```python

```
### - Inches
![D.i.png](images/Sensors/D.i.png)  
```python

```
## - Gesture
![G.png](images/Sensors/G.png)  
```python

```
## - Is Hub Shaken?
### - Base
![IHS.b.png](images/Sensors/IHS.b.png)  
```python

```
### - Tapped
![IHS.t.png](images/Sensors/IHS.t.png)  
```python

```
### - Falling
![IHS.f.png](images/Sensors/IHS.f.png)  
```python

```
## - Is Hub orientation?
### - Base
![IHo.b.png](images/Sensors/IHo.b.png)  
```python

```
### - Back
![IHo.back.png](images/Sensors/IHo.back.png)  
```python

```
### - Top
![IHo.t.png](images/Sensors/IHo.t.png)  
```python

```
### - Bottom
![IHo.bo.png](images/Sensors/IHo.bo.png)  
```python

```
### - Right Side
![IHo.r.png](images/Sensors/IHo.r.png)  
```python

```
### - Left Side
![IHo.l.png](images/Sensors/IHo.l.png)  
```python

```
## - Hub Orientation
![HO.png](images/Sensors/HO.png)  
```python

```
## - Set Hub Yaw Angle to 0
![SHYA.png](images/Sensors/SHYA.png)  
```python

```
## - Is Hub Button pressed?
### - Base
![IHBp.b.png](images/Sensors/IHBp.b.png)  
```python

```
### - Right
![IHBp.ri.png](images/Sensors/IHBp.ri.png)  
```python

```
### - Released
![IHBp.re.png](images/Sensors/IHBp.re.png)  
```python

```
## - Hub Pitch Roll Yaw Angle
### - Base
![HPRYA.b.png](images/Sensors/HPRYA.b.png)  
```python

```
### - Roll
![HPRYA.r.png](images/Sensors/HPRYA.r.png)  
```python

```
### - Yaw
![HPRYA.y.png](images/Sensors/HPRYA.y.png)  
```python

```
## - Timer
![T.png](images/Sensors/T.png)  
```python

```
## - Reset Timer
![RT.png](images/Sensors/RT.png)  
```python

```
## - Key Pressed
![KP.png](images/Sensors/KP.png)  
```python

```
# Operators
## - Pick Random Number
## - Plus
## - Minus
## - Multiply
## - Divide
## - Greater Than
## - Less Than
## - Equal
## - And
## - Or
## - Not
## - Is Between
## - Join Strings
## - Letter of String
## - Length of String
## - String Contains
## - Mod
## - Round
## - Math Functions
# Variables
## - Variable
## - Set Variable To
## - Change Variable By
## - List
## - Add Item to List
## - Delete Item in List
## - Delete All Items in List
## - Insert Item at Index in List
## - Replace  item at Index in List with Another Item
## - Value of Item in List
## - Length of List
## - List contains
