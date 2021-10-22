# USB-Digital-Audio-Cables-Testing (Draft 2021.10.22)

1. [ความรู้เบื้องต้นเกี่ยวกับ USB Digital Audio](#ความรู้เบื้องต้นเกี่ยวกับ-usb-digital-audio)
2. [สรุปผลการทดสอบ](#สรุปผลการทดสอบ)

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

- **USB to S/PDIF Digital to Digital Converter:** [SIGNSTEK Q5 USB DDC/DAC](https://www.amazon.co.jp/-/en/dp/B00X9TY8ZW/) UAC 1.0 16bit/48kHz, ชิป [Burr-Brown PCM2407](https://www.ti.com/product/PCM2704)
- **S/PDIF to USB Digital to Digital Converter:** [Hifime UR23 SPDIF Optical to USB Converter](https://hifimediy.com/product/hifime-ur23-spdif-optical-to-usb-converter/) UAC 1.0 24bit/96kHz, ชิป [Savitech SA9023](https://www.savitech.co/usb-products)
- **USB Cable Tester:** [BitTradeOne USB CABLE CHECKER 2](https://bit-trade-one.co.jp/adusbcim/)
- **USB C Female to A Male Adapter:** [Mcdodo OT-697](https://www.mcdodolife.com/products/ot-697-full-compatibility-type-c-5a-to-usb-a-2.0-c.html)
- **USB C Female to B Male Adapter:** [UGREEN 20120](https://ugreenvietnam.com/ugreen-20120-usb-2-0-duc-may-in-ra-dau-cai-type-c-vo-nhom-mau-xam-us382-20020120.html)
- **TOSLINK Cable:** [UGREEN 70890](https://www.ugreen.com/products/fiber-optical-audio-cable) สายยาว 100 เซนติเมตร

### สาย USB ที่ใช้ทดสอบ

แบ่งกลุ่มสาย USB ออกเป็น 3 กลุ่ม กลุ่มละ 5 เส้น รวมเป็นสาย USB ทั้งหมด 15 เส้น ได้แก่
- กลุ่มสาย USB C แบบสั้น ความยาวน้อยกว่าหรือเท่ากับ 20 เซนติเมตร
- กลุ่มสาย USB C ทั่วไป ความยาวมากกว่า 20 เซนติเมตร
- กลุ่มสาย USB B ทุกความยาว

####  กลุ่มสาย USB C แบบสั้น ความยาวน้อยกว่าหรือเท่ากับ 20 เซนติเมตร

|ยี่ห้อ<img width=80/>|รุ่น<img width=120/>|ประภทหัวต่อ|ความเร็วสาย<img width=30/>|ความยาวสาย (ซม.)|USB-IF Certified|
|-|-|-|-|-|-|
|Shanling|[สายแถมจาก UA2](https://en.shanling.com/product/396)|C to C|USB 2.0|10|-|
|ddHifi|[TC05 1st Gen.](https://www.ddhifi.com/productinfo/469679.html)|C to C|USB 2.0|10|-|
|FiiO|[LT-TC1](https://www.fiio.com/productinfo/354074.html)|C to C|USB 2.0|12|-|
|OE Audio|[OTG Digital Cable](https://www.oeaudio.net/oeotg)|C to C|USB 2.0|12|-|
|AENZR|[FPC AZ1301](http://www.aenzr.com/pd.jsp?id=31)|C to C|USB 3.1 Gen 2|13|-|

#### กลุ่มสาย USB C ทั่วไป ความยาวมากกว่า 20 เซนติเมตร

|ยี่ห้อ<img width=80/>|รุ่น<img width=120/>|ประภทหัวต่อ|ความเร็วสาย<img width=30/>|ความยาวสาย (ซม.)|USB-IF Certified|
|-|-|-|-|-|-|
|UGREEN|[50996](https://www.ugreen.com.ph/products/usb-c-to-usb-c-cable?variant=16295877935153)|C to C|USB 2.0|50|-|
|ANKER|[PowerLine II A8485](https://www.anker.com/es/products/A8485011)|C to C|USB 3.1 Gen 2|90|[✔](https://www.usb.org/single-product/3563)|
|Verbatim|[65684](https://www.verbatim.com.hk/accessories/mobile-accessories/sync-charge-cables/usb3-2-c-to-c-cable.html)|C to C|USB 3.2|100|-|
|RØDE|[SC17](https://www.rode.com/accessories/cables/sc17)|C to C|USB 2.0|150|[✔](https://www.usb.org/single-product/3751)|
|KUULAA|[KL-X31](http://www.kuulaa.cn/plus/view.php?aid=45)|C to C|USB 2.0|300|-|

#### กลุ่มสาย USB B ทุกความยาว

|ยี่ห้อ<img width=80/>|รุ่น<img width=120/>|ประภทหัวต่อ|ความเร็วสาย<img width=30/>|ความยาวสาย (ซม.)|USB-IF Certified|
|-|-|-|-|-|-|
|NO BRAND|BLUE|A to B|USB 2.0|18|-|
|Audioquest|[Forest](https://www.audioquest.com/cables/digital-cables/usb-a-to-usb-b/forest)|A to B|USB 2.0|75|-|
|NEO by OYAIDE|[d+ USB class B](https://www.neo-w.com/english/d_plus/d_plus_usb_ser/)|A to B|USB 2.0|100|-|
|UGREEN|[80805](https://www.ugreen.com/products/usb-c-to-usb-b-2-0-printer-cable)|C to B|USB 2.0|100|-|
|UGREEN|[10350](https://www.ugreen.com/products/usb-2-0-printer-scanner-cable)|A to B|USB 2.0|150|-|


### โปรแกรมที่ใช้ทดสอบ
- [FFmpeg v4.4](https://www.ffmpeg.org/)
- [fmedia v1.24](https://stsaz.github.io/fmedia/)
- [Pratt v6.1.53](https://www.fon.hum.uva.nl/praat/)
- [SoX v14.4.2](http://sox.sourceforge.net/)
- [DeltaWave v2.0.1](https://deltaw.org/)

### เพลงที่ใช้ทดสอบ
- [Sennheiser 'Sound Check' by Tim Cowie](https://en-us.sennheiser.com/hearthedifference) โดยใช้ไฟล์จาก https://assets.sennheiser.com/global-downloads/file/13888/Sennheiser__Sound_Check__by_Tim_Cowie.wav

### วิธีการทดสอบ

Notebook ==> **USB Cable** ==> SIGNSTEK Q5 ==> UGREEN TOSLINK Cable ==> Hifime UR23 ==> Notebook

![Test Rig 1](pictures/IMG20211016153917_1600.jpg)

### การเตรียมสภาพแวดล้อมเพื่อการทดลอง (Test Environment Setup)

- เครื่อง Notebook ใช้ไฟจากแบตเตอรี่ ไม่เสียบสายไฟ เพื่อป้องกันปัญหา ground loop
- เปิด Airplane mode เพื่อป้องกันไม่ให้ Windows Update ทำงานเบื้องหลังซึ่งอาจกระทบการอ่าน-เขียนไฟล์ได้
- ปิดเสียงของ Windows โดยปรับให้เสียงอยู่ที่ 0 เนื่องจากโดยปกติสัญญาณเสียงที่ออกมาจาก USB DDC ทางช่อง Optical Out จะไม่ขึ้นอยู้กับระดับเสียงของ Windows แต่กับ USB DDC บางตัวเมื่อปรับเสียงให้ดังขึ้น ตัวเครื่องเองก็ปรับระดับสัญญาณของ Optical Out ให้สูงขึ้นด้วย ทำให้เสียงที่ได้ไม่เหมือนกับต้นฉบับและอาจเกิดการ clip ของเสียงได้
- ปรับ bit depth และ sample rate ให้ตรงกันทั้งระบบ ตั้งแต่ไฟล์ต้นฉบับ, USB DDC และ S/PDIF to USB หากไฟล์ต้นฉบับที่ใช้ในการทดสอบมี  bit depth หรือ sample rate ที่สูงกว่าระบบที่ใช้ทดสอบ ให้ทำการแปลงไฟล์ก่อนทำการทดสอบ
- เพิ่มเสียงว่าง (silence pad) เข้าไปที่ไฟล์ต้นฉบับ ทางด้านหัวและท้ายด้านละ 2 วินาที เนื่องจากเมื่อกดเล่นเพลงเสียงในช่วงเริ่มต้นอาจจะกระตุกจากการที่โปรแกรมเล่นเพลงกำลังทำการ buffer ไฟล์ ซึ่งจะทำให้ผลการทดลองคลาดเคลื่อน

#### การปรับตั้งค่าในส่วน Playback (USB to S/PDIF)

1. Double click ที่ SIGNSTEK Q5

    ![Playback_01](pictures/Playback_01.png)

2. ปรับเสียง Speakers ให้อยู่ที่ 0

    ![Playback_02](pictures/Playback_02.png)

3. ปิด Enhancements ทั้งหมด

    ![Playback_03](pictures/Playback_03.png)

4. ปรับ Default Format ให้อยู่ที่ 16 bit, 48000 Hz สูงสุดที่ SIGNSTEK Q5 รองรับ

    ![Playback_04](pictures/Playback_04.png)

5. ปิด Spartial sound

    ![Playback_05](pictures/Playback_05.png)

#### การปรับตั้งค่าในส่วนของ Recording (S/PDIF to USB)

1. Double click ที่ Hifime UR23

    ![Recording_01](pictures/Recording_01.png)

2. ปรับเสียง SPDIF interface ให้อยู่ที่ 100

    ![Recording_02](pictures/Recording_02.png)

3. ปรับ Default Format ให้อยู่ที่ 2 channel, 16 bit, 48000 Hz สูงสุดที่ SIGNSTEK Q5 รองรับ

    ![Recording_03](pictures/Recording_03.png)

#### การตรวจสอบ bit depth และ sample rate ไฟล์ต้นฉบับ

sox --info Sennheiser__Sound_Check__by_Tim_Cowie.wav

![sox_info](pictures/sox_info.png)

#### การแปลง bit depth และ sample rate ไฟล์ต้นฉบับ

sox Sennheiser__Sound_Check__by_Tim_Cowie.wav -b 16 -r 48000 -c 2 master_16_48_pad.wav pad 2 2

![sox_convert_pad](pictures/sox_convert_pad.png)

### Proof of Concept

ทดลองปรับ equalizer โดยลองปรับความถี่่ 100 Hz ขึ้นไป 1 dB

ffmpeg -hide_banner -y -i master_16_48_pad.wav -af "equalizer=frequency=100:width_type=h:width=1:gain=1" master_16_48_pad_eq_100.wav

![ffmpeg_eq_100](pictures/ffmpeg_eq_100.png)

จากนั้นลองกลับเฟสเทียบกับไฟล์ต้นฉบับ

sox -m -v 1 master_16_48_pad.wav -v -1 master_16_48_pad_eq_100.wav master_16_48_pad_eq_100_inverted.wav

![sox_phase_invert_100](pictures/sox_phase_invert_100.png)

เมื่อตรวจสอบไฟล์ที่กลับเฟสด้วยภาพ spectrogram จะพบว่าไฟล์ไม่ได้เงียบสนิท

sox master_16_48_pad_eq_100_inverted.wav -n spectrogram -t master_16_48_pad_eq_100_inverted.wav -o master_16_48_pad_eq_100_inverted.png

![master_16_48_pad_eq_100_inverted](pictures/master_16_48_pad_eq_100_inverted.png)

### ผลการทดสอบ

|ไฟล์เสียงที่ปรับ offset แล้ว|เปรียบเทียบ Bit Perfect กับต้นฉบับ|Spectrogram กลับเฟส|
|-|-|-|
|[AENZR FPC AZ1301](recorded_trim/AENZR_AZ1301_C-C_USB31_13cm.wav)|[100%](result_deltawave/AENZR_AZ1301_C-C_USB31_13cm.txt)|[Spectrogram](visual_spectrogram/AENZR_AZ1301_C-C_USB31_13cm_inverted.png)|
|[ANKER PowerLine II A8485](recorded_trim/ANKER_A8485_C-C_USB31_90cm.wav)|[100%](result_deltawave/ANKER_A8485_C-C_USB31_90cm.txt)|[Spectrogram](visual_spectrogram/ANKER_A8485_C-C_USB31_90cm_inverted.png)|
|[Audioquest Forest](recorded_trim/Audioquest_Forest_A-B_75cm.wav)|[100%](result_deltawave/Audioquest_Forest_A-B_75cm.txt)|[Spectrogram](visual_spectrogram/Audioquest_Forest_A-B_75cm_inverted.png)|
|[ddHifi TC05 1st Gen.](recorded_trim/ddHifi_TC05_C-C_USB20_15cm.wav)|[100%](result_deltawave/ddHifi_TC05_C-C_USB20_15cm.txt)|[Spectrogram](visual_spectrogram/ddHifi_TC05_C-C_USB20_15cm_inverted.png)|
|[FiiO LT-TC1](recorded_trim/FiiO_LT-TC01_C-C_USB20_15cm.wav)|[100%](result_deltawave/FiiO_LT-TC01_C-C_USB20_15cm.txt)|[Spectrogram](visual_spectrogram/FiiO_LT-TC01_C-C_USB20_15cm_inverted.png)|
|[NEO (created by OYAIDE Elec.) d+ USB class B](recorded_trim/NEO_d%2B_A-B_USB20_100cm.wav)|[100%](result_deltawave/NEO_d%2B_A-B_USB20_100cm.txt)|[Spectrogram](visual_spectrogram/NEO_d%2B_A-B_USB20_100cm_inverted.png)|
|[OE Audio OTG Digital Cable](recorded_trim/OEAudio_OTG_C-C_USB20_12cm.wav)|[100%](result_deltawave/OEAudio_OTG_C-C_USB20_12cm.txt)|[Spectrogram](visual_spectrogram/OEAudio_OTG_C-C_USB20_12cm_inverted.png)|
|[RØDE SC17](recorded_trim/RODE_SC17_C-C_USB20_100cm.wav)|[100%](result_deltawave/RODE_SC17_C-C_USB20_100cm.txt)|[Spectrogram](visual_spectrogram/RODE_SC17_C-C_USB20_100cm_inverted.png)|
|[Shanling UA2 สายแถม](recorded_trim/Shanling_UA2_C-C_USB2.0_10cm.wav)|[100%](result_deltawave/Shanling_UA2_C-C_USB2.0_10cm.txt)|[Spectrogram](visual_spectrogram/Shanling_UA2_C-C_USB2.0_10cm_inverted.png)|
|[UGREEN 10350](recorded_trim/UGREEN_10350_A-B_USB20_150cm.wav)|[100%](result_deltawave/UGREEN_10350_A-B_USB20_150cm.txt)|[Spectrogram](visual_spectrogram/UGREEN_10350_A-B_USB20_150cm_inverted.png)|
|[UGREEN 50996](recorded_trim/UGREEN_50996_C-C_USB20_50cm.wav)|[100%](result_deltawave/UGREEN_50996_C-C_USB20_50cm.txt)|[Spectrogram](visual_spectrogram/UGREEN_50996_C-C_USB20_50cm_inverted.png)|

### สรุปผลการทดสอบ

สาย USB ทุกเส้นให้เสียงที่เหมือนกับต้นฉบับ 100% ไม่ว่าจะเปลี่ยนไปใช้สายเส้นไหนก็ตาม แสดงว่าสาย USB ไม่มีผลต่อเสียงที่ได้แต่อย่างใด
