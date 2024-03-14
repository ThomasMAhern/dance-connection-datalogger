# dance-connection-datalogger
Device that records pressure-sensor and gyro data during a dance to evaluate and characterize tension and compression during a partner dance.

You'll have to solder some of the components together, and then load the code onto the Adalogger via [Arduino IDE](https://www.arduino.cc/en/software) + micro usb. You can follow [this guide](https://github.com/ThomasMAhern/dance-connection-datalogger/blob/main/A%20guide%20to%20testing_%20connecting%20and%20completing%20the%20project..pdf).


## Parts required:
* $20 - [Adafruit Feather M0 Adalogger](https://www.adafruit.com/product/2796)
* $12 - [Adafruit LSM6DSOX 6 DoF Accelerometer and Gyroscope](https://www.adafruit.com/product/4438)
* $1 - [Through-Hole Resistors - 10K ohm 5% 1/4W](https://www.adafruit.com/product/2784)
* $7 - [LIPO Battery w JST connector - 3.7V 400mAh](https://www.adafruit.com/product/3898) - ensure correct JST polarity - you'll kill the Adalogger :(
* $4 - [Force-Sensitive Resistor (FSR)](https://www.adafruit.com/product/166) (still testing out the best ones, but 20kg is best so far)
* $1 - [Stemma QT JST SH 4-Pin 1.0mm pitch Cable](https://www.adafruit.com/product/4399)
* $9 - [MicroSD card](https://www.adafruit.com/product/1294) - format to ExFAT32, some don't work with the Adalogger **(3hrs = 27MB)**
   * Amazon Basics v30 ✅
   * Gigastone v30 ✅
   * Prograde v60 ✅
   * Verbatim V10 ✅
   * Kootion ❌
   * Netac V10 ✅

## Soldering kit:
If you're new to soldering, I would recommend: 
* $26 - [Pinecil USB-C powered Soldering Iron](https://pine64.com/product/pinecil-smart-mini-portable-soldering-iron/) (I think it requires a 60W USB-C PD cable)
* $11 - [TS-BC2 soldering tip](https://a.co/d/acchofP)
* $40 - [KESTER SOLDER 24-6337-0027 Solder Wire](https://a.co/d/aGZpqEn) (leaded solder is SO much easier to work with)
* $38 - [Omnifixio OF-S2 third hand](https://omnifixo.com/collections/all) (not required, but holds components in place during soldering)

## About the data:
Once you've made some recordings, I use [this Jupyter Notebook](https://github.com/ThomasMAhern/dance-connection-datalogger/blob/main/Dance_Connection_Datalogger_Code.ipynb) to analyze the data and get the interactive graphs.

Here is a short recording showing 8 claps for sync, and then light, medium, and heavy connection against a doorframe:
![Screen Shot 2024-03-14 at 16 02 28](https://github.com/ThomasMAhern/dance-connection-datalogger/assets/33540039/86d82798-1156-4c98-8a1e-156c65f7063d)


You want to use KT tape to secure the sensor to your finger. The elastic band I tried kept moving/slipping during even sugar tucks. You can see the result in the 3rd graph as the band kept needing to be adjusted (in this case I feel like it was slowly wrapping around my finger causing slightly more tension:
![Screen Shot 2024-03-12 at 23 06 51](https://github.com/ThomasMAhern/dance-connection-datalogger/assets/33540039/9dc9c643-998c-4477-b68d-d90084f3cd52)

These graphs show a single dance, where it kept moving and had to adjust it halfway through - thus ruining a good baseline:
![Screen Shot 2024-03-12 at 23 07 02](https://github.com/ThomasMAhern/dance-connection-datalogger/assets/33540039/8c30f41a-0a4a-470f-8761-382b20e98b56)

Contrasted to the first night where I used KT tape, while it loosened up and I needed to adjust it in the beginning, it stayed relatively constant afterwards (This was also using a 6kg sensor):
![Screen Shot 2024-03-12 at 23 18 52](https://github.com/ThomasMAhern/dance-connection-datalogger/assets/33540039/e3d07c07-26d8-4aab-be41-45c5a14cb107)




## Images:
Complete with 200mAh battery:
![WhatsApp Image 2024-03-12 at 23 26 24 (1)](https://github.com/ThomasMAhern/dance-connection-datalogger/assets/33540039/b4a50347-50c0-482c-90c7-218251f08d90)
![WhatsApp Image 2024-03-12 at 23 26 24](https://github.com/ThomasMAhern/dance-connection-datalogger/assets/33540039/1b0de71c-5428-4dd4-aa13-6f9be76132c0)
![Screen Shot 2024-03-13 at 01 27 17](https://github.com/ThomasMAhern/dance-connection-datalogger/assets/33540039/ed911205-8805-4879-a1c1-979ba12cbfac)


#### Future ideas: 
* Show difference between beginner/experienced connection smoothness
* Classify different patterns based on Accelerometer + Gyro readings
* Vector Database showing which pro your connection/patterns/etc. are most similar to
* Quantify connection quality during comps
