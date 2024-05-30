   # JMeter
## Kiểm tra hiệu năng trang web
  ### Mục tiêu:

  - Sử dụng jMeter để tạo một kịch bản kiểm tra mô phỏng người dùng truy cập trang web https://www.coursera.org/learn/machine-learning.
  - Chạy kịch bản kiểm tra và ghi lại kết quả.
  - Phân tích kết quả kiểm tra, bao gồm thời gian phản hồi, số lượng yêu cầu thành công, số lượng yêu cầu thất bại, v.v.
  - Dựa trên kết quả phân tích, đưa ra kết luận về hiệu năng của trang web.

  ### Kịch bản kiểm tra:

- Thread Group:
  - Số lượng thread: 100
  - Thời gian chạy: 60 giây
  - Ramp-up period: 10 giây
- HTTP Request:
  - URL: https://www.coursera.org/learn/machine-learning
  - Method: GET
  - Content encoding: UTF-8
- Listeners:
  - View Results Tree
  - Aggregate Report
### Kết quả kiểm tra:
![MACHINE](https://github.com/Nguyenha2112/Jmeter/assets/96609701/c866cbbc-3926-42e0-8869-753a6663d6e4)

![KetquaMACHINE1](https://github.com/Nguyenha2112/Jmeter/assets/96609701/6955348d-c9a4-4547-b58e-212fdab470b0)



### Phân tích kết quả kiểm tra:

- Số lượng yêu cầu thành công: 1000/1000 = 100%
- Số lượng yêu cầu thất bại: 0/1000 = 0%
- Thời gian phản hồi trung bình: 29,48 ms
- Thời gian phản hồi trung vị: 27,08 ms
- Thời gian phản hồi percentil 90: 47,77 ms
- Chuyển tải: 12 yêu cầu/giây
  
### Kết luận:
Trang web https://www.coursera.org/learn/machine-learning có hiệu năng tốt. Số lượng yêu cầu thành công rất cao (100%), số lượng yêu cầu thất bại rất thấp (0,00%). Thời gian phản hồi trung bình, trung vị và percentil 90 đều ở mức thấp (dưới 100 ms). Chuyển tải của trang web cũng khá cao (12 yêu cầu/giây).

## Kiểm tra hiệu năng API

### Mục tiêu:

- Sử dụng jMeter để tạo một kịch bản kiểm tra mô phỏng người dùng truy cập API thời tiết https://openweathermap.org/current.
- Chạy kịch bản kiểm tra và ghi lại kết quả.
- Phân tích kết quả kiểm tra, bao gồm thời gian phản hồi, số lượng yêu cầu thành công, số lượng yêu cầu thất bại, v.v.
- Dựa trên kết quả phân tích, đưa ra kết luận về hiệu năng của API.

  
### Kịch bản kiểm tra:
- Thread Group:
  - Số lượng thread: 100
  - Thời gian chạy: 60 giây
  - Ramp-up period: 10 giây
- HTTP Request:
  - URL: https://openweathermap.org/current
  - Method: GET
  - Content encoding: UTF-8
- Listeners:
  - View Results Tree
  - Aggregate Report
### Kết quả kiểm tra:

![API](https://github.com/Nguyenha2112/Jmeter/assets/96609701/0d3ed162-fcdf-465f-bda1-023ff27d7cb5)

![KetquaAPI](https://github.com/Nguyenha2112/Jmeter/assets/96609701/cf31058f-fde5-4247-853c-f007df79034a)


### Phân tích kết quả kiểm tra:

- Số lượng yêu cầu thành công: 993/1000 = 99,63%
- Số lượng yêu cầu thất bại: 7/1000 = 0,37%
- Thời gian phản hồi trung bình: 80,77 ms
- Thời gian phản hồi trung vị: 74,12 ms
- Thời gian phản hồi percentil 90: 110,79 ms
- Chuyển tải: 5 yêu cầu/giây
  
### Kết luận:
Trang web https://openweathermap.org/current có hiệu năng tốt. Số lượng yêu cầu thành công trung bình (99,63%), số lượng yêu cầu thất bại thấp (0,37%). Thời gian phản hồi trung bình, trung vị đều ở mức thấp (dưới 100 ms). Chuyển tải của trang web trung bình(5 yêu cầu/giây).

## So Sánh :
Với 2 trang web https://www.coursera.org/learn/machine-learning và https://openweathermap.org/current thì trang web https://www.coursera.org/learn/machine-learning có hiệu năng tốt hơn khi có thể phản hồi số lượng request lớn hơn, tỉ lệ lỗi nhỏ hơn, thời gian phản hồi nhanh hơn
