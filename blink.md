# Getting to Blink

![Cover Image](https://mewing-nebula-d50.notion.site/images/page-cover/met_canaletto_1720.jpg)

## 💡 Introduction

เมื่อคุณดูที่บอร์ดไมโครคอนโทรลเลอร์ จะพบว่าไม่มีวิธีง่าย ๆ ในการแสดงผลบนหน้าจอ ดังนั้นโปรแกรมแรกที่นิยมใช้คือการ **กระพริบ LED** เพื่อทดสอบว่า:

- ✅ Compile code ได้ถูกต้อง
- ✅ รันบนไมโครคอนโทรลเลอร์ได้
- ✅ ควบคุมขา (pins) ได้จริง

## 🔍 Arduino Board

- บอร์ด Arduino ส่วนใหญ่มี LED ติดตั้งอยู่บน **PIN 13**
- การทำให้ LED กระพริบเป็นขั้นตอนสำคัญในการตรวจสอบว่าอุปกรณ์ทำงานได้

## 🛠️ 1. Arduino IDE

เปิดโปรแกรม Arduino แล้ว:

- Paste โค้ด
- กด **Verify** เพื่อ compile
- กด **Upload** เพื่ออัปโหลดไปยังบอร์ด

### 📘 Arduino Programming Language

#### Functions

- [`pinMode()`](https://www.arduino.cc/reference/en/language/functions/digital-io/pinmode/)
- [`digitalRead()`](https://www.arduino.cc/reference/en/language/functions/digital-io/digitalread/)
- [`delay()`](https://www.arduino.cc/reference/en/language/functions/time/delay/)

#### Variables

- [`INPUT`, `INPUT_PULLUP`, `OUTPUT`](https://www.arduino.cc/reference/en/language/variables/constants/inputoutputpullup/)
- [`HIGH`, `LOW`](https://www.arduino.cc/reference/en/language/variables/constants/highlow/)

## 🔧 2. Schematic and Circuit Simulator

ลองใช้ [Tinkercad Circuit Design Blink](https://www.tinkercad.com/things/0LWlH4WEsVC-blink?sharecode=S3q8Pjr8kyig00HoM01p_wVuP3_XJTq3WRuQ_QlWQW4)

```cpp
digitalWrite(LED_BUILTIN, HIGH);
delay(1000);
digitalWrite(LED_BUILTIN, LOW);
delay(1000);
