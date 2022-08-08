JTAG
===================================

## Schritt\_01:

jetzt richten wir JTAG ein.

https://docs.espressif.com/projects/esp-idf/en/latest/api-guides/jtag-debugging/configure-wrover.html

https://github.com/espressif/esp-iot-solution/blob/master/documents/evaluation_boards/ESP-Prog_guide_en.md

![Schritt_01 https://raw.githubusercontent.com/Meisterschulen-am-Ostbahnhof-Munchen/Install-ISOBUS-Environment/master/images/JTAG/Schritt_01.png

![Schritt_01a https://raw.githubusercontent.com/Meisterschulen-am-Ostbahnhof-Munchen/Install-ISOBUS-Environment/master/images/JTAG/Schritt_01a.jpeg 

![Schritt_01b https://raw.githubusercontent.com/Meisterschulen-am-Ostbahnhof-Munchen/Install-ISOBUS-Environment/master/images/JTAG/Schritt_01b.jpeg 

![Schritt_01c https://raw.githubusercontent.com/Meisterschulen-am-Ostbahnhof-Munchen/Install-ISOBUS-Environment/master/images/JTAG/Schritt_01c.jpeg 

https://docs.espressif.com/projects/esp-idf/en/latest/api-guides/jtag-debugging/configure-other-jtag.html

## Schritt\_02:

openocd --version

![Schritt_02 https://raw.githubusercontent.com/Meisterschulen-am-Ostbahnhof-Munchen/Install-ISOBUS-Environment/master/images/JTAG/Schritt_02.png

## Schritt\_03:

https://docs.espressif.com/projects/esp-idf/en/v4.0-beta2/api-guides/jtag-debugging/index.html

openocd -f interface/ftdi/esp32\_devkitj\_v1.cfg -f board/esp-wroom-32.cfg

https://docs.espressif.com/projects/esp-idf/en/v4.0-beta2/api-guides/jtag-debugging/index.html

falsch: openocd -f board/esp32-wrover-kit-3.3v.cfg

falsch: https://docs.espressif.com/projects/esp-idf/en/latest/api-guides/jtag-debugging/index.html

![Schritt_03 https://raw.githubusercontent.com/Meisterschulen-am-Ostbahnhof-Munchen/Install-ISOBUS-Environment/master/images/JTAG/Schritt_03.png

## Schritt\_04:

https://docs.espressif.com/projects/esp-idf/en/latest/api-guides/jtag-debugging/debugging-examples.html#jtag-debugging-examples-eclipse

https://docs.espressif.com/projects/esp-idf/en/latest/api-guides/jtag-debugging/using-debugger.html#jtag-debugging-using-debugger-eclipse

![Schritt_04 https://raw.githubusercontent.com/Meisterschulen-am-Ostbahnhof-Munchen/Install-ISOBUS-Environment/master/images/JTAG/Schritt_04.png

## Schritt\_05:

![Schritt_05 https://raw.githubusercontent.com/Meisterschulen-am-Ostbahnhof-Munchen/Install-ISOBUS-Environment/master/images/JTAG/Schritt_05.png

## Schritt\_06:

![Schritt_06 https://raw.githubusercontent.com/Meisterschulen-am-Ostbahnhof-Munchen/Install-ISOBUS-Environment/master/images/JTAG/Schritt_06.png

## Schritt\_07:

![Schritt_07 https://raw.githubusercontent.com/Meisterschulen-am-Ostbahnhof-Munchen/Install-ISOBUS-Environment/master/images/JTAG/Schritt_07.png