# JTAG

## Schritt\_01:

jetzt richten wir JTAG ein.

https://docs.espressif.com/projects/esp-idf/en/v4.4.3/esp32/api-guides/jtag-debugging/configure-ft2232h-jtag.html

https://docs.espressif.com/projects/espressif-esp-iot-solution/en/latest/hw-reference/ESP-Prog_guide.html

https://docs.espressif.com/projects/esp-idf/en/stable/esp32/api-guides/jtag-debugging/index.html

![Schritt_01](https://raw.githubusercontent.com/Meisterschulen-am-Ostbahnhof-Munchen/Install-ISOBUS-Environment-docs/main/images/JTAG/Schritt_01.png)

![Schritt_01a](https://raw.githubusercontent.com/Meisterschulen-am-Ostbahnhof-Munchen/Install-ISOBUS-Environment-docs/main/images/JTAG/Schritt_01a.jpeg)

![Schritt_01b](https://raw.githubusercontent.com/Meisterschulen-am-Ostbahnhof-Munchen/Install-ISOBUS-Environment-docs/main/images/JTAG/Schritt_01b.jpeg)

Diese Pins werden mindestens gebraucht:

![](https://user-images.githubusercontent.com/69573151/203024137-ff74b56a-aa9c-4492-a743-da31df66fcb3.png)

![Schritt_01c](https://raw.githubusercontent.com/Meisterschulen-am-Ostbahnhof-Munchen/Install-ISOBUS-Environment-docs/main/images/JTAG/Schritt_01c.jpeg)

![](https://user-images.githubusercontent.com/69573151/203024448-ca6c2e56-4927-4140-aa36-bdfda1c0fcc1.png)

![](https://user-images.githubusercontent.com/69573151/203026388-1db50d10-e977-4246-aa9e-0755429acaee.png)

https://docs.espressif.com/projects/esp-idf/en/latest/api-guides/jtag-debugging/configure-other-jtag.html

## Schritt\_02:

openocd --version

![Schritt_02](https://raw.githubusercontent.com/Meisterschulen-am-Ostbahnhof-Munchen/Install-ISOBUS-Environment-docs/main/images/JTAG/Schritt_02.png)

## Schritt\_03:

https://docs.espressif.com/projects/esp-idf/en/v4.0-beta2/api-guides/jtag-debugging/index.html

openocd -f interface/ftdi/esp32\_devkitj\_v1.cfg -f board/esp-wroom-32.cfg

https://docs.espressif.com/projects/esp-idf/en/v4.0-beta2/api-guides/jtag-debugging/index.html

falsch: openocd -f board/esp32-wrover-kit-3.3v.cfg

falsch: https://docs.espressif.com/projects/esp-idf/en/latest/api-guides/jtag-debugging/index.html

![Schritt_03](https://raw.githubusercontent.com/Meisterschulen-am-Ostbahnhof-Munchen/Install-ISOBUS-Environment-docs/main/images/JTAG/Schritt_03.png)

## Schritt\_04:

https://docs.espressif.com/projects/esp-idf/en/latest/api-guides/jtag-debugging/debugging-examples.html#jtag-debugging-examples-eclipse

https://docs.espressif.com/projects/esp-idf/en/latest/api-guides/jtag-debugging/using-debugger.html#jtag-debugging-using-debugger-eclipse

![Schritt_04](https://raw.githubusercontent.com/Meisterschulen-am-Ostbahnhof-Munchen/Install-ISOBUS-Environment-docs/main/images/JTAG/Schritt_04.png)

## Schritt\_05:

![Schritt_05](https://raw.githubusercontent.com/Meisterschulen-am-Ostbahnhof-Munchen/Install-ISOBUS-Environment-docs/main/images/JTAG/Schritt_05.png)

## Schritt\_06:

![Schritt_06](https://raw.githubusercontent.com/Meisterschulen-am-Ostbahnhof-Munchen/Install-ISOBUS-Environment-docs/main/images/JTAG/Schritt_06.png)

## Schritt\_07:

![Schritt_07](https://raw.githubusercontent.com/Meisterschulen-am-Ostbahnhof-Munchen/Install-ISOBUS-Environment-docs/main/images/JTAG/Schritt_07.png)
