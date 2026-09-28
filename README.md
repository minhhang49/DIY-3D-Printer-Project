# DIY-3D-Printer-Project

## Firmware

Firmware được xây dựng dựa trên Marlin 2.x. Thư mục này chứa các tệp cấu hình và build đã được điều chỉnh để phù hợp với máy in 3D FDM tự chế tạo sử dụng MKS TinyBee.

**Cấu trúc thư mục**

03_Firmware/
├── Marlin/
├── ini/
└── platformio.ini

**Cài đặt và sử dụng Firmware**

Các tệp được đưa lên GitHub là các tệp đã chỉnh sửa, không phải toàn bộ mã nguồn Marlin.
Để sử dụng firmware, thực hiện theo các bước sau:

**Bước 1: Tải Marlin gốc**

Tải phiên bản Marlin 2.x tương ứng với phiên bản được sử dụng trong project.
Marlin Firmware: https://github.com/makerbase-mks/MKS-TinyBee/tree/main/firmware
Nên sử dụng đúng phiên bản Marlin đã được sử dụng trong project để tránh lỗi tương thích.

**Bước 2: Giải nén Marlin**

Sau khi tải Marlin gốc, giải nén và mở thư mục Marlin.

**Bước 3: Copy các tệp đã chỉnh sửa**

Copy các tệp và thư mục đã được cung cấp trong thư mục 03_Firmware của project vào đúng vị trí tương ứng trong Marlin gốc.
Khi được hỏi, chọn: Replace / Replace the files in the destination

**Bước 4: Mở project bằng Visual Studio Code**

Mở thư mục Marlin gốc đã được thay thế các tệp cấu hình bằng: Visual Studio Code + PlatformIO

**Bước 5: Biên dịch Firmware**

Trong Visual Studio Code, sử dụng PlatformIO để Build firmware.
Nếu quá trình Build không xuất hiện lỗi, firmware có thể được nạp vào MKS TinyBee.

**Bước 6: Nạp Firmware**

Kết nối MKS TinyBee với máy tính thông qua USB và sử dụng PlatformIO để Upload firmware.
