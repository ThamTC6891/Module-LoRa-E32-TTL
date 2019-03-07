# Module-LoRa-E32-TTL
# Phần này mình sẽ trình bày cách thức setting các tham số cho module LoRa UART
# Trước tiên các bạn hãy chuẩn bị
* 1/ User Manual cho module dạng TTL, các bạn có thể xem tại đây http://www.inhaos.com/uploadfile/otherpic/DS-RF-TTL-100-V01-EN.pdf 
* 2/ Cách nối dây giữa LoRa với MCU như bên dưới (ở đây lấy ví dụ là Arduino) 

| Module LoRa | Arduino |
|--------------|-------|
| M0 | Pin 3 |
| M1 | Pin 3 |
| TXD | RXD |
| RXD | TXD |
| AUX | NC |
| VCC | 5V |
| GND | GND |

# Tiếp theo chúng ta sẽ tìm hiểu về khung truyền dữ liệu của module lora

Để thiết lập các thông số cho module thì khung truyền bao gồm 6 tham số như sau:

| Byte 0 | Byte 1 | Byte 2 | Byte 3 | Byte 4 | Byte 5 |
| ------ | ------ | ------ | ------ | ------ | ------ |
| HEADER | ADDH | ADDL | SPED | CHAN | OPTION |

