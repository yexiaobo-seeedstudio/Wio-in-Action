 
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
Start to add your first Pion One, please check the operation video. 

**Android:**

< 视频内容：1. 需要 Pion One 和 Android 手机同时出现在视频。2. 点击 + 后进入连引导页面。3. 长按 3 秒Pion One 的功能键。4. 输入SSID 和 PWD。5. 完成>

<video width="400" height="711" controls>
  <source src="/Users/xiaobo/Desktop/Pion One/video/smartconfig.mp4" type="video/mp4">
Your browser does not support the video tag.
</video>

**iOS:**

Coming soon.
 
#### Step 4: Setup You Pion One on Mobile App and Updating Firmware
Finally, we connect the Pion One with internet; we will animate it now.

Press the Wi-Fi-connected Pion One in APP, start to configure.

**Android:**

< 视频内容：1. 需要 Pion One 和 Android 手机同时出现在视频。2. 点击刚刚连接上网络的 Pion One。3. 点击 Pion One 左上角的 Grove 接口。4. 在 App 下边选择 Output。5. 选择 Grove - temp&humidity pro 模块。 6. 点击 App 右下角的 勾，确定。7. 点击右上角的 Update Firmware。8. 等待更新完成。>

**iOS:**

Coming soon.

#### Step 5: Plug Grove Temp&Humidity Sensor to Pion One
Pion One has 6 Grove connectors, compatible with most of the Grove modules. We need a Grove-Temp & Humidity Pro module in this tutorial, it is a multifunctional sensor that gives you temperature and relative humidity information at the same time.

Firstly, please plug the Grove-Temp & Humidity Pro module to the left corner (near to LED light) of Pion One. 

￼<img src="https://github.com/yexiaobo-seeedstudio/Pion-Docs/raw/master/images/connected_grove-temp.jpg" width="500" height="650" frameborder="0" alt="" style="max-width:100%;">

#### Step 6: Pion One is Get Ready
Well, Pion One has become a device that is connected to Wi-Fi and can acquire the temperatures&huminity of surroundings, which is an IoT hardware device.

As I said，We just build an IoT devices in 5 minutes. 

Each Grove module connected to Pion One can be visited by URL，and carry out Write，Read operations，similar to HTTP.  Sometimes we call them **Web of Things** devices too.

Press the ** Tips button with 3 dots ** on the right side of Pion One, and then press ** Detail **， we will see the picture as below.

￼￼<img src="https://github.com/yexiaobo-seeedstudio/Pion-Docs/raw/master/images/details.png" width="400" height="730" frameborder="0" alt="" style="max-width:100%;">

Open the link, we can see all the available Grove Modules information, include how to visit, and the parameters each Grove Module support, ect. It is the same link information in QR Code.

￼￼<img src="https://github.com/yexiaobo-seeedstudio/Pion-Docs/raw/master/images/api_tips.png" width="400" height="730" frameborder="0" alt="" style="max-width:100%;">

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

- **IFTTT**:

Please to visit **`Demos`** section to get more IFTTT demos.

- **Your Application**:

All the returned data visited by URL are JSON format, so you can integrate Pion One as a platform independent device to any other applications.

We are expecting your masterpieces!  More projects please visit **``Showcases**.

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

### What is Grove

**Grove** is a modulated, ready-to-use tool set. Much like Lego, it takes a building block approach to assembling electronics. Compared with the traditional, complicated learning method of using a breadboard and various electronic components to assemble a project, Grove simplifies and condenses the learning process significantly.  Every Grove module addresses a single function, such as a simple button or a more complex heart rate sensor.

There are more than 150+ Grove modules, more details about Grove System, please visit [Grove Wiki][Grove Wiki].

< 插入 Grove 图：一张预览图 >

### Pion One Modes

- Config Mode

	<iframe src="https://player.vimeo.com/video/138398577" width="500" height="281" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>

- Requesting IP from Router
	
	<iframe src="https://player.vimeo.com/video/138397446" width="500" height="281" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>
	
- Connecting to The Server
	
	<iframe src="https://player.vimeo.com/video/138397448" width="500" height="281" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>
	
- Over-The-AIr(OTA), upgrade firmware
	
	<iframe src="https://player.vimeo.com/video/138397455" width="500" height="281" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>
	
- Connected Cloud
	
	<iframe src="https://player.vimeo.com/video/138399063" width="500" height="281" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>
	
### Pion One and Grove
Pion One supports 4 types connector of Grove：`I2C`，`Digital IO`，`Analog IO`，`UART`。

￼![][pionone-grove]

### Lightweight Server/Cloud

## Workflow of Pion One
###Hardware is Out-of-Box
###Grove is Plug&Play, without soldering
  
## Mobile App
###Features (要有 Android 和 iOS App 截
  - Smart Config(TM), AP Config
  - Visual Configuration
  - Device Management

## Accessing Grove Sensors and Actuators
### Command Line （Curl 和 Python 脚本演示）
### IFTTT （引用 Demo 项目）
### Node-Red （待定）
### Web App （用 Rails 写个简单的 App）
### Your Application and More (引用 Demo 项目）

## Cloud
### Lightweight Server
  - Cloud Compile and Over-The-Air(OTA) Upgrade
  - Account Management
  - URL routing
### Thirty Cloud Services
  
[Grove Wiki]: http://www.seeedstudio.com/wiki/Grove_System

[pionone-grove]: https://github.com/yexiaobo-seeedstudio/Pion-Docs/raw/master/images/pionone-grove.png

[connected_grove-temp]: https://github.com/yexiaobo-seeedstudio/Pion-Docs/raw/master/images/connected_grove-temp.jpg

[details]: https://github.com/yexiaobo-seeedstudio/Pion-Docs/raw/master/images/details.png

[api_tips]: https://github.com/yexiaobo-seeedstudio/Pion-Docs/raw/master/images/api_tips.png
