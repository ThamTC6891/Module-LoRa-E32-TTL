# Module-LoRa-E32-TTL
# Phần này mình sẽ trình bày cách thức setting các tham số cho module LoRa UART
# Trước tiên các bạn hãy chuẩn bị những thứ sau:
* 1/ User Manual cho module dạng TTL, các bạn có thể xem tại đây http://www.inhaos.com/uploadfile/otherpic/DS-RF-TTL-100-V01-EN.pdf 
* 2/ Cách nối dây giữa LoRa với MCU như bên dưới (ở đây lấy ví dụ là Arduino) 
Module LoRa ******** Arduino
AUX      ----------> Not connect
M0, M1     --------> Pin Output (vd: Pin 3)
TXD      ----------> RXD 
RXD      ----------> TXD 
GND      ----------> GND
5V      -----------> 5V
