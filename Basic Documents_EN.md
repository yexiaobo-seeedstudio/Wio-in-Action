 
## Getting Started: Build a Temp&Humidity IoT Device in 5 Minutes
#### Step 1: Plug Grove Temp&Humidity Sensor to Pion One
Pion One has 6 Grove connectors, compatible with most of the Grove modules. We need a Grove-Temp & Humidity Pro module in this tutorial, it is a multifunctional sensor that gives you temperature and relative humidity information at the same time.
 
Firstly, please plug the Grove-Temp & Humidity Pro module to the left corner (near to LED light) of Pion One. 
![][image-1]
￼

#### Step 2: Installing Android/iOS App
You need to install an Android(链接) or iOS(链接) App to manage and configure Pion One device.

**Android:**
Please make sure your OS version is Android 4.1 or later, search in Google Play and install Pion One.
\< 需要 Google Play 搜索截图 \>
 
**iOS:**
\< 需要 App Store 搜索截图 \>
OS Version requires iOS 7 or later, please find Pion One in App Store and then install it.
 
#### Step 3: Creating You Account
When you use the Android/iOS App for the first time, you need to sign up an account to manage your Pion One Devices.
\< signup.mp4 \>
 
#### Step 4: Connecting Pion One to WiFi AP
开始添加你的第一个 Pion One，请看操作视频。
Start to add your first Pion One, please check the operation video.
 
**Android:**
\< 视频内容：1. 需要 Pion One 和 Android 手机同时出现在视频。2. 点击 + 后进入连引导页面。3. 长按 3 秒Pion One 的功能键。4. 输入SSID 和 PWD。5. 完成\>
 
**iOS:**
\< 视频内容：1. 需要 Pion One 和 iPhone 手机同时出现在视频。2. 点击 + 后进入连引导页面。3. 长按 3 秒Pion One 的功能键。4. 退出 Pion One，打开 Setting，连接 PionOne-xxx。5. 重新打开 Pion One 输入SSID 和 PWD。5. 完成\>
 
#### Step 5: Setup You Pion One on Mobile App and Updating Firmware
我们终于让 Pion One 连接上网络了，现在要赋予它生命。
Finally, we connect the Pion One with internet; we will animate it now.
 
在 App 界面上点击刚刚连接上网络的 Pion One，开始配置：
Press the Wi-Fi-connected Pion One in APP, start to configure.
 
**Android:**
\< 视频内容：1. 需要 Pion One 和 Android 手机同时出现在视频。2. 点击刚刚连接上网络的 Pion One。3. 点击 Pion One 左上角的 Grove 接口。4. 在 App 下边选择 Output。5. 选择 Grove - temp&humidity pro 模块。 6. 点击 App 右下角的 勾，确定。7. 点击右上角的 Update Firmware。8. 等待更新完成。\>
 
**iOS:**
\< 视频内容：1. 需要 Pion One 和 iPhone 手机同时出现在视频。2. 点击刚刚连接上网络的 Pion One。3. 点击 Pion One 坐上角的 Grove 接口。4. 在 在弹出的列表中选择 Grove - temp&humidity pro 模块。 6. 点击右上角的 Update Firmware。8. 等待更新完成。\>
 
#### Step 6: Pion One is Get Ready
Well，现在 Pion One 已经变成了一个联网，且能获取周围环境温湿度的设备——也就是一款物联网硬件设备。
Well, Pion One has become a device that is connected to Wi-Fi and can acquire the temperatures of surroundings, which is an IoT hardware device.
 
As I said，We just build an IoT devices in 5 minutes.
 
每个 Pion One 所连接的 Grove 模块都可以通过 URL 连接访问，可以执行：Write, Read，与 HTTP 协议类似。所以有时候我们也会称呼它们为 Web of Things devices.
Each Grove module connected to Pion One can be visited by URL, and carry out Write, Read operations， similar to HTTP. Sometimes we call them Web of Things devices too.
 
点击 Pion One 列表右边的 ** 3 个小点的提示按钮 **。然后再点击 ** Detail **，我们就会看到下面的图：
\< Detail 图片 \>
Press the  ** Tips button with 3 dots ** on the right side of Pion One, and then press ** Detail **， we will see the picture as below.
 
￼

打开链接，可以看到所有能访问的 Grove 模块信息，包括如何访问，以及每个 Grove 模块支持的参数，等等。QR Code 里的信息也是同一个链接。
\< 打开 URL 的浏览器图片 \>
Open the link, we can see all the available Grove Modules information, include how to visit, and the parameters each Grove Module support, ect. It is the same link information in QR Code.
 
￼

#### Step 7: Accessing Grove Temp&Humidity Sensor
Now，lets try to get temperature and humidity via URL.
 
1. Command Line:
_Temperature_:
`$> curl -H "Authorization: token Your Token" https://iot.seeed.cc/v1/node/GroveTempHum/humidity`
Result:
`{result: 200, temp: 28}`
 
_Humidity_:
`curl -H "Authorization: token 962a6d7dca54bc4cbf01b9fc92bb49cc" https://iot.seeed.cc/v1/node/GroveTempHum/humidity`
Result:
`{result: 200, humidity: 28}`
 
2. IFTTT:
Please to visit ** Demos ** section to get more IFTTT demos.
 
3. Your Application:
通过 URL 访问所返回的数据都是 JSON 格式（JSON format），所以你可以把 Pion One 做为平台无关的设备集成到任何应用中。
All the returned data visited by URL are JSON format, so you can integrate Pion One as a platform un-related device to any other applications.
 
 
我们期待你的杰作！更多项目请访问 **Showcases**.
#### What next?
你不用焊接，也不用编程，在 5 分钟内构建了一个 IoT device. 
 
但是，接下来我们能干什么呢？以下方向可以参考：
We are expecting your masterpieces!  More projects please visit **Showcases**.
You can build an IoT device in 5 minutes without soldering or programming.
But, what can we do next? You can refer to the following directions. 
 
1. 集成到你现有的项目中。
2. 结合其他云服务，构建完整的 IoT Application。
3. 与其他 Web Services 构建你的 IoT Node devices，比如使用 Github Hook Services，Twitter API 等服务。
4. etc and 其他你认为好玩的事情 :)
1.Integrate to your existing projects.
2. Combine with other Cloud service to build a complete IoT Application.
3.Build your IoT Node devices with other Web Services. For example, how to use Github Hook Services, Twitter API and other services.
4.Other things that you find  interesting.
 
如果你想了解 Pion One 详细的信息，请访问** Pion One Basic Documents **.  如果你是开发者，想了解背后的技术细节，请访问** Pion One Advanced Documents ** 和** Tools and Services **.  更多的 Demo，请访问 ** Demos ** 和 ** Showcases **.
If you want to know more details about Pion One, please visit ** Pion One Basic Documents **.If you are a developer and want to know more technical detail , please visit ** Pion One Advanced Documents ** and ** Tools and Services **.More Demos, please visit  ** Demos ** 和 ** Showcases **.
 
 
## Introduction
- What is Pion One
**Pion One** is a Wi-Fi development board to build connected IoT projects with Groves. 
 
It’s based on ESP8266 Wi-Fi SoC, supporting a lot of Grove modules. 
 
Simplify your development of IoT devices without requirements of hardware programming or soldering.
 
\< 插入 Pion One 矢量图：每一部分做介绍。\>
 
- What is Grove
**Grove** is a modulated, ready-to-use tool set. Much like Lego, it takes a building block approach to assembling electronics. Compared with the traditional, complicated learning method of using a breadboard and various electronic components to assemble a project, Grove simplifies and condenses the learning process significantly.  Every Grove module addresses a single function, such as a simple button or a more complex heart rate sensor.
 
There are more than 150+ Grove modules, more details about Grove System, please visit [wiki.seeed.cc]()[1]().
 
\< 插入 Grove 图：一张预览图 \>
- Pion One Modes
	 
\< 需要几个 Pion One 的实物 gif 图，演示各种模式：LED 灯的不同闪烁代表的意思\>
 
- Pion One and Grove
Pion One 支持 4 中类型的 Grove 接口：I2C，Digital IO，Analog IO，UART。
![]()[image-1]()
 
- Lightweight Server/Cloud
## Workflow of Pion One
- Hardware is Out-of-Box
- Grove is Plug&Play, without soldering
	 
## Mobile App
- Features (要有 Android 和 iOS App 截图）
    - Smart Config(TM)
    - Visual Configuration
    - Device Management
## Accessing Grove Sensors and Actuators
- Command Line （Curl 和 Python 脚本演示）
- IFTTT （引用 Demo 项目）
- Node-Red （待定）
- Web App （用 Rails 写个简单的 App）
- Your Application and More (引用 Demo 项目）
## Cloud
- Lightweight Server
    - Cloud Compile and Over-The-Air(OTA) Upgrade
    - Account Management
    - URL routing
- Thirty Cloud Services
	 
[1]():    http://www.seeedstudio.com/wiki/Grove_System
 
[image-1]():  file:///Users/xiaobo/Desktop/Pion%20One/content.png



[image-1]:	file:///Users/xiaobo/Desktop/Pion%20One/F411E2374D5EB409B1F072AE0505974C.jpg