# Ranger-ROV

This repo is to keep track of all my work on Ranger ROV, ranging from design, BOM, program, SID and technicial document.

This is basically two separate system, ardusub firmware in pixhawk to control the main ROV, and teensy to mini ROV.

Firmware : ArduSub (ardusub.com) / Px4 (pix4.io and ardupilot.org)

For QGroundControl (Main ROV unit)

1.Surface : Jetson Nano with Ubunto 20.08 (64-bit)

2.ROV Componian computer : Raspberry Pi with Raspbian

3.ROV ArduSub : Pix4 (2.4.8)

4.ROV Controller - XBox control or Custom made with teensy, program with arduino C

5.Control reference : DIY ROV Software Setup Tutorial, Raspberry Pi (https://www.youtube.com/watch?v=mH0vH4dd3Vo)

Note : Cat5 / Cat 5E was use as signal tether for the maximum cable length in this case is about 20m, signal attenuation is expected to be neglib
le for this physical cable confiuration with 100 megabits per second. (we can skip the Fathom-X as in BlueROV configuration)


For Mini-robot

1.Teensy at surface with custom made control, teensy at ROV with custom made manulipator

2.Signal via RS485 module

PixHawk setting
MAIN 1-6 : Thruster ESC
Aux 1-3 : 3 DOF Gripper(U R T)
Aux 4-6 : Mini ROV (Forward/Backward, Grippler(T), Gripper rotation (R))


