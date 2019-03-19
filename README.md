
MPU6050 teapot demo with DMP, or Digital Motion Processor in C++

MPU6050-Pi-Demo

```
sudo apt-get install libgtkmm-3.0-dev
sudo i2cdetect -y 1
make
cd MPU6050-Pi-Demo
./demo_3d
./demo_dmp
./demo_raw
```

I2Cdev.h and I2Cdev.cpp modified for I2C_PATH.
```#define I2C_PATH "/dev/i2c-1"```
Original has "/dev/i2c-0" in three locations in I2Cdev.cpp

https://www.okahiro.info/gd/2016/10/07/post-1978/


PiBits
======

Here you'll find various RaspberryPi related projcts:

ServoBlaster:  A kernel driver that lets you control 8 (or more) servos from your RaspberryPi.

Panalyzer:     A Pi based Logic Analyzer.  This can be found in a separate repository alongside this one, but is mentioned here for completeness.

PiFmDma:       A Version of the FM Transmitter software that uses DMA for improved quality and much reduced CPU load.  NOTE: Do not use this code unless you understand what it does, what FM frequencies it might interfere with, what is and is not legal in your country, etc.

MouseScan:     Code to turn the sensor in an optical mouse in to a very crude
               hand held scanner.

MPU6050-Pi-Demo:  Code to drive an MPU6050 accelerometer/gyroscope via I2C
               from the RaspberryPi.
