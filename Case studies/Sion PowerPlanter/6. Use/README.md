## User guide of EPS32

#### 1. Description of product
 
  * Name of product: EPS32
     
 #### 2. Use of product
 
  * Materials required
      * Software
   
  * Procedure
  
     * Install the software:
      
  To install the software on the EPS32 you can use the free "Arduino IDE". If you don't have it, you can get it here for free: https://www.arduino.cc  /en/software

  Load the code (powerplant.ino, version number may vary, higher is better) from GitHub:
https://github.com/munichseb/powerplant and open it in the Arduino IDE.

  Connect the ESP32 to your computer, and select the correct device in the "Tools" section. It should look like this:
  
 [Selection of the correct device in the "Tools" section](https://wikifactory.com/files/RmlsZTo1NzE4NDc=)
 
 ![image](https://user-images.githubusercontent.com/59058909/122737358-3fec5880-d281-11eb-81fd-1ac220b75c09.png)

 
 If the "Wemos D1" is not avilable, go to "Board administation" in the same menu, and install the ESP32 set. Make sure the "Port" selection is pointing to the device (there is one selection in the list that looks weird, this is the one).

Now comes a very important step: click on "Tools" / "Serial Monitor" and open the serial monitor. It will open a second window. Leave it like it is.

Click on "upload" in the IDE, and the sketch will be uploaded. Your device should reset and the LEDs should shine in magenta. Congrats! You have a working Powerplanter device!

Now head to the serial monitor window. You should see a line like this:

Device ID: SINSLRCR

The 10 digit code it your unique device ID. Write it down. Copy it and send it to you via E-Mail. This is an important key to your device.
    
   * Setup instruction: 
    
 When the device is shining in magenta, it means that everything is fine, but it cannot connect to the internet. To get it online, use your smartphone or your tablet (Android, iOS, all fine) and look for a new wifi network you have not seen before. The new network is from your powerplanter device.

If you connect to it, it will present you a configuration interface:

![image](https://user-images.githubusercontent.com/59058909/122736953-d8cea400-d280-11eb-9bfe-d77c418d32dd.png)

Select "Configure Wifi (Auto Scan)" to get a list of all available WiFi-Networks the device can see.

![image](https://user-images.githubusercontent.com/59058909/122737180-129faa80-d281-11eb-92ee-429594199952.png)

Pick your WiFi, enter your credentials. The device should now get online immediately. As soon as it online, the color will change from magenta to white. You are all set!

![image](https://user-images.githubusercontent.com/59058909/122737991-dfa9e680-d281-11eb-9938-0c07a54a3a42.png)


#### 3. Update of firmware

* ...

#### 4. Troubleshooting

* ...

#### 5. Repair information

* ...

#### 6. Reporting problems

* ...


## User guide of the PowerPlanter Portal

#### 1. Description of product
 
  * Name of product: PowerPlanter Porta
     
 #### 2. Use of product
 
  * Materials required
      * device
   
  * Procedure
  
     * Setup instruction: 
    
 You don't need a Sion to use the device: it can also display some other status information. By default, it will show the amount of renewable energy in the german energy grid.

https://www.sono.community/powerplanter/

You need the Device ID from step #3 to log in. After loggin in, you will see some device data, such as the internal temperature sensor. Pro Tip: Write the code on a piece of paper and stick it into the powerplanter. So you have it at hand when you need it.

![image](https://user-images.githubusercontent.com/59058909/122741587-614f4380-d285-11eb-9926-87c7fb7ff181.png)

The most fun feature is to send color patterns to the device. It should work instantly.

![image](https://user-images.githubusercontent.com/59058909/122741632-6c09d880-d285-11eb-8fc4-7c338a8ac326.png)

There are some more functions. At the bottom, you will find a custom QR-Code. You can print it and place it somewhere (inside some kitchen door?).  You can scan it with your smartphone camera, and it will open the portal without logging in.

To link the device to your Sion, you need to perform two steps:

1) Log into the Sono Motors Customer Portal. There you will find an API key. Copy it to your clipboard.
2) In the powerplanter portral, select "Sion Live Data" and enter the token.

![image](https://user-images.githubusercontent.com/59058909/122741690-7d52e500-d285-11eb-886a-1186d3ebebf1.png)

The portal will now exchange the Device ID and Sion Data, and the device will start to show your Sion live data!

#### 3. Update of firmware

* ...

#### 4. Troubleshooting

* ...

#### 5. Repair information

* ...

#### 6. Reporting problems

* ...
