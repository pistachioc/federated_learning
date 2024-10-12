### Nums of normal and 9 attack types record collected on Win7-10 

| Type of Events | Windows 7 | Windows 10 |
|----------------|-----------|------------|
| Normal         | 22,387    | 24,871     |
| Backdoor       | 1,779     | -          |
| DDoS           | 2,134     | 4,608      |
| Ransomware     | -         | 82         |
| Injection      | 998       | 612        |
| XSS            | 4         | 1,268      |
| Password       | 757       | 3,628      |
| Scanning       | 226       | 447        |
| DoS            | -         | 525        |
| MITM           | -         | 15         |
### 10 most correlated features (data types are numeric) in Win7
| Tên Thuộc Tính                                      | Mô Tả Thuộc Tính                                                                                                                           |
| --------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------ |
| `Process Total IO Other Bytes/sec`                  | Quá trình phát hành các byte cho các hoạt động I/O không liên quan đến dữ liệu, chẳng hạn như các hoạt động điều khiển.                    |
| `Network I.Intel R Pro 1000MT Bytes Received/sec`   | Tốc độ byte được nhận qua mỗi bộ điều hợp mạng, bao gồm cả các ký tự đóng khung.                                                           |
| `Process Total IO Other Operations/sec`             | Tốc độ quá trình phát hành các hoạt động I/O không phải là hoạt động đọc hoặc ghi (ví dụ: một chức năng điều khiển).                       |
| `Process Total IO Data Bytes/sec`                   | Tốc độ quá trình đọc và ghi byte trong các hoạt động I/O.                                                                                  |
| `Process Total IO Read Bytes/sec`                   | Tốc độ quá trình đọc byte từ các hoạt động I/O.                                                                                            |
| `Network I.Intel.R Pro 1000MT Bytes Received/sec`   | Tốc độ byte được nhận qua mỗi bộ điều hợp mạng.                                                                                            |
| `Process Pool Paged Bytes`                          | Kích thước, tính bằng byte, của bộ nhớ ảo có phân trang của hệ thống, được sử dụng cho các đối tượng có thể ghi vào đĩa khi không sử dụng. |
| `Network I.Intel.R Pro 1000MT Bytes Sent/sec`       | Tốc độ byte được gửi qua mỗi bộ điều hợp mạng, bao gồm cả các ký tự đóng khung.                                                            |
| `Network I.Intel.R Pro 1000MT Packets Received/sec` | Tốc độ gói tin được nhận trên giao diện mạng.                                                                                              |
| `Process Total IO Data Operations/sec`              | Tốc độ quá trình phát hành các hoạt động I/O đọc và ghi.                                                                                   |
### 10 most correlated features (data types are numeric) in Win10
| Tên Thuộc Tính                                          | Mô Tả Thuộc Tính                                                                                                |
| ------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------- |
| `Network I.Intel.R 82574L GNC.Current Bandwidth`        | Băng thông hiện tại của giao diện mạng, được tính bằng bit mỗi giây (BPS).                                      |
| `Network I.Intel.R 82574L GNC.Packets Sent Unicast/sec` | Tốc độ gói tin được yêu cầu để truyền đến các địa chỉ unicast bởi các giao thức cấp cao hơn.                    |
| `Memory.Pool.Paged Bytes`                               | Kích thước, tính bằng byte, của phần bộ nhớ ảo có phân trang hiện đang cư trú và hoạt động trong bộ nhớ vật lý. |
| `LogicalDisk.Total Disk Read Bytes/sec`                 | Tốc độ byte được chuyển từ đĩa trong các thao tác đọc.                                                          |
| `Memory.Page Reads/sec`                                 | Tốc độ đọc từ đĩa để giải quyết các lỗi trang cứng (hard page faults).                                          |
| `Network I.Intel.R 82574L GNC.Packets Sent/sec`         | Tốc độ gói tin được gửi trên giao diện mạng.                                                                    |
| `Memory.Modified.Page List Bytes`                       | Lượng bộ nhớ vật lý, tính bằng byte, được gán cho danh sách trang đã sửa đổi.                                   |
| `Process IO Data Operations/sec`                        | Tốc độ mà quá trình phát hành các thao tác I/O đọc và ghi dữ liệu.                                              |
| `LogicalDisk.Total Avg.Disk.Bytes Transfer`             | Số byte trung bình được chuyển đến hoặc từ đĩa trong các thao tác ghi hoặc đọc.                                 |
| `Processor % Processor Time`                            | Lượng thời gian mà bộ xử lý sử dụng để thực thi một luồng không ở trạng thái nhàn rỗi.                          |
