# Movement-of-Robot-Joints
## Aim:  
To move and drive the joints of the robot using python API.

## Equipment’s required:

Visual Components Premium 4.3

## Procedure:

1. 	In the eCatalog panel, Collections view, browse to Models by Type>Robots>Visual Components and then add a Generic Articulated Robot to the 3D world.
2. 	Click the Modeling tab, and then add a Python Script behaviour. The script editor will open automatically when you add the behaviour.
3. 	In the script editor, add the code and then compile the code.

## Program
```
from vcScript import *
from vcHelpers.Robot2 import *
def OnRun():
  pos=[[1,30],[2,40],[3,90]]
  robot = getRobot()
  robot.driveJoints(0,0,0,0,0,0)
  delay(5)
  for i in pos:
    robot.Controller.moveJoint(i[0],i[1])
    delay(5)
```
## Output
### 1. Generic Articulated Robot

![image](https://github.com/surothaaman/Movement-of-Robot-Joints/assets/133313653/1b3718d2-8e2d-474b-a1bc-45b702427b4e)

### 2. robot.driveJoints(0,0,0,0,0,0)

![image](https://github.com/surothaaman/Movement-of-Robot-Joints/assets/133313653/bd7b6fbb-30fb-4398-af60-aeb85e07f7de)

### 3. Movement of Joint1

![image](https://github.com/surothaaman/Movement-of-Robot-Joints/assets/133313653/8ae5a91b-0c8a-4054-a0f8-a43d526a5763)



### 3. Movement of Joint2

![image](https://github.com/surothaaman/Movement-of-Robot-Joints/assets/133313653/58ebdc42-4331-4214-bfa9-0beba69fe9f6)


### 3. Movement of Joint3


![image](https://github.com/surothaaman/Movement-of-Robot-Joints/assets/133313653/957e975e-607d-4025-8540-c7a736112865)

## Result 
Thus the different robots joints are moved with the help of python list.


