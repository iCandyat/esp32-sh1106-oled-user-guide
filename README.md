# ESP32 驱动 SH1106 OLED 屏幕教程

## 一、硬件准备
### 硬件清单
- ESP32-WROOM 开发板（搭载CH340 USB转串口芯片）
- SH1106 OLED SPI 屏幕
- 若干杜邦线

### 设备连线说明
| 开发板引脚 | 屏幕引脚 |
|------------|----------|
| GND        | GND      |
| VCC        | 3v3      |
| D22        | SCK      |
| D21        | SDA      |
| D4         | RES      |
| D13        | DC       |
| D5         | CS       |


## 二、软件准备
### 1. CH340驱动
根据操作系统选择对应的驱动：
- Windows系统：[下载链接](https://www.wch.cn/download/file?id=65)
- Linux系统：[下载链接](https://www.wch.cn/download/file?id=5)
- macOS系统：[下载链接](https://www.wch.cn/download/file?id=178)
- Android系统：[下载链接](https://www.wch.cn/download/file?id=195)
- WCH官网驱动汇总：[官网链接](https://www.wch.cn/downloads/category/67.html)

### 2. Arduino IDE
各系统版本下载：
- Windows 64位: [下载链接](https://downloads.arduino.cc/arduino-ide/arduino-ide_2.3.6_Windows_64bit.exe)
- Windows MSI: [下载链接](https://downloads.arduino.cc/arduino-ide/arduino-ide_2.3.6_Windows_64bit.msi)
- Windows ZIP:[下载链接](https://downloads.arduino.cc/arduino-ide/arduino-ide_2.3.6_Windows_64bit.zip)
- Linux Applmage:[下载链接](https://downloads.arduino.cc/arduino-ide/arduino-ide_2.3.6_Linux_64bit.AppImage)
- Linux zip:[下载链接](https://downloads.arduino.cc/arduino-ide/arduino-ide_2.3.6_Linux_64bit.zip)
- Macos intel:[下载连接](https://downloads.arduino.cc/arduino-ide/arduino-ide_2.3.6_macOS_64bit.dmg)
- MacOS :[下载连接](https://downloads.arduino.cc/arduino-ide/arduino-ide_2.3.6_macOS_arm64.dmg)
- Arduino IDE官网:[官网链接](https://www.arduino.cc/en/software/)

### 3. ESP32 开发包
- Windows 版本：[百度网盘](https://pan.baidu.com/s/1vxRKCljoZyfE3GjvRIpOrw?pwd=1234)


## 三、点亮屏幕步骤
### 1. 初始设置
- 打开Arduino IDE
- 更换语言：`File`→`Preferences`→`Language`（选择所需语言）

### 2. 安装ESP32开发包
- 打开从百度网盘下载的`esp32_package_2.0.9_arduinome.exe`，按照提示完成安装

### 3. 配置开发板
- 选择开发板：`Arduino`→`工具`→`开发板`→`esp32`→`ESP32 WROVER MODULE`
- 选择端口：`Arduino`→`工具`→`端口`→`COMx`（根据实际连接的端口选择）

### 4. 安装所需库
- 打开库管理器：`Arduino`→`工具`→`管理库`
- 分别搜索并安装以下库：
  - Adafruit GFX Library by Adafruit
  - Adafruit BusIO by Adafruit
  - Adafruit SH110X by Adafruit

### 5. 上传测试代码
- 复制代码：访问[GitHub仓库](https://github.com/iCandyat/esp32-sh1106-oled-user-guide/blob/main/Demo_1)，复制示例代码
- 粘贴到Arduino IDE中
- 单击"上传"按钮，编译并将代码推送到开发板

如果一切顺利，此时屏幕应该会亮起！

🎉**恭喜成功点亮屏幕！**🎉


## 四、问题解决
如果遇到报错或有疑问，请发送邮件至：`icandyat@gmail.com`
