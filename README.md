# USB-Digital-Audio-Cables-Testing (Draft 2021.10.13)

## ความรู้เบื้องต้นเกี่ยวกับ USB Digital Audio

- อ้างอิง Google [USB Digital Audio ](https://source.android.com/devices/audio/usb)
- Cambridge Audio [Our Guide to USB Audio - Why Should I Use it?](https://www.cambridgeaudio.com/usa/en/blog/our-guide-usb-audio-why-should-i-use-it/)
- EDN [Fundamentals of USB Audio](https://www.edn.com/fundamentals-of-usb-audio/)
- Intona [Cable](https://intona.eu/en/stories/cable)

## USB 1.0, 2.0, 3.0 ...

สามารถตรวจสอบความเร็วของ USB DAC ด้วยโปรแกรม [Thesycon USB Descriptor Dumper](https://www.thesycon.de/eng/usb_descriptordumper.shtml) บน Windows OS

จากการตรวจสอบ Shanling UA2 พบว่าใช้ USB 2.0 HighSpeed การเลือกใช้สาย USB 2.0 จึงเพียงพอต่อการใช้งาน การใช้สาย USB 3.0 จึงไม่ได้ทำให้รับ-ส่งข้อมูลเร็วขึ้นแต่อย่างใด

![Shanling UA2](/pictures/DescriptorDump_Shanling_UA2.png)

## USB Audio Class (UAC)

## สาย USB มีผลต่อเสียงที่ได้หรือไม่ ?

### อุปกรณ์ที่ใช้ทดสอบ

- **USB to S/PDIF Digital to Digital Converter:** [SIGNSTEK Q5 USB DDC/DAC](https://www.amazon.co.jp/-/en/dp/B00X9TY8ZW/) UAC X.0 24bit/96kHz, ชิป [TI/Burr-Brown PCM2407](https://www.ti.com/product/PCM2704)
- **S/PDIF to USB Digital to Digital Converter:** [Hifime UR23 SPDIF Optical to USB Cconverter](https://hifimediy.com/product/hifime-ur23-spdif-optical-to-usb-converter/) UAC 1.0 24bit/96kHz, ชิป [Savitech SA9023](https://www.savitech.co/usb-products)
- **S/PDIF to USB Digital to Digital Converter:** [CSL Externe 7.1 USB Soundkarte](https://www.amazon.de/-/en/dp/B00KXAVBQY/) clone, ชิป [Cmedia CM6206](https://www.cmedia.com.tw/products/USB20_FULL_SPEED/CM6206), ติดตั้งไดรเวอร์ของ [StarTech 7.1 USB Audio](https://www.startech.com/en-us/cards-adapters/icusbaudio7d#driver-and-downloads)
- **USB Cable Tester:** [BitTradeOne USB CABLE CHECKER 2](https://bit-trade-one.co.jp/adusbcim/)
- **USB C Female to A Male Adapter:** [Mcdodo OT-697](https://www.mcdodolife.com/products/ot-697-full-compatibility-type-c-5a-to-usb-a-2.0-c.html)
- **USB C Female to B Male Adapter:** UGREEN 20120
- **TOSLINK Cable:** [UGREEN 70890](https://www.ugreen.com/products/fiber-optical-audio-cable) สายยาว 100 เซนติเมตร

### โปรแกรมที่ใช้ทดสอบ
- [FFmpeg v4.4](https://www.ffmpeg.org/)
- [fmedia v1.24](https://stsaz.github.io/fmedia/)
- [Pratt v6.1.53](https://www.fon.hum.uva.nl/praat/)
- [SoX v14.4.2](http://sox.sourceforge.net/)

### สาย USB ที่ใช้ทดสอบ
- [AENZR FPC AZ1301, USB C Male to C Male, USB 3.1 Gen 2](http://www.aenzr.com/pd.jsp?id=31) สายยาว 13 เซนติเมตร
- [ANKER PowerLine II A8485, USB C Male to C Male, USB 3.1 Gen 2](https://www.anker.com/es/products/A8485011) ได้รับมาตรฐาน [USB-IF Certified](https://www.usb.org/single-product/3563) สายยาว 90 เซนติเมตร
- [ddHifi TC05 1st Gen. USB C Male to C Male, USB 2.0](https://www.ddhifi.com/productinfo/469679.html) สายยาว 10 เซนติเมตร
- [FiiO LT-TC1, USB C Male to C Male USB 2.0](https://www.fiio.com/productinfo/354074.html) สายยาว 12 เซนติเมตร
- [NEO (created by OYAIDE Elec.) d+ USB class B, USB A Male to B Male , USB 2.0](https://www.neo-w.com/english/d_plus/d_plus_usb_ser/) สายยาว 100 เซนติเมตร
- [OE Audio OTG Digital Cable, USB C Male to C Male, USB 2.0](https://www.oeaudio.net/oeotg) สายยาว 12 เซนติเมตร
- [RØDE SC17, USB C Male to C Male, USB 2.0](https://www.rode.com/accessories/cables/sc17) ได้รับมาตรฐาน [USB-IF Certified](https://www.usb.org/single-product/3751) สายยาว 150 เซนติเมตร
- [Shanling UA2, USB C Male to C Male, USB 2.0 สายแถม](https://en.shanling.com/product/396) สายยาว 12=0 เซนติเมตร
- [UGREEN 10350, USB A Male to B Male USB 2.0](https://www.ugreen.com/products/usb-2-0-printer-scanner-cable) สายยาว 150 เซนติเมตร
- [UGREEN 50996, USB C Male to C Male, USB 2.0](https://www.ugreen.com.ph/products/usb-c-to-usb-c-cable?variant=16295877935153) สายยาว 50 เซนติเมตร

### เพลงที่ใช้ทดสอบ
- [Sennheiser 'Sound Check' by Tim Cowie](https://en-us.sennheiser.com/hearthedifference)

### วิธีการทดสอบ

PC ==> USB Cable ==> SIGNSTEK Q5 USB DDC/DAC ==> TOSLINK Cable ==> USB 7.1 Sound Card ==> USB Cable ==> PC

![Test Rig 1](/pictures/IMG20211013144032.jpg)

![Test Rig 2](/pictures/IMG20211013144532.jpg)

### ผลการทดสอบ
