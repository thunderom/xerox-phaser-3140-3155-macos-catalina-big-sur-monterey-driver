# Xerox-Phaser-3140-3155-macOS-Catalina-Big-Sur-Monterey-Sonoma-driver

Xerox Phaser 3140/3155 macOS Catalina (version 10.15), Big Sur (version 11), Monterey (version 12), Sonoma (14.4.1) driver

I tried to do it bymyself based on the [Gist](https://gist.github.com/santiago26/60425d2759b1360555111caa47b6769f), but it didn't work with the driver over there so I installed the driver on an old Macintosh machine running macOS Mojave (version 10.14.6) and copied the files from there.

The files can be found here: [link](driver/Xerox_Phaser_3140_3155_macOS_Catalina_Big_Sur_Monterey_driver.zip) /* There's a Download button on the right side... */

And it worked.

## Installation

Copy all of the files and directories to the right place on your machine manually:

```
copy Library/Printers/Xerox/Phaser_3140_3155/* to /Library/Printers/Xerox/Phaser_3140_3155
copy Library/Printers/PPDs/Contents/Resources/Xerox Phaser 3140 and 3155.gz to /Library/Printers/PPDs/Contents/Resources/Xerox Phaser 3140 and 3155.gz
copy private/etc/cups/ppd/Xerox_Phaser_3140_and_3155.ppd to /private/etc/cups/ppd/Xerox_Phaser_3140_and_3155.ppd
```

and install the printer as usual:

![](pics/install_1.png "")
![](pics/install_2.png "")
![](pics/install_3.png "")
![](pics/install_4.png "")
![](pics/install_5.png "")

Test print:

![](pics/install_6.png "")

[Tada.wav](https://www.youtube.com/watch?v=QDUv_8Dw-Mw&ab_channel=ProductDesignsYT)

Драйвер Apple Silicon для Xerox Phaser 3140, 3155 (Catalina, Big Sur, Monterey, Sonoma)
Для тех из вас, кто всё ещё ищет драйвер для Xerox Phaser 3140, 3155, совместимый с Apple Silicon (M1, M2, M3 на данный момент) и последними версиями macOS (до Sonoma 14.5 на данный момент), этот драйвер, по-видимому, извлечённый из более старого пакета драйверов Xerox для macOS, разработанного Дьёрдем Флейшманом, подошёл мне:

https://github.com/FleXoft/Xerox-Phaser-3140-3155-macOS-Catalina-Big-Sur-Monterey-driver

В дополнение к инструкциям, приведённым в README.md в связанном репозитории, мне нужно было пометить как безопасный следующий исполняемый файл:
/Library/Printers/Xerox/Phaser_3140_3155/rastertoxrx

Для этого я перешёл по ссылке
/Library/Printers/Xerox/Phaser_3140_3155/
щелкнул правой кнопкой мыши на rastertoxrx и выбрал Открыть -> Открыть и т.д. чтобы подтвердить, что я доверяю этому исполняемому файлу.

Вот отчёт VirusTotal об архиве репозитория на момент публикации:
https://www.virustotal.com/gui/file/cae2f6948b3c33a38e8d9fc0064762cd61a901adcd03885b602e26fcebcd5d50

Мы рекомендуем вам в любом случае проверять на вирусы все загружаемые файлы!

Используйте на свой страх и риск. Спасибо :)
