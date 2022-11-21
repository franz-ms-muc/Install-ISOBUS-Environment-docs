# JTAG

## Schritt\_01:

jetzt richten wir JTAG ein.

[https://docs.espressif.com/projects/esp-idf/en/v4.4.3/esp32/api-guides/jtag-debugging/configure-ft2232h-jtag.html](https://docs.espressif.com/projects/esp-idf/en/v4.4.3/esp32/api-guides/jtag-debugging/configure-ft2232h-jtag.html)

[https://docs.espressif.com/projects/espressif-esp-iot-solution/en/latest/hw-reference/ESP-Prog_guide.html](https://docs.espressif.com/projects/espressif-esp-iot-solution/en/latest/hw-reference/ESP-Prog_guide.html)

[https://docs.espressif.com/projects/esp-idf/en/stable/esp32/api-guides/jtag-debugging/index.html](https://docs.espressif.com/projects/esp-idf/en/stable/esp32/api-guides/jtag-debugging/index.html)

### USB - Schnittstelle mit ZADIG umstellen:

#### vorher:

![](https://user-images.githubusercontent.com/69573151/203028255-a0b5e911-0242-4ecf-957d-ef70e81c8e86.png)

![](https://user-images.githubusercontent.com/69573151/203028864-2b13e1a3-9be6-4c23-bea2-b32463a38cdb.png)

#### Aufruf von ZADIG:

siehe auch: [https://docs.espressif.com/projects/esp-idf/en/v4.4.3/esp32/api-guides/jtag-debugging/configure-ft2232h-jtag.html#windows](https://docs.espressif.com/projects/esp-idf/en/v4.4.3/esp32/api-guides/jtag-debugging/configure-ft2232h-jtag.html#windows)

![Schritt_01](https://raw.githubusercontent.com/Meisterschulen-am-Ostbahnhof-Munchen/Install-ISOBUS-Environment-docs/main/images/JTAG/Schritt_01.png)

#### nachher:

![](https://user-images.githubusercontent.com/69573151/203028640-6106a050-2190-4467-86d0-e956cf905026.png)

Hinweis: der Vorgang muss leider wiederholt werden wenn man den ESP-PROG an eine andere Schnittstelle anschließt. 

daher idealerweise immer dieselben USB Steckplätze verwenden. 

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

https://docs.espressif.com/projects/esp-idf/en/v4.4.3/esp32/api-guides/jtag-debugging/index.html#run-openocd

openocd -f board/esp32-wrover-kit-3.3v.cfg

![](https://user-images.githubusercontent.com/69573151/203031746-93eec259-ef86-4e3e-95a5-7daafd7ebd21.png)

ACHTUNG !!! das starten des GDB Servers von der Kommandozeile ist nur noch erforderlich, wenn man auch an der Kommandozeile debuggt. 

\--> aus der ESP-IDF heraus wird openocd automatisch gestartet. 

## Schritt\_04:

an dieser Stelle ist die Doku hoffnungslos veraltet. 

wenn man die Espressif-IDE (Espressif-IDE) verwendet, dann stimmen diese Links nicht mehr.

https://docs.espressif.com/projects/esp-idf/en/latest/api-guides/jtag-debugging/debugging-examples.html#jtag-debugging-examples-eclipse

[https://docs.espressif.com/projects/esp-idf/en/latest/api-guides/jtag-debugging/using-debugger.html#jtag-debugging-using-debugger-eclipse](https://docs.espressif.com/projects/esp-idf/en/latest/api-guides/jtag-debugging/using-debugger.html#jtag-debugging-using-debugger-eclipse)

Ich habe wie folgt sofort eine Debugging zustande gebracht:

1.  nur ESP-IDF GDB... wählen, dann links oben auf das

![](https://user-images.githubusercontent.com/69573151/203037697-609963cb-6331-4772-95b8-35f5f93ed371.png)

Symbol klicken, 

und starten. 

keinerlei Einstellungen zu tätigen. 

![](https://user-images.githubusercontent.com/69573151/203036844-41313b50-3286-4cd1-bfde-dec157615413.png)

## Schritt\_05:

entfällt

## Schritt\_06:

entfällt

## Schritt\_07:

![](https://user-images.githubusercontent.com/69573151/203037819-ed99f4f7-3f08-4199-8075-e7261f328ff3.png)

und ja, man kann die Console parallel zur Debugging Session laufen lassen, 

aber die Console muss vor dem Start der Debugging Session offen sein.
