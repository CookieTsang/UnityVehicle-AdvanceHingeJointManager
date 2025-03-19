# UnityVehicle-AdvanceHingeJointManager   
![image](https://github.com/user-attachments/assets/be0d9de8-bdd5-4674-bb6e-92b2b0a6416f)  
# 使用步骤  
添加脚本到游戏对象：  
﻿![image](https://github.com/user-attachments/assets/69e0eb1e-75d7-4d25-a26f-ab04331103ec)

在 Unity 中创建一个空的 GameObject，并将这个脚本附加到该对象上。  
设置铰链关节：  
在游戏对象的检视面板中，你会看到 Controlled Joints 列表。你可以通过点击“+”按钮添加新的 ControlledHingeJoint 元素。  
每个元素都需要关联一个铰链关节（Hinge Joint）组件。确保在场景中创建并配置你的铰链关节。  
# 配置键位：  
对于每个铰链关节，你可以设置三个按键：  
clockwiseKey：控制关节顺时针旋转的按键。  
counterClockwiseKey：控制关节逆时针旋转的按键。  
singleCtrlKey：用于单独控制关节的按键。  
你可以根据需要选择任何可用的 KeyCode（例如：KeyCode.A、KeyCode.D等）。  
调整运动参数：  
individualForce：设置单独控制时的力大小。  
motorSpeed：设置控制时的速度。  
# 全局控制（两个按键控制所有铰链的例子）：  
﻿脚本中定义了全局控制按键（O 和 P），你可以通过按这些键来控制所有关节的运动。  
按 O：所有关节同时顺转。  
按 P：所有关节同时反转。  
运行游戏  
运行游戏时，你可以通过设置的按键来控制关节的动作。脚本会处理关节的状态并确保只在需要的时候激活马达。  
# 提示  
确保所有的铰链关节都是有效的，不然被移除的关节将不会被控制。  
使用 DisableAllMotors 方法可以在需要时禁用所有马达控制。  
# Usage steps  
Add script to game object:  
Create an empty GameObject in Unity and attach this script to the object.  
# Set hinge joints:  
In the inspection panel of the game object, you will see a list of Controlled Joints. You can add a new ControlledHingeJoint element by clicking the "+" button.  
Each element needs to be associated with a hinge joint component. Make sure to create and configure your hinge joints in the scene.  
Configure key positions:  
For each hinge joint, you can set three buttons:  
clockwiseKey： The button that controls the clockwise rotation of the joint.  
counterClockwiseKey： The button that controls the counterclockwise rotation of the joint.  
singleCtrlKey： A button used for individually controlling joints.  
You can choose any available KeyCode as needed (e.g. KeyCode. A, KeyCode. D, etc.).  
Adjust motion parameters:  
individualForce： Set the force magnitude for individual control.  
motorSpeed： Set the speed during control.  
# Global control:  
The script defines global control keys (O and P), which you can press to control the movement of all joints.  
Press O: All joints rotate clockwise simultaneously.  
Press P: Reverse all joints simultaneously.  
Run game  
When running the game, you can control the joint movements through the set buttons. The script will handle the state of the joints and ensure that the motor is only activated when needed.  
# Important Note  
Ensure that all hinge joints are valid, otherwise the removed joints will not be controlled.  
The DisabAllMotors method can be used to disable all motor controls when needed.  
