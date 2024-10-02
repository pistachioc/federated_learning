### 1. Raw datasets
- IOT/IIOT data ghi bằng file **log** và **csv** mà các sensor như thời tiết thu thập dữ liệu từ xa
- Network data ở dạng file **pcap** (packet capture), **log**, và **csv** qua công cụ *ZEEK*
- Linux data cho việc logging desk, process, processor, memory và network activities ở dang **txt** và **csv** sử dụng lệnh *atop* (tracing tool)
- Win data ở dạng **blg** thu thập như linux rồi mở trong file **csv** sử dụng *Performance Monitor Tool on Windows 7 and 10*
### 2. Processed datasets
- 4 data trên được lọc để tạo ra **features** và **label** rồi định dạng ở file **csv** 
- Các feature mới này được mô tả trong ‘*Description_stats_datasets*’
### 3. Train_Test_datasets
- Bao gồm các **samples** của 4 data phía trên ở dạng **csv** dùng cho model AI
- Số lượng records bao gồm normal và attack types cho training và testing thuật toán được mô tả trong *’Description_stats_datasets’*
### 4. Description_stats_datasets
- Mô tả các features và thống kê của chúng
### 5. SecurityEvents_GroundTruth_datasets
- Có các security events of hacking happened trong 4 datasets
- Labeled dựa trên IP add và timestamps trong 4 datasets