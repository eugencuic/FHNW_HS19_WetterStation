## <span style="color:green">**Wetterstation - Anleitung für Aufbau und Inbetriebnahme**

## Hardware
### *Hardwarevoraussetzungen:*

- Waveshare Display 10.1 inch HDM LCDD (B) (with case)
- Raspberry Pi 4 Computer
- SD Karte für OS und Daten (16GB)

### *Zusammenbau Hardware*

Um den Monitor und den Raspberry Pi zusammenzubauen nutzten Sie bitte folgenden Link und folgen Sie der Bildanleitung:

***[Bauanleitung](https://www.waveshare.com/w/upload/4/4a/10.1inch-HDMI-LCD-B-with-Holder-assemble.jpg)***

## Software

### *Softwarevoraussetzungen:*

 Library  | Version | Link
:---------|:---------:| ------
fhnw-ds-hs2019-weatherstation-api 0.21 | v 0.19 | [GitHub](https://github.com/markif/WeatherStation_HS2019)

### Installation:

Nachdem ersten Anschliessen an die Stromquelle Terminal starten und Raspberry auf den neusten Stand bringen












Laden der Daten ist mit crontab erstellt. script lädt automatisch am start

bildschirm sleep mode:
Open your lightdm configuration:

sudo nano /etc/lightdm/lightdm.conf
Anywhere below the [SeatDefaults] header, add:

xserver-command=X -s 0 -dpms
This will set your blanking timeout to 0 and turn off your display power management signaling.

