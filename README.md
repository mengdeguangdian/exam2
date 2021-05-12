# exam2
By sudo screnn command "/DET_Thread/run 2 1, the led2 will be on and the angle detection mode will begin
Then uLCD begin to update recent detected angle consecutivelly
You can make a gesture from "ring", "slope" and "tilt" which match to gesture_class number 0, 1 and 2
After you make a gesture, the screen will show the gesture ID(0~10), gesture class(0/1/2)
The screen will also show the feature, my feature is the maximum detected angle during the gesture, if maximum angle > 45 degree, the feature is represented by 1,
else if maximum angle < 45 degree, this feature is represented by 0
After 10 gestures are made, the mbed will send all the 10 events to python
IF MQTT/Wifi doesn't work, you can use sudo screen command /DATA_T/run 3 1 to retrive 10 gesture events
