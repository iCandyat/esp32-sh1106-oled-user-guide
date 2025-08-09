# 硬件清单
- ESP32-WROOM 开发板（搭载CH340 USB转串口芯片）
- SH1106 OLED SPI 屏幕
- 若干杜邦线


### 扩展硬件
- 3P风扇


# 设备连线说明
| 开发板引脚 | 屏幕引脚 |
|------------|----------|
| GND        | GND      |
| VCC        | 3v3      |
| D22        | SCK      |
| D21        | SDA      |
| D4         | RES      |
| D13        | DC       |
| D5         | CS       |


# 软件清单
## CH340驱动
- Windows系统：[下载链接](https://www.wch.cn/download/file?id=65)
- Linux系统：[下载链接](https://www.wch.cn/download/file?id=5)
- macOS系统：[下载链接](https://www.wch.cn/download/file?id=178)
- Android系统：[下载链接](https://www.wch.cn/download/file?id=195)
- WCH官网驱动汇总：[官网链接](https://www.wch.cn/downloads/category/67.html)

## Arduino IDE
- Windows 64位: [下载链接](https://downloads.arduino.cc/arduino-ide/arduino-ide_2.3.6_Windows_64bit.exe)
- Windows MSI: [下载链接](https://downloads.arduino.cc/arduino-ide/arduino-ide_2.3.6_Windows_64bit.msi)
- Windows ZIP:[下载链接](https://downloads.arduino.cc/arduino-ide/arduino-ide_2.3.6_Windows_64bit.zip)
- Linux Applmage:[下载链接](https://downloads.arduino.cc/arduino-ide/arduino-ide_2.3.6_Linux_64bit.AppImage)
- Linux zip:[下载链接](https://downloads.arduino.cc/arduino-ide/arduino-ide_2.3.6_Linux_64bit.zip)
- Macos intel:[下载连接](https://downloads.arduino.cc/arduino-ide/arduino-ide_2.3.6_macOS_64bit.dmg)
- MacOS :[下载连接](https://downloads.arduino.cc/arduino-ide/arduino-ide_2.3.6_macOS_arm64.dmg)
- Arduino IDE官网:[官网链接](https://www.arduino.cc/en/software/)


## esp32_package_2.0.12_arduinome
- Windows [百度网盘](https://pan.baidu.com/s/1vxRKCljoZyfE3GjvRIpOrw?pwd=1234)


# 点亮屏幕
### 打开Arduino IDE
## 更换语言
### file-->preferences-->language
## step 1
### 打开从百度网盘上下载的esp32_package_2.0.9_arduinome.exe
## step 2
### Arduino-->工具-->开发板-->esp32-->ESP32 WROVER MODULE
### Arduino-->工具-->端口-->COMx(视情况而定)
