# MPU9250 with Beaglebone Black - SPI

This project contains Self Test, calibration, AHRS fusion demostration with embedded Linux development board Beaglebone Black, using _SPI 4 wires_.

For information and datasheet links, please check wiki page https://github.com/leptonation/BBB_MPU9250/wiki

Some of the ideas come from https://github.com/kriswiner/MPU-9250, which is for Arduino using I2C and AUX I2C ByPass Mode for magnetometer to show up in I2C Bus.

IMU and AHRS codes come from http://www.x-io.co.uk/open-source-imu-and-ahrs-algorithms/

When processor using SPI to talk with MPU, setting ByPass Mode in MPU and let processor to use I2C to communicate with magnetometer is not possible. In this case MPU9250 need to enable Master mode and using slave register to communicate with magnetometer. This project, hopefully, provide a demostration how to do it.
