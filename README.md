# dance-connection-datalogger
Device that records pressure-sensor and gyro data during a dance to evaluate and characterize tension and compression during a partner dance.


Parts required:
1. $20 - [Adafruit Feather M0 Adalogger](https://www.adafruit.com/product/2796)
2. $12 - [Adafruit LSM6DSOX 6 DoF Accelerometer and Gyroscope](https://www.adafruit.com/product/4438)
3. $1 - [Through-Hole Resistors - 10K ohm 5% 1/4W](https://www.adafruit.com/product/2784)
4. $7 - [LIPO Battery w JST connector - 3.7V 400mAh](https://www.adafruit.com/product/3898) - ensure correct JST polarity - you'll kill the Adalogger :(
5. $9 - [MicroSD card](https://www.adafruit.com/product/1294) - format to ExFAT32, some don't work with the Adalogger **(3hrs = 27MB)**
   * Amazon Basics v30 ✅
   * Gigastone v30 ✅
   * Prograde v60 ✅
   * Verbatim V10 ✅
   * Kootion ❌
   * Netac V10 ✅
7. $4 - [Force-Sensitive Resistor (FSR)](https://www.adafruit.com/product/166) (still testing out the best ones, but 20kg is best so far)


You want to use KT tape to secure the sensor to your finger. The elastic band I tried kept moving/slipping during even sugar tucks. You can see the result in the 3rd graph as the band kept needing to be adjusted (in this case I feel like it was slowly wrapping around my finger causing slightly more tension:
![Screen Shot 2024-03-12 at 23 06 51](https://github.com/ThomasMAhern/dance-connection-datalogger/assets/33540039/9dc9c643-998c-4477-b68d-d90084f3cd52)

These graphs show a single dance, where it kept moving and had to adjust it halfway through - thus ruining a good baseline:
![Screen Shot 2024-03-12 at 23 07 02](https://github.com/ThomasMAhern/dance-connection-datalogger/assets/33540039/8c30f41a-0a4a-470f-8761-382b20e98b56)

Contrasted to the first night where I used KT tape, while it loosened up and I needed to adjust it in the beginning, it stayed relatively constant afterwards (This was also using a 6kg sensor):
![Screen Shot 2024-03-12 at 23 18 52](https://github.com/ThomasMAhern/dance-connection-datalogger/assets/33540039/e3d07c07-26d8-4aab-be41-45c5a14cb107)





Complete with 200mAh battery:
![WhatsApp Image 2024-03-12 at 23 26 24 (1)](https://github.com/ThomasMAhern/dance-connection-datalogger/assets/33540039/b4a50347-50c0-482c-90c7-218251f08d90)
![WhatsApp Image 2024-03-12 at 23 26 24](https://github.com/ThomasMAhern/dance-connection-datalogger/assets/33540039/1b0de71c-5428-4dd4-aa13-6f9be76132c0)
