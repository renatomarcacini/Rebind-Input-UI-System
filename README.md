# Rebind-Input-UI-System

Simple system to rebind buttons with new input system.

# Instalation

1) In Package Manager install the lastest version of Input System. (Used 1.3.0v)
2) In Player Settings->Other Settings->Active Input Handling; Change 'Input Manager (old) or Input System Package (new)' to 'Both'.
3) Open and play the scene example in Scenes/Rebind System Example.<br> 

Note ¹: To work properly when developing your own Canvas interface, locate your EventSystem and check that the 'Standalone Input Module' has been updated to 'Input System UI Input Module'. To do this, click on 'Replace with InputSystemUIInputModule' generating the result below. <br>

[EventSystem] Old input system: <br>
<img src= "https://i.ibb.co/gZTwDNs/event-system-before.png" width='400px'>
 
[EventSystem] New input system: <br>
<img src= "https://i.ibb.co/ys1Lz7p/event-system-after.png" width='400px'>

Note 2: In 'Input System UI Input Module'->Submit it is 'None' as the joystick/southButton is recognized as UI/Submit, automatically applying the same input during rebind. This problem will not occur depending on how you work with your Canvas/Menu System.

# Making Settings

In the scene example 'Scenes/Rebind System Example', localize in Hiearchy Canvas->ControlsPanel->PSPanel->Rebind Button.  
<img src= "https://i.ibb.co/R6f0Xb2/rebind-button2.png" width='400px'>

<h3>Input Action Reference</h3> 
It is the input mapped to the 'PlayerInput' component that you want to perform or rebind. Example: jumping, shooting, etc... <br>

<h3>Selected Binding<h3> 
It is the index according to the type of controller you want to rebind.
  
<h3>Input Binding</h3> 
Debugger to visualize the action and controller to remap. Example according to PlayerInput in that package: <br> <br>
If Selected Binding = 0, the 'path' will be for the 'Keyboard' type. <br>
If Selected Binding = 1, the 'path' will be for the 'Gamepad' type.  <br>
If Selected Binding = 2, the 'path' will be for type 'PS4'. <br>
If Selected Binding = 3, the 'path' will be for type 'Xbox'. <br>
