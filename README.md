# USB-Digital-Audio-Cables-Testing (Draft 2021.09.18)

## ความรู้เบื้องต้นเกี่ยวกับ USB Digital Audio

- อ้างอิง Google [USB Digital Audio ](https://source.android.com/devices/audio/usb)
- Cambridge Audio [Our Guide to USB Audio - Why Should I Use it?](https://www.cambridgeaudio.com/usa/en/blog/our-guide-usb-audio-why-should-i-use-it/)

## USB Audio Class (UAC)

## USB 1.0, 2.0, 3.0 ...

สามารถตรวจสอบความเร็วของ USB DAC ด้วยโปรแกรม [Thesycon USB Descriptor Dumper](https://www.thesycon.de/eng/usb_descriptordumper.shtml) บน Windows OS

จากการตรวจสอบ Shanling UA2 พบว่าใช้ USB 2.0 HighSpeed การเลือกใช้สาย USB 2.0 จึงเพียงพอต่อการใช้งาน การใช้สาย USB 3.0 จึงไม่ได้ทำให้รับ-ส่งข้อมูลเร็วขึ้นแต่อย่างใด

![Shanling UA2](/Pictures/DescriptorDump_Shanling_UA2.png)

## สาย USB มีผลต่อเสียงที่ได้หรือไม่ ?

### อุปกรณ์ที่ใช้ทดสอบ

- **Android Phone:** [Realme 5 Pro](https://www.realme.com/th/realme-5-pro) RMX1971EX
- **USB DAC:** [Shanling UA2](https://en.shanling.com/product/396) USB 2.0, UAC 1.0/2.0
- **Audio Interface:** [ESI audio U22 XT ](https://www.esi-audio.com/products/u22xt/)
- **สายสัญญาณ:** สาย 3.5mm to RCA ใช้สาย [Canare L-2B2AT](https://www.canare.co.jp/en/products/cables/index.php?tid=4_003) ความยาว 1 เมตร เข้าหัว [Amphenol RCA](https://www.amphenol.com/node/4900)

### โปรแกรมที่ใช้ทดสอบ
- **Music Player:** [HiBy Music](https://play.google.com/store/apps/details?id=com.hiby.music)
- **Digital Audio Workstation:** [Bitwig Studio 8-Track](https://www.bitwig.com/8-track/)
- **Spectrogram Analysis:** [SoX - Sound eXchange](http://sox.sourceforge.net/)
- **Acoustics Fingerprint:** [Chromaprint](https://acoustid.org/chromaprint)

### สาย USB ที่ใช้ทดสอบ
- [ddHifi TC05 1st Gen.](https://www.ddhifi.com/productinfo/469679.html) สายยาว 10 เซนติเมตร
- [FiiO LT-TC1](https://www.fiio.com/productinfo/354074.html) สายยาว 12 เซนติเมตร
- [OE Audio OTG Digital Cable](https://www.oeaudio.net/oeotg) สายยาว 12 เซนติเมตร
- [RØDE SC17](https://www.rode.com/accessories/cables/sc17) ได้รับมาตรฐาน [USB-IF Certified](https://www.usb.org/single-product/3751) สายยาว 150 เซนติเมตร

### วิธีการทดสอบ

### ผลการทดสอบ
