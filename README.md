# USB-Digital-Audio-Cables-Testing (Draft 2021.09.25)

## ความรู้เบื้องต้นเกี่ยวกับ USB Digital Audio

- อ้างอิง Google [USB Digital Audio ](https://source.android.com/devices/audio/usb)
- Cambridge Audio [Our Guide to USB Audio - Why Should I Use it?](https://www.cambridgeaudio.com/usa/en/blog/our-guide-usb-audio-why-should-i-use-it/)
- EDN [Fundamentals of USB Audio](https://www.edn.com/fundamentals-of-usb-audio/)
- Intona [Cable](https://intona.eu/en/stories/cable)

## USB 1.0, 2.0, 3.0 ...

สามารถตรวจสอบความเร็วของ USB DAC ด้วยโปรแกรม [Thesycon USB Descriptor Dumper](https://www.thesycon.de/eng/usb_descriptordumper.shtml) บน Windows OS

จากการตรวจสอบ Shanling UA2 พบว่าใช้ USB 2.0 HighSpeed การเลือกใช้สาย USB 2.0 จึงเพียงพอต่อการใช้งาน การใช้สาย USB 3.0 จึงไม่ได้ทำให้รับ-ส่งข้อมูลเร็วขึ้นแต่อย่างใด

![Shanling UA2](/Pictures/DescriptorDump_Shanling_UA2.png)

## USB Audio Class (UAC)

## สาย USB มีผลต่อเสียงที่ได้หรือไม่ ?

### อุปกรณ์ที่ใช้ทดสอบ

- **Android Phone:** [Realme 5 Pro](https://www.realme.com/th/realme-5-pro) RMX1971EX
- **USB to S/PDIF Digital to Digital Converter:** [North Flat Japan FX-AUDIO- FX-D03J](http://www.nfjapan.com/新製品のご案内/usbバスパワー駆動ハイレゾ対応ddc-fx-audio-『fx-d03j』を発売/) UAC 1.0 24bit/96kHz
- **S/PDIF to USB Digital to Digital Converter:** [Hifime UR23 SPDIF Optical to USB Cconverter](https://hifimediy.com/product/hifime-ur23-spdif-optical-to-usb-converter/) UAC 1.0 24bit/96kHz
- **USB Cable Tester:** [BitTradeOne USB CABLE CHECKER 2](https://bit-trade-one.co.jp/adusbcim/)

### โปรแกรมที่ใช้ทดสอบ
- **Music Player:** [HiBy Music](https://play.google.com/store/apps/details?id=com.hiby.music)
- **Digital Audio Workstation:** [Bitwig Studio 8-Track](https://www.bitwig.com/8-track/)
- **Digital Audio Workstation:** [Audacity](https://www.audacityteam.org/)
- **Spectrogram Analysis:** [SoX - Sound eXchange](http://sox.sourceforge.net/)

### สาย USB ที่ใช้ทดสอบ
- [ddHifi TC05 1st Gen.](https://www.ddhifi.com/productinfo/469679.html) สายยาว 10 เซนติเมตร
- [FiiO LT-TC1](https://www.fiio.com/productinfo/354074.html) สายยาว 12 เซนติเมตร
- [OE Audio OTG Digital Cable](https://www.oeaudio.net/oeotg) สายยาว 12 เซนติเมตร
- [RØDE SC17](https://www.rode.com/accessories/cables/sc17) ได้รับมาตรฐาน [USB-IF Certified](https://www.usb.org/single-product/3751) สายยาว 150 เซนติเมตร

### วิธีการทดสอบ

Android ===> USB Cable ===> NFJ FX-AUDIO- FX-D03J ===> S/PDIF Cable ===> Hifime UR23 ===> PC

### ผลการทดสอบ
