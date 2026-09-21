# Internet Radio

ESP32 Internet Radio - This is a fully functional Internet Radio Based on ESP32-S3 
**Features:**
- Internet radio streaming
- Touchscreen and rotary encoder control
- Web-based configuration
- Hundreds of thousands of stations to choose from
- 1000 stations in your favorites list
- MP3, AAC, FLAC, Vorbis and other audio formats
- Bluetooth audio transmitter
- ESP32-S3 and ESP32-P4 support
<br>

**Interested in building your own Internet Radio ?**

**Firmware, DIY kits, and fully assembled units are available at:** [https://tmicromaker.com/](https://tmicromaker.com/shop-2/)

<br>
<br>


**There are few versions avaliable:**

Version with Rotary Encoder or Touch Screen:

![IMG_4870](https://github.com/user-attachments/assets/27eed72e-b462-4414-9c2e-7d4f0acef384)

<br>

Version with touch screen:

<img width="4032" height="2268" alt="IMG_5058" src="https://github.com/user-attachments/assets/e66cb312-404b-45b1-9e0c-250ae0f83afa" />


![IMG_3577](https://github.com/user-attachments/assets/19e128bc-b9b6-4e2b-bd15-aea5ab638663)
![IMG_3576](https://github.com/user-attachments/assets/ca0a1ff1-3cd8-4685-a9a8-28e3d01f89e3)

<br>

Version with only Rotary Encoder (no option for touch screen):

<img width="4032" height="2268" alt="IMG_4994" src="https://github.com/user-attachments/assets/b02f5701-7adf-4c5c-8062-8f69f8b3f6c6" />

<br>
<br>
Version Based on ESP32-P4 with SPDIF out and WebUi Management Interface

![IMG_4602](https://github.com/user-attachments/assets/404d861e-c2d5-45e2-b299-c588e6edba75)

<br>
<br>

A repository where you can find documantation, various firmware version and enclosures 3D files, : 
https://tinyurl.com/4yduvmdj

<br>

For any quations Email me to: tmicromaker@gmail.com

Note: The Radio was designed to work only with ESP32S3 Lilygo t-displayS3 family

<br>
<br>

You can watch the Radio various versions and evolution here:

**https://www.youtube.com/@tmicromaker**


<br>
<br>

**Firmware Installation:**


1. In your web prowser open:  https://tmicromaker.com/MicroMaker_WebFlasher.html

<img width="642" height="1010" alt="firmware" src="https://github.com/user-attachments/assets/515fc0c8-b4f9-4527-b8c0-5d6a3a94a92c" />

2. Connect your microcontroller to the USB port of your computer.

3. Put the microcontroller in boot mode
   - Hold BOOT.
   - Press and release RESET.
   - Keep holding BOOT for another second or two.
   - Release BOOT.

4. Enter your email address and press continue

5. Press connect choose the right port and flash.

6. Press Install firmware

7. Wait for the upload to finish

8. Restart the microcontroller and wait (it takes about 1~1.5 minutes to boot up on the first time).

<br>
<br>

**Radio Operation:**

After flashing is finished:

1. Press the RESET button on the ESP board (if it does not reboot automatically).
The new firmware will start running.

3. After ESP32 boot wait for arround 1 min until network scanning is completed.

4. Open the wifi in your phone or computer and search for BT_Radio

5. Connect to your network

6. Have a look at the LCD for the IP address

7. Connect to that IP address using your computer browser

8. Upload a single station or list of stations using the following format

Station Name 1,Station Address 1

Station Name 2,Station Address 2

Radio Space,http://123.456.789.0/stream

Radio Hits,http://stream.awesomehitsradio.com
.
Note: An I2S DAC is required for this project, Amplifier is optional.  Consult the I2S data sheet to learn how to activate the (L+R)/2 or stereo signal.  

Note: for some stations that don't play and their URL starts with https:// try to change it to http:// and check if it is working

<br>
<br>

**DIY Instructions:**

Connection diagram using the Max98357a chip (if you use a header you don't need to connect wires as the pins are arranged correctly). 
I strongly recommend using the PCM5102a for better sound quality.      
 
Connect the I2S DAC to the following pins: 
BCLK to pin 12, 
LRC to pin 11, 
DOUT to pin 13,
VCC to 5V,
GND to GND

Following is the connection diagram:
![2000](https://github.com/Arielhh/ESP32-Radio-Internet/assets/4849568/eb7a9487-50be-4602-b988-5af08c9675d4)

Just solder it like that and connect it to the speaker (the pins are already aligned with the DAC pins):


![2001](https://github.com/Arielhh/ESP32-Radio-Internet/assets/4849568/cfae9a96-6d9e-48fd-bd41-e1cd02ca62a5)


![image](https://github.com/Arielhh/ESP32-Radio-Internet/assets/4849568/d405b0ce-b7a1-45ff-980c-08a1a25e7c60)
![image](https://github.com/Arielhh/ESP32-Radio-Internet/assets/4849568/d6fd0191-0bdb-4603-8089-db5a063e00e1)

Module designed by the MicroMaker which combines DAC + AMP + Bluetooth in one module and is being controlled directlly by the microcontroller 
<img width="1536" height="1024" alt="ChatGPT Image Sep 4, 2026, 03_16_44 PM" src="https://github.com/user-attachments/assets/62a63f19-e903-45d7-88f0-5eef8f5e518b" />


Optional Pam8406 amplifier 2x6w amp+ pcm5102a Stereo DAC on one PCB which can be mounted directlly on top of the LILYGO T-Display Touch S3 (no wires soldering needed)
![pam](https://github.com/user-attachments/assets/7c26c655-e0bc-49e2-af36-5a40c3ad6195)


You can watch the videos by clicking on the below videos:


[![▶ Watch the video](https://i9.ytimg.com/vi_webp/UsdidMPg164/mqdefault.webp?v=69a4ca24&sqp=CKCTk80G&rs=AOn4CLAiW8gmMZz_3K2KjQ3we_rY3myKoQ)](https://youtu.be/UsdidMPg164)


[![▶ Watch the video](https://i9.ytimg.com/vi_webp/jb2SspnF-nk/mqdefault.webp?v=69a4c9dd&sqp=CKSak80G&rs=AOn4CLA0-gdPMe77tKCUpStJ2oLFzjOb8A)](https://youtu.be/jb2SspnF-nk)
















