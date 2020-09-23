# Odoo Barcode

Hilfreiche Einführung: https://www.youtube.com/watch?v=OTfss3WF0jI

Odoo generiert Barcodes nach *1D Industrial Codes*

## Integration

**USB oder Bluetooth**

Jeder Barcode-Scanner, der über USB oder Bluetooth an einem Computer angeschlossen werden kann, ist kompatibel.  
Im Normall wird beim Scannen eines Barcodes der Code eingefügt. Wenn auf dem Computer die Odoo Barcode-App im Browser aktiv ist, wird der eingefügt Code erfasst.
Der Barcode-Scanner setzt den gescannten Code um und schreibt diesen ins ausgewählte Feld. Eigentlich derselbe Vorgang wie bei einer herkömmlichen USB-Tastatur.

**Ventor App**

Die App und geräte von Ventor sehen interessant aus.

Website: https://ventor.app/
Anleitung: https://ventor.tech/warehouse-management/how-to-connect-a-barcode-scanner-with-odoo/

Hierbei verbindet sich die Ventor App direkt mit der Odoo-Installation

**Barcode to PC**

Es gibt Lösungen um einen Scan vom Smartphone an den Computer zu senden.

Website https://barcodetopc.com/

Auf dem Computer startet man ein Program zum Empfang der Barcodes vom Smartphone. Auf dem Smartphone startet man die Barcode-App und verbindet sich mit dem Computer-Program über Wifi. Dann öffnet man auf dem Computer Odoo im Browser, wählt die Barcode-App und starte einen Vorgang. Wenn man mit dem Smartphone einen Barcode scannt, wird dieser über via Wifi übertragen, vom Program entfangen und in Odoo eingefügt.

## Drucken von BarCodes
Barcodes können von fast allen Programmen aus gedruckt werden. Dies, weil meistens ein Font für den Druck verwendet wird.
Der als Barcode angedruckte Wert wird zuerst als Klarwert eingetragen und anschliessend mit dem Font (z.B. 3of9.ttf) angezeigt.
Beim Betriebssystem Windows kann die Prüfziffer einige Probleme bereiten. Ein Sicherheitsupdate von Windows aus dem Jahr 2012 blockt den GDI-Trieber und lässt die Berechnung der Prüfziffer nicht zu sodass dieser Barcode nicht lesbar ist. Tritt bei 1000 Code in etwa 18 mal auf. 

## Mobile Apps

**iOS**

* [Scandit Keyboard Wedge](https://apps.apple.com/us/app/scandit-keyboard-wedge/id1275099694)
* [Barcode to PC: Wi-Fi scanner](https://apps.apple.com/us/app/barcode-to-pc-wi-fi-scanner/id1180168368)

## Hardware

**Scaner**

Die Scanner der DATALOGIC (z.B. QuickScan Barcode Scanner QD2430 Black) wurden zu dutzenden an mehreren hunderten von Generalversammlungen eingesetzt und haben sich bewährt. Sie sind günstig (unter CHF 200), einfach in der Handhabung und robust. Die Scanner müssen für den ersten Einsatz nicht konfiguriert werden. 

## Barcode-Arten

** Code39**
Der Barcode 39 hat keine Prüfziffer und kann in fast allen Fällen immer gelesen werden. Nachteil ist die Grösse, resp. Breite bei grösseren Werten.

**Code 128**
Der BarCode 128 verwendet eine Prüfziffer und gilt als Sicher. Auch stellt der BarCode 128 grössere Werte in einer vernüftigen Breite dar. Je nach Font kann der BarCode 128 als HR angedruckt werden. Das heisst, unter dem Barcode wird der Wert noch lesebar angedruckt.
