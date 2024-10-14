- **44 features classified into four groups** 
- 2 new attributes, namely *label* and *type* were added to tag the entire vectors in the datasets listed in Table 7
> label attribute can be used when a binary classification model is used to classify normal and attack data. The type attributes can be applied when a multi classification model is used to classify normal and attack types
### First group - connection atriibutes
- Contains infos about flow indentifiers - sour, des IPs, ports, protocol types, … 
Table1: Connection Features

| ID  | Feature        | Type       | Description                                                                                                                          |
| --- | -------------- | ---------- | ------------------------------------------------------------------------------------------------------------------------------------ |
| 1   | `ts`           | Time stamp | Timestamp of connection between flow identifiers                                                                                     |
| 2   | `src_ip`       | String     | Source IP addresses which originate endpoints’ IP addresses                                                                          |
| 3   | `src_port`     | Number     | Source ports which originate endpoint’s TCP/UDP ports                                                                                |
| 4   | `dst_ip`       | String     | Destination IP addresses which respond to endpoint’s IP addresses                                                                    |
| 5   | `dst_port`     | Number     | Destination ports which respond to endpoint’s TCP/UDP ports                                                                          |
| 6   | `proto`        | String     | Transport layer protocols of flow connections                                                                                        |
| 7   | `service`      | String     | Dynamically detected protocols, such as DNS, HTTP, and SSL                                                                           |
| 8   | `duration`     | Number     | The time of the packet connections, estimated by subtracting ‘time of the last packet seen’ and ‘time of the first packet seen’      |
| 9   | `src_bytes`    | Number     | Source bytes which are originated from payload bytes of TCP sequence numbers                                                         |
| 10  | `dst_bytes`    | Number     | Destination bytes which are responded payload bytes from TCP sequence numbers                                                        |
| 11  | `conn_state`   | String     | Various connection states, such as S0 (connection without reply), S1 (connection established), and REJ (connection attempt rejected) |
| 12  | `missed_bytes` | Number     | Number of missing bytes in content gaps                                                                                              |


### Second group - statistical attributes
- Comprise info about the numbers of flow identifiers and their statistics 
Table 2: Statistical features

| ID  | Feature        | Type   | Description                                                                                               |
| --- | -------------- | ------ | --------------------------------------------------------------------------------------------------------- |
| 13  | `src_pkts`     | Number | Số lượng gói tin gốc được gửi từ hệ thống nguồn.                                                          |
| 14  | `src_ip_bytes` | Number | Tổng số byte IP gốc, bao gồm tổng chiều dài của trường tiêu đề IP (IP header) được gửi từ hệ thống nguồn. |
| 15  | `dst_pkts`     | Number | Số lượng gói tin gốc được gửi từ hệ thống đích.                                                           |
| 16  | `dst_ip_bytes` | Number | Tổng số byte IP gốc, bao gồm tổng chiều dài của trường tiêu đề IP (IP header) được gửi từ hệ thống đích.  |
- `src_bytes` tính mỗi PAYLOAD, còn `src_ip_bytes` tính cả PACKET (header + payload)
### Third group - user-centric
- Info about high-level services and their interactions with end-users
Table 3: DNS features

| ID  | Feature        | Type    | Description                                                                                     |
| --- | -------------- | ------- | ----------------------------------------------------------------------------------------------- |
| 17  | `dns_query`    | String  | Tên miền được yêu cầu trong các truy vấn DNS.                                                   |
| 18  | `dns_qclass`   | Number  | Giá trị số mô tả lớp truy vấn DNS, như IN (Internet) hoặc CH (Chaos).                           |
| 19  | `dns_qtype`    | Number  | Giá trị số mô tả loại truy vấn DNS, như A (Address Record), AAAA (IPv6 Address), CNAME (Alias). |
| 20  | `dns_rcode`    | Number  | Mã phản hồi (Response code) trong phản hồi DNS, như NOERROR, NXDOMAIN, SERVFAIL.                |
| 21  | `dns_AA`       | Boolean | Trả lời có thẩm quyền của DNS, nếu `True` thì máy chủ DNS là máy chủ chính cho truy vấn.        |
| 22  | `dns_RD`       | Boolean | Yêu cầu truy vấn đệ quy trong DNS, nếu `True` thì yêu cầu tìm kiếm đệ quy cho truy vấn.         |
| 23  | `dns_RA`       | Boolean | Truy vấn đệ quy có sẵn trong DNS, nếu `True` thì máy chủ hỗ trợ truy vấn đệ quy.                |
| 24  | `dns_rejected` | Boolean | Truy vấn DNS bị từ chối, nếu `True` thì truy vấn bị máy chủ DNS từ chối.                        |
Table 4: SSL features

| ID  | Feature           | Type    | Description                                                                                                               |
| --- | ----------------- | ------- | ------------------------------------------------------------------------------------------------------------------------- |
| 25  | `ssl_version`     | String  | Phiên bản SSL được máy chủ cung cấp.                                                                                      |
| 26  | `ssl_cipher`      | String  | Bộ mã hóa SSL mà máy chủ đã chọn.                                                                                         |
| 27  | `ssl_resumed`     | Boolean | Cờ SSL cho biết phiên làm việc có thể được sử dụng để khởi tạo các kết nối mới, `True` nếu kết nối SSL đã được khởi động. |
| 28  | `ssl_established` | Boolean | Cờ SSL chỉ ra việc thiết lập kết nối giữa hai bên, `True` nếu kết nối đã được thiết lập.                                  |
| 29  | `ssl_subject`     | String  | Chủ thể của chứng chỉ X.509 được máy chủ cung cấp.                                                                        |
| 30  | `ssl_issuer`      | String  | Chủ sở hữu/nguồn gốc đáng tin cậy của SSL và chứng chỉ số (cơ quan cấp chứng chỉ).                                        |
Table 5: HTTP features

| ID  | Feature                  | Type   | Description                                                              |
| --- | ------------------------ | ------ | ------------------------------------------------------------------------ |
| 31  | `http_trans_depth`       | Number | Độ sâu của các truy vấn HTTP được xếp chồng lên nhau.                    |
| 32  | `http_method`            | String | Phương thức yêu cầu HTTP, như GET, POST, HEAD.                           |
| 33  | `http_uri`               | String | URI được sử dụng trong yêu cầu HTTP.                                     |
| 34  | `http_referrer`          | String | Giá trị của header 'referer' trong giao thức HTTP.                       |
| 35  | `http_version`           | String | Phiên bản HTTP được sử dụng, như HTTP/1.1.                               |
| 36  | `http_request_body_len`  | Number | Kích thước thực tế của nội dung không nén được chuyển từ máy khách HTTP. |
| 37  | `http_response_body_len` | Number | Kích thước thực tế của nội dung không nén được chuyển từ máy chủ HTTP.   |
| 38  | `http_status_code`       | Number | Mã trạng thái trả về từ máy chủ HTTP.                                    |
| 39  | `http_user_agent`        | String | Giá trị của header 'User-Agent' trong giao thức HTTP.                    |
| 40  | `http_orig_mime_types`   | String | Danh sách các kiểu MIME từ hệ thống nguồn trong giao thức HTTP.          |
| 41  | `http_resp_mime_types`   | String | Danh sách các kiểu MIME từ hệ thống đích trong giao thức HTTP.           |

### Fourth group - violation attributes
- Include any abnormal info happened while transmitting packets listed in 
Table 6: Violation features

| ID  | Feature        | Type    | Description                                                                |
| --- | -------------- | ------- | -------------------------------------------------------------------------- |
| 42  | `weird_name`   | String  | Tên của các bất thường/vi phạm liên quan đến các giao thức đã xảy ra.      |
| 43  | `weird_addl`   | String  | Thông tin bổ sung liên quan đến các bất thường/vi phạm giao thức.          |
| 44  | `weird_notice` | Boolean | Cờ chỉ ra liệu vi phạm/bất thường đã được chuyển thành thông báo hay chưa. |
Table 7: Labeling atributes

| ID  | Feature | Type   | Description                                                                                                              |
| --- | ------- | ------ | ------------------------------------------------------------------------------------------------------------------------ |
| 45  | `label` | Number | Ghi nhãn các bản ghi bình thường và tấn công, trong đó 0 chỉ định bình thường và 1 chỉ định tấn công.                    |
| 46  | `type`  | String | Ghi nhãn các loại tấn công, chẳng hạn như bình thường, DoS, DDoS và tấn công backdoor, cùng với các bản ghi bình thường. |
Table 8: Numbers of records

|               | Total data records | Train_Test records |
| ------------- | ------------------ | ------------------ |
| Backdoor      | 508,116            | 20,000             |
| DDoS          | 6,165,008          | 20,000             |
| DoS           | 3,375,328          | 20,000             |
| Injection     | 452,659            | 20,000             |
| MITM          | 1,052              | 1,043              |
| Password      | 1,718,568          | 20,000             |
| Ransomware    | 72,805             | 20,000             |
| Scanning      | 7,140,161          | 20,000             |
| XSS           | 2,108,944          | 20,000             |
| Bình Thường   | 796,380            | 300,000            |
| **Tổng Cộng** | **22,339,021**     | **461,043**        |
