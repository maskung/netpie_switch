# netpie_switch

โปเจคนี้เป็นโปรเจคปิดเปิดไฟด้วยผ่าน netpie 

## รายละเอียดระบบ

โปรเจคจะมี loop รับคำสั่งจาก netpie
OUTPUT Relay มี 4 ช่อง ดูได้จากบันทัด #define LIGHT1 - LIGHT4
ชื่ออุปกรณ์ที่ใช้สั่งงานผ่าน netpie คือ SmartHomeSST 

### การตั้งค่าต่างๆ และสิ่งที่ต้องใข้

ไลบรารีที่ต้องใช้
1.netpie microgear

พารามิเตอร์ต่างๆ ในการกำหนดให้ระบบทำงานอยู่ทางตอนต้นของโค้ด

```
#define APPID   "xxxxxxx"   //หมายเลข appid ของท่านที่สร้างใน netpie
#define KEY     "xxxxxxx"   //key ที่สร้างขึ้น ใน APPID
#define SECRET  "xxxxxxx"   //secrate ที่ได้จากการสร้าง key

#define ALIAS   "SmartSwitches"           // ชื่ออุปกรณ์ของท่านที่จะให้ปรากฏใน netpie

// --------------------------------------------------------------------------------------

//ขา รีเลย์ ต่างที่ต่อ ในที่นี้ใช้การอ้างอิงด้วย nodemcu เป็นหลัก
#define LIGHT1 D7 
#define LIGHT2 D5
#define LIGHT3 D3
#define LIGHT4 D6
```
### การติดตั้ง

ดาวน์โหลดโค้ดแล้วคอมพายล์ด้วย Ardunio IDE

## สร้างด้วย

* [Ardunio 1.8.3](https://www.arduino.cc/en/main/software) - ดาวน์โหลดเวอร์ชั่นล่าสุดได้ที่นี่
* [Microgear Lirary](https://github.com/netpieio/microgear-esp8266-arduino) - ไลบรารีสำหรับการเชื่อมต่อ netpie 

## ผู้เขียน

* **Suphanut Thanyaboon** - *ผู้ริเริ่ม* - [maskung](https://github.com/maskung)

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details
