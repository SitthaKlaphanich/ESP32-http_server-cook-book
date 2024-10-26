# ESP32-http_server-cook-book

### 1.ESP-IDF Example

เลือก simple ที่หัวข้อ http_server หลังจากนั้นกด Create project

![image](https://github.com/user-attachments/assets/295365e7-e9fd-4191-aaa8-78ef85832e60)

### 2.กำหนดการตั้งค่า

ตั้งค่า ESP-IDF: SDK configuration editor (menuconfig) ให้เชื่อมกับ WiFi บ้านหรือตามที่เรากำหนด เพื่อเชื่อมต่อ ESP32

![image](https://github.com/user-attachments/assets/085a4292-cab8-48f4-a0f6-3f25517c9aa4)

### 3.แก้ไข code

ไปที่ Folder main และไปที่ File main.c แล้วเพิ่ม #include ดังนี้

![image](https://github.com/user-attachments/assets/7588c967-f25d-4225-a556-51f52db2ba7c)

### 4.กำหนดตัวแปร

ต่อมาประกาศตัวแปร ดังนี้

![image](https://github.com/user-attachments/assets/7e6c141a-6327-40e8-b4e1-535430dccd1e)

![image](https://github.com/user-attachments/assets/b5c88f43-addd-4986-94fc-7e9f758f9b87)

### 5.กำหนดการอ่านค่าและแสดงผล

เพิ่มการแสดงผลและอ่านค่า ดังนี้

![image](https://github.com/user-attachments/assets/330c490a-09bb-4497-98b7-38d8d69c5417)

### 6.เพิ่ม  analogtxt

เพิ่ม analogtxt ดังนี้

![image](https://github.com/user-attachments/assets/6b8746c8-1376-496f-a0ed-cb3c701d7608)

### 7.กำหนดการทำงาน

ตั้งค่า ADC ใน app_main(void) Code สามารถเอามาจาก ADC Example ESP-IDF ได้ และ Build โปรเจค

![image](https://github.com/user-attachments/assets/acc8de71-4edb-4708-bf11-fedf30f05796)

### 8.เข้า Browser ไปที่ URL ใส่ IP Address ของ ESP32 ตามด้วย /hello

เช่น 192.168.0.111/hello จะได้ดังนี้

![image](https://github.com/user-attachments/assets/ed683c16-222b-4614-8888-b78bfad0b0db)

จั๊มสาย ไป volume จากนั้นต่อเข้ากับ GPIO 36 จากนั้นลองปรับ จะได้ผลลัพธ์ดังนี้ (ค่าสามารถปรับเปลี่ยนได้)

![image](https://github.com/user-attachments/assets/69fb4a20-3204-4a29-8c26-386d054f46e2)

### 9.สรุป 
ESP32 สามารถใช้ HTTP Server เพื่ออ่านค่า ADC (Analog-to-Digital Converter) ได้ โดยการตั้งค่า ADC เพื่อให้สามารถอ่านค่า 
ได้


