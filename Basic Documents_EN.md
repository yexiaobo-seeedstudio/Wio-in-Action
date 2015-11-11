## Introduction

### What is Pion One

**Pion One** is a Wi-Fi development board to build connected IoT projects with Groves. 

It’s based on ESP8266 Wi-Fi SoC, supporting a lot of [Grove modules](#grove).

Simplify your development of IoT devices without requirements of hardware programming or soldering.

￼￼<img src="https://github.com/yexiaobo-seeedstudio/Pion-Docs/raw/master/images/pionone-grove.png" width="454" height="495" alt="Pion One and Grove">

**Pion One is Out-of-Box**

Pion One based community friendly ESP8266 WiFi SoC and Grove 这种统一和简单接口的模块化硬件，把硬件开发难度几乎降低为零。

对硬件没有一点基础知识的软件开发人员，特别是 Web developers and Android/iOS developers, 可以以一种开箱即用的方式来开发 IoT devices.

Please visit **`Pion One Advanced Documents`** and **`Tools and Services`** to get total workflow of Pion One.

### <h3 id="grove"> What is Grove </h3>

**Grove** is a modulated, ready-to-use tool set. Much like Lego, it takes a building block approach to assembling electronics. Compared with the traditional, complicated learning method of using a breadboard and various electronic components to assemble a project, Grove simplifies and condenses the learning process significantly.  Every Grove module addresses a single function, such as a simple button or a more complex heart rate sensor.

**Grove is a Plug&Play hardware, without soldering**

There are more than 150+ Grove modules, more details about Grove System, please visit [Grove Wiki][Grove Wiki].

< 插入 Grove 图：一张预览图 >

### Pion One Modes, LED Status

- Config Mode

	<iframe src="https://player.vimeo.com/video/138398577" width="500" height="281" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>

- Requesting IP from Router
	
	<iframe src="https://player.vimeo.com/video/138397446" width="500" height="281" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>
	
- Connecting to The Server
	
	<iframe src="https://player.vimeo.com/video/138399886" width="500" height="281" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>
	
- Over-The-AIr(OTA), upgrade firmware
	
	<iframe src="https://player.vimeo.com/video/138397455" width="500" height="281" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>
	
- Connected Cloud
	
	<iframe src="https://player.vimeo.com/video/138399063" width="500" height="281" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>
	
### Pion One and Grove
Pion One supports 4 types connector of Grove：`I2C`，`Digital IO`，`Analog IO`，`UART`。

￼￼<img src="https://github.com/yexiaobo-seeedstudio/Pion-Docs/raw/master/images/pionone-grove.png" width="410" height="450" alt="Pion One and Grove">

There are almost 30 Grove moduels have been supported by Pion One. Such as:
 
 - Grove - Temp&Huminity Pro
 - Grove - Relay
 - Grove - Gesture Sensor
 - Grove - WS2812 led strip
 - Grove - Moisture Sensor
 - Grove - Air quality sensor v1.3
 - Grove - Digital Light Sensor
 - Grove - Magnetic Switch
 - Grove - PIR Motion Sensor
 - Grove - Barometer Sensor（BMP180)
 - Grove - Multichanel Gas Sensor
 - Grove - Speaker
 - And more... 

You cant get full list from **`Supported Grove Modules`** section.

## Mobile App

现在，我们分别提供了 Android 和 iOS App 对应 Android 和 iOS 设备。当然的，源码依然开源，Seeed 是一家硬件公司，Mobile App 的开发不是我们的特长，我们喜欢更多的人可以基于现在有的 App 开发他们自己的 Application。

Also, welcome to contribute to Pion One's Android/iOS App. [Android][Android App in Github] and [iOS][iOS App in Github] is host on GitHub.

###Features of Android/iOS App
  - Smart Config or AP Config: Let Pion One conenct to WiFi AP
  - Visual Configuration: Setup Pion One with Grove, update Firmware
  - Device Management: Create or Remove Pion One from server
  - Others created by you!!!

## Accessing Grove Sensors and Actuators
Each Grove module connected to Pion One can be visited by URL，and carry out Write，Read operations，similar to HTTP.  

How it's easy to access Grove sensors and actuators. 

### Command Line

**Shell Script with Curl:**

```shell
#!/bin/sh

curl -H "Authorization: token Your Token" https://iot.seeed.cc/v1/node/GroveTempHum/humidity
```

**Python Script:**

```python
import os;

def main:
	print "waiting"
```

**Ruby Script:**

```ruby
puts System.call("curl -H "Authorization: token Your Token"\
					 https://iot.seeed.cc/v1/node/GroveTempHum/humidity")
```

### IFTTT
(需要 App 操作视频）

### Node-Red
### Web App
### Your Application and More

## Cloud
### Lightweight Server/Cloud

Our lightweight server is Open Source by **Apache 2.0 License**.

There are some features:

- Account Manage
- Server for Compiling Firmware on Cloud
- Push Firmware to Pion One Over-The-Air(OTA)
- RESTful API support, Easy to Integrate Third Parts Cloud or Web Services
- Sync Grove Driver from Github Repos

We hope it can be more powerful, So, welcome to contribute, something like:

- Porting More Grove Module from Arduino Library, Check **`Developing Grove Driver`** Section
- Dashboard
- OAuth support
- IoT Services support, such as Azure, AWS
- More ...

Also, Welcome non-Grove hardware developer port your hardware to Pion One, please read **`Developing non-Grove Driver`** to get more infomation.
### Thirty Parts Cloud or Web Services
Pion One 现在支持 `IFTTT` 的 `IF Recipe` and `DO Recipe`, 可以从 **`Demos`** 章节了解更多细节。

`Github Hook Service`

`Microoft Azure`

`Intel HOPE`

More is coming soon.

## Supported Grove Modules
(列表）

[details]: https://github.com/yexiaobo-seeedstudio/Pion-Docs/raw/master/images/details.png

[Grove Wiki]: http://www.seeedstudio.com/wiki/Grove_System

[pionone-grove]: https://github.com/yexiaobo-seeedstudio/Pion-Docs/raw/master/images/pionone-grove.png

[connected_grove-temp]: https://github.com/yexiaobo-seeedstudio/Pion-Docs/raw/master/images/connected_grove-temp.jpg

[details]: https://github.com/yexiaobo-seeedstudio/Pion-Docs/raw/master/images/details.png

[api_tips]: https://github.com/yexiaobo-seeedstudio/Pion-Docs/raw/master/images/api_tips.png

[API Wiki]: http://www.seeedstudio.com/wiki/Grove_System

[Android App in Github]: http://www.seeedstudio.com/wiki/Grove_System

[iOS App in Github]: http://www.seeedstudio.com/wiki/Grove_System