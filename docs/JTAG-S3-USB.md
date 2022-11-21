# JTAG-S3-USB

[https://docs.espressif.com/projects/esp-idf/en/latest/esp32s3/api-guides/jtag-debugging/index.html](https://docs.espressif.com/projects/esp-idf/en/latest/esp32s3/api-guides/jtag-debugging/index.html)

openocd --version

![](https://user-images.githubusercontent.com/69573151/203045056-0c215f49-db0d-4015-a5c4-3ee519a8e02f.png)

openocd -f board/esp32s3-builtin.cfg

![](https://user-images.githubusercontent.com/69573151/203045142-a7128ca7-d41a-45e5-8d12-f585134d4ae2.png)

wenn wie oben der Text kommt: 

Error: libusb\_open() failed with LIBUSB\_ERROR\_NOT\_SUPPORTED

dann bitte diesen Treiber installieren:

[https://dl.espressif.com/dl/idf-driver/idf-driver-esp32-usb-jtag-2021-07-15.zip](https://dl.espressif.com/dl/idf-driver/idf-driver-esp32-usb-jtag-2021-07-15.zip)

TODO: woher weiß ich dass das der aktuelle ist ? 

![](https://user-images.githubusercontent.com/69573151/203050292-1710c660-14cf-44aa-9ada-a7983bdb8654.png)

![](https://user-images.githubusercontent.com/69573151/203045621-d08ba43d-fca0-4416-8fe8-b55c00724ff2.png)

![](https://user-images.githubusercontent.com/69573151/203046659-9083d6ed-055f-43fa-8976-bc81bbed79de.png)

![](https://user-images.githubusercontent.com/69573151/203046810-44c4c2d4-237c-462c-9430-acbdf775b092.png)

![](https://user-images.githubusercontent.com/69573151/203046882-e9b0c9d0-0f04-461c-bd2d-20bd0f862466.png)

dann läuft es nicht, es muss folgende Einstellung geändert werden:

![](https://user-images.githubusercontent.com/69573151/203047161-4cc44700-bf47-4987-befd-a3b6d3c98a4b.png)

ESP32-S3 chip (via ESP USB Bridge)

![](https://user-images.githubusercontent.com/69573151/203047309-0cb01fdf-270d-466b-9cfa-3ff82b325a6b.png)

bringt im Moment folgendes:

![](https://user-images.githubusercontent.com/69573151/203048056-01a71651-e9fb-4f04-bf82-f1fe34db9bef.png)
