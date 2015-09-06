 
## Getting Started: Build a Temp&Humidity IoT Device in 5 Minutes
#### Step 1: Installing Android/iOS App
In this tutorial, we will build a temperature and humidity monitor with Pion One. 

Firstly, You need to install an Android(Google Play Link) or iOS(App Store Link) App to manage and configure Pion One device.

**Android:**

Please make sure your OS version is Android 4.1 or later, search in Google Play and install Pion One.

`Google Play Screeshot is coming soon`

**iOS:**

OS Version requires iOS 7 or later, please find Pion One in App Store and then install it.

`App Store Screeshot is coming soon`

#### Step 2: Creating You Account
When you use the Android/iOS App for the first time, you need to sign up an account to manage your Pion One Devices.

<iframe src="https://player.vimeo.com/video/138394370" width="400" height="711" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>

#### Step 3: Connecting Pion One to WiFi AP
Start to add your first Pion One, click the `Plus Button`.

Please check the operation video. 

**Android:**

<iframe src="https://player.vimeo.com/video/138451080" width="500" height="281" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>

**iOS:**

Coming soon.
 
#### Step 4: Setup You Pion One on Mobile App and Updating Firmware
Finally, we connect the Pion One with internet; we will animate it now.

Click Wi-Fi connected Pion One in Node list, start to configure.

**Android:**

<iframe src="https://player.vimeo.com/video/138450290" width="500" height="281" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>

**iOS:**

Coming soon.

#### Step 5: Plug Grove Temp&Humidity Sensor to Pion One
Pion One has 6 Grove connectors, compatible with most of the Grove modules. We need a Grove-Temp & Humidity Pro module in this tutorial, it is a multifunctional sensor that gives you temperature and relative humidity information at the same time.

Firstly, please plug the Grove-Temp & Humidity Pro module to the left corner (near to LED light) of Pion One. 

￼<img src="https://github.com/yexiaobo-seeedstudio/Pion-Docs/raw/master/images/connected_grove-temp.jpg" width="500" height="650" alt="Connected Grove-Temp&Huminity">

#### Step 6: Pion One is Get Ready
Well, Pion One has become a device that is connected to Wi-Fi and can acquire the temperatures&huminity of surroundings, which is an IoT hardware device.

As I said，We just build an IoT devices in 5 minutes. 

Each Grove module connected to Pion One can be visited by URL，and carry out Write，Read operations，similar to HTTP.  Sometimes we call them **Web of Things** devices too.

Press the ** Tips button with 3 dots ** on the right side of Pion One list, and then click ** Details **， we will see the picture as below.

￼￼<img src="https://github.com/yexiaobo-seeedstudio/Pion-Docs/raw/master/images/details.png" width="400" height="730" alt="Pion One Details">

Open the link, we can see all the available Grove Modules information, include how to visit, and the parameters each Grove Module support, ect. It is the same link information in QR Code.

￼￼<img src="https://github.com/yexiaobo-seeedstudio/Pion-Docs/raw/master/images/api_tips.png" width="400" height="730" alt="API Tips">

#### Step 7: Accessing Grove Temp&Humidity Sensor
Now，lets try to get temperature and humidity via URL.

 - **Command Line**:

_Temperature_:
```
$> curl -H "Authorization: token Your Token" https://iot.seeed.cc/v1/node/GroveTempHum/humidity
```

Result:
```
{result: 200, temp: 28}`
```

_Humidity_:
```
$> curl -H "Authorization: token 962a6d7dca54bc4cbf01b9fc92bb49cc" https://iot.seeed.cc/v1/node/GroveTempHum/humidity
```

Result:
```
{result: 200, humidity: 28}
```

Please visit `API Wiki` to get full API documents.

- **IFTTT**:

Please to visit **`Demos`** section to get more IFTTT demos.

- **Your Application**:

All the returned data visited by URL are JSON format, so you can integrate Pion One as a platform independent device to any other applications.

We are expecting your masterpieces!  More projects please visit **``Showcases``**.

#### What next?

Well Done. Now, you can build an IoT device in 5 minutes without soldering or programming.But, what can we do next? You can refer to the following directions. 

1.Integrate to your existing projects.

2.Combine with other Cloud service to build a complete IoT Application.

3.Build your IoT Node devices with other Web Services. For example, how to use Github Hook Services, Twitter API and other services.

4.Other things that you find interesting :)

If you want to know more details about Pion One, please visit **`Pion One Basic Documents`**.If you are a developer and want to know more technical detail , please visit **`Pion One Advanced Documents`** and **`Tools and Services`**. More Demos, please visit  **`Demos`** and **`Showcases`**.
 
## Introduction

### What is Pion One

**Pion One** is a Wi-Fi development board to build connected IoT projects with Groves. 

It’s based on ESP8266 Wi-Fi SoC, supporting a lot of Grove modules. 

Simplify your development of IoT devices without requirements of hardware programming or soldering.

< 插入 Pion One 矢量图：每一部分做介绍。>

**Pion One is Out-of-Box**

Pion One based community friendly ESP8266 WiFi SoC and Grove 这种统一和简单接口的模块化硬件，把硬件开发难度几乎降低为零。

对硬件没有一点基础知识的软件开发人员，特别是 Web developers and Android/iOS developers, 可以已一种开箱即用的方式来

Please visit **`Pion One Advanced Documents`** and **`Tools and Services`** to get total workflow of Pion One.

### What is Grove

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

```
#!/bin/sh

curl -H "Authorization: token Your Token" https://iot.seeed.cc/v1/node/GroveTempHum/humidity
```

**Python Script:**

```
import os;

def main:
	print "waiting"
```

**Ruby Script:**

```
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
- OAuth2 support
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

[Grove Wiki]: http://www.seeedstudio.com/wiki/Grove_System

[pionone-grove]: https://github.com/yexiaobo-seeedstudio/Pion-Docs/raw/master/images/pionone-grove.png

[connected_grove-temp]: https://github.com/yexiaobo-seeedstudio/Pion-Docs/raw/master/images/connected_grove-temp.jpg

[details]: https://github.com/yexiaobo-seeedstudio/Pion-Docs/raw/master/images/details.png

[api_tips]: https://github.com/yexiaobo-seeedstudio/Pion-Docs/raw/master/images/api_tips.png

[API Wiki]: http://www.seeedstudio.com/wiki/Grove_System

[Android App in Github]: http://www.seeedstudio.com/wiki/Grove_System

[iOS App in Github]: http://www.seeedstudio.com/wiki/Grove_System