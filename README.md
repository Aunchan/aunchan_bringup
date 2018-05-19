# aunchan_bringup
roslaunch scripts for starting the Aunchan

## Package dependencies

```
$ sudo apt install ros-kinetic-rosserial*
```

## Add rules

```
$ sudo cp 99-aunchan.rules /etc/udev/rules.d/
$ sudo udevadm control --reload-rules
$ sudo udevadm trigger
```

> เปลี่ยนพอร์ท `STM32` จาก `/dev/ttyUSB0` เป็น `/dev/ttySTM32`
> 
>เปลี่ยนพอร์ท `Lidar` จาก `/dev/ttyUSB1` เป็น `/dev/ttyLidar`