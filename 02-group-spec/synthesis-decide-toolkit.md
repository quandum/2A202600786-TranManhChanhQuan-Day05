# Synthesis Decide Toolkit

## 1. Gom evidence thành cụm

### Cụm 1

Không biết bắt đầu lập kế hoạch từ đâu.

### Cụm 2

Không biết chọn khách sạn hoặc khu vực lưu trú.

### Cụm 3

Đọc quá nhiều nguồn nhưng khó tổng hợp thành lịch trình.

### Cụm 4

AI dễ sinh lịch trình không phù hợp khi thiếu thông tin.

---

## 2. Insight

Người đi du lịch tự túc không chỉ cần danh sách địa điểm.

Họ thật ra cần hỗ trợ ra quyết định và ghép các lựa chọn thành một kế hoạch hoàn chỉnh.

Vì nhiều người phải đọc nhiều nguồn khác nhau và không biết lựa chọn nào phù hợp với nhu cầu của mình.

---

## 3. Opportunity

Cơ hội là dùng AI để tự động thu thập intent còn thiếu và sinh itinerary sơ bộ.

Giúp người dùng có kế hoạch du lịch trong vài phút.

Trong khi vẫn kiểm soát rủi ro bằng cơ chế hỏi lại khi thông tin chưa đủ.

---

## 4. Chọn build slice

| Câu hỏi               | Đánh giá |
| ----------------------- | ----------- |
| User cụ thể chưa?    | Có         |
| Task đủ hẹp chưa?   | Có         |
| AI decision rõ chưa?  | Có         |
| Failure path rõ chưa? | Có         |
| Có evidence không?    | Có         |

Build Slice:

User nhập yêu cầu du lịch → AI hỏi lại intent còn thiếu → tạo itinerary 3 ngày → đề xuất khách sạn.

---

## 5. Quyết định

Ý tưởng quá rộng.

Giữ domain Travel Planning.

Giảm scope xuống:

Intent Collection + Itinerary Generation.

Không build:

* Booking
* Thanh toán
* Visa
* Vé máy bay

---

## 6. Câu chốt cuối

Dựa trên evidence,

nhóm sẽ build prototype slice:

AI Travel Planner.

Cho khách du lịch tự túc.

Để giải quyết việc mất nhiều thời gian lập kế hoạch.

Bằng cách AI tự động thu thập intent và sinh itinerary.

Và sẽ test failure path khi người dùng cung cấp thiếu thông tin.

---

## 7. Backlog

* Đặt khách sạn
* Đặt vé máy bay
* Weather integration
* Budget optimization
* Multi-city planning
* Travel companion mode
