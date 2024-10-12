### Linux disk 
| ID  | Tên Thuộc Tính | Loại   | Mô Tả                                                                                                                    |
| --- | -------------- | ------ | ------------------------------------------------------------------------------------------------------------------------ |
| 1   | `PID`          | Number | Định danh của tiến trình đang hoạt động trong nhân Linux.                                                                |
| 2   | `RDDSK`        | Number | Lượng dữ liệu được đọc từ đĩa.                                                                                           |
| 3   | `WRDSK`        | Number | Lượng dữ liệu được ghi vào đĩa.                                                                                          |
| 4   | ``WCANCL``     | Number | Lượng dữ liệu đã được ghi nhưng đã bị hủy bỏ.                                                                            |
| 5   | `DSK`          | Number | Phần trăm dung lượng đĩa được chiếm dụng.                                                                                |
| 6   | `CMD`          | String | Tên tiến trình đang hoạt động trong nhân Linux.                                                                          |
| 7   | `label`        | Number | Gán nhãn cho bản ghi bình thường và tấn công, với 0 chỉ định bình thường và 1 chỉ định tấn công.                         |
| 8   | `type`         | String | Gán nhãn các loại tấn công, chẳng hạn như bình thường, DoS, DDoS và tấn công backdoor, cũng như các bản ghi bình thường. |
### Linux process 
| ID  | Tên Thuộc Tính | Loại   | Mô Tả                                                                                                                                          |
| --- | -------------- | ------ | ---------------------------------------------------------------------------------------------------------------------------------------------- |
| 1   | `PID`          | Number | Định danh của tiến trình đang hoạt động trong nhân Linux.                                                                                      |
| 2   | `TRUN`         | Number | Số lượng luồng đang ở trạng thái chạy (R).                                                                                                     |
| 3   | `TSLPI`        | Number | Số lượng luồng đang ở trạng thái ngủ có thể bị gián đoạn (S).                                                                                  |
| 4   | `TSLPU`        | Number | Số lượng luồng đang ở trạng thái ngủ không thể bị gián đoạn (D).                                                                               |
| 5   | `POLI`         | String | Chính sách lập lịch (chia sẻ thời gian bình thường, quay vòng thời gian thực, fifo thời gian thực).                                            |
| 6   | `NICE`         | Number | Giá trị ưu tiên "nice" của tiến trình, từ -20 (ưu tiên cao) đến +19 (ưu tiên thấp).                                                            |
| 7   | `PRI`          | Number | Độ ưu tiên của tiến trình, từ 0 (cao nhất) đến 139 (thấp nhất).                                                                                |
| 8   | `RTPR`         | Number | Độ ưu tiên thời gian thực theo tiêu chuẩn POSIX. Giá trị từ 0 (tiến trình chia sẻ thời gian) đến 99 (thời gian thực cao nhất).                 |
| 9   | `CPUNR`        | Number | Số định danh CPU hiện tại mà luồng chính của tiến trình đang chạy hoặc đã chạy gần đây.                                                        |
| 10  | `Status`       | Number | Trạng thái của tiến trình, vị trí đầu tiên cho biết tiến trình đã bắt đầu trong khoảng thời gian gần đây hay chưa (N nghĩa là tiến trình mới). |
| 11  | `EXC`          | Number | Mã thoát của tiến trình đã kết thúc hoặc số hiệu tín hiệu chết người (fatal signal number).                                                    |
| 12  | `State`        | String | Trạng thái hiện tại của luồng chính của tiến trình.                                                                                            |
| 13  | `CPU`          | Number | Thời gian CPU tiêu thụ của tiến trình ở chế độ hệ thống (kernel mode), thường do xử lý các lời gọi hệ thống.                                   |
| 14  | `CMD`          | String | Tên của tiến trình. Nếu tên được bao quanh bởi dấu < hoặc >, điều đó có nghĩa là tiến trình đã kết thúc trong khoảng thời gian gần đây.        |
| 15  | `label`        | Number | Gán nhãn cho bản ghi bình thường và tấn công, với 0 chỉ định bình thường và 1 chỉ định tấn công.                                               |
| 16  | `type`         | String | Gán nhãn các loại tấn công, chẳng hạn như bình thường, DoS, DDoS và tấn công backdoor, cũng như các bản ghi bình thường.                       |
### Linux memory
| ID  | Tên Thuộc Tính | Loại   | Mô Tả                                                                                                                               |
| --- | -------------- | ------ | ----------------------------------------------------------------------------------------------------------------------------------- |
| 1   | `PID`          | Number | Định danh của tiến trình đang hoạt động trong nhân Linux.                                                                           |
| 2   | `MINFLT`       | Number | Số lần lỗi trang (page fault) mà tiến trình phát sinh, được giải quyết bằng cách thu hồi trang bộ nhớ từ danh sách các trang trống. |
| 3   | `MAJFLT`       | Number | Số lần lỗi trang mà tiến trình phát sinh, được giải quyết bằng cách tạo hoặc tải trang bộ nhớ được yêu cầu.                         |
| 4   | `VSTEXT`       | Number | Kích thước bộ nhớ ảo được sử dụng bởi phần văn bản chia sẻ của tiến trình này.                                                      |
| 5   | `VSIZE`        | Number | Tổng lượng bộ nhớ ảo mà tiến trình này tiêu thụ.                                                                                    |
| 6   | `RSIZE`        | Number | Tổng lượng bộ nhớ cư trú mà tiến trình này tiêu thụ.                                                                                |
| 7   | `VGROW`        | Number | Lượng bộ nhớ ảo mà tiến trình đã tăng lên trong khoảng thời gian gần đây.                                                           |
| 8   | `RGROW`        | Number | Lượng bộ nhớ cư trú mà tiến trình đã tăng lên trong khoảng thời gian gần đây.                                                       |
| 9   | `MEM`          | Number | Phần trăm bộ nhớ bị chiếm dụng.                                                                                                     |
| 10  | `CMD`          | String | Tên tiến trình.                                                                                                                     |
| 11  | `label`        | Number | Gán nhãn cho các bản ghi bình thường và tấn công, với 0 là bình thường và 1 là tấn công.                                            |
| 12  | `type`         | String | Gán nhãn các loại tấn công như bình thường, DoS, DDoS và tấn công backdoor, cũng như các bản ghi bình thường.                       |
