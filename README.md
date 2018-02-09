# Arduino-SteamVR-controller

# What is this?
This is the code of my custom built motion controller made from a set of Razer Hydras with a TeensyLC and a MPU9250. For use in conjunction with the Leap Motion in Virtual Reality.

# Known issues
- Currently the orientation data is the built-on DMP's (Digital Motion Processor)  output, without any further processing. It's quite good and stable, 
but it uses only the gyroscope, and the accelerometer, not the magnetometer. With intense movements, it can drift quite easily.
- As the communication is on USB only, you need two, quite long USB cables. This is far from comfortable, especially when using it with a VR headset
(what is the intended use).

# Future plans for improvements
- Add Bluetooth, and a battery, to enable wireless operation.

# Build process
I've built one of these controllers so far, from a TeensyLC, MPU2950 and the button and joystick daughter board from a set of Razer Hydras.

# Special thanks
Thanks for github user rpicopter, for the DMP enabled motion processing library for the MPU9250. I used this, to get the DMP data from my MPU-9255.
https://github.com/rpicopter/ArduinoMotionSensorExample

Thanks to githug user peter10110 who built this entire project of which I am just modifying to my spec.
