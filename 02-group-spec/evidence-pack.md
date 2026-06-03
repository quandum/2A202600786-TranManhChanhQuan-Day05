
# Evidence Pack

## 1. Nhóm và Track

**Tên nhóm:** Những Người Hành Khất

**Track:** AI Agent

**Product/App đã chọn:** AI Travel Planner Agent

**Build Slice đang nghĩ:**

AI Travel Planner Agent là một hệ thống AI Agent hỗ trợ lập kế hoạch du lịch đầu-cuối (end-to-end). Người dùng chỉ cần mô tả nhu cầu bằng ngôn ngữ tự nhiên, agent sẽ tự động thu thập và làm rõ các intent còn thiếu, sau đó sử dụng nhiều công cụ để tìm kiếm địa điểm, tối ưu lịch trình, hiển thị trên bản đồ và gợi ý khách sạn hoặc dịch vụ phù hợp. Thay vì chỉ trả lời câu hỏi, agent có khả năng chủ động lập kế hoạch và hỗ trợ ra quyết định, giúp người dùng xây dựng một chuyến đi hoàn chỉnh trong vài phút.

Mục tiêu của product không phải thay thế hoàn toàn việc lên kế hoạch du lịch, mà giúp người dùng rút ngắn đáng kể thời gian ra quyết định.

---

# 2. Self-use Evidence

Nhóm tự thực hiện workflow lên kế hoạch du lịch để quan sát điểm gãy.

| Observation    | Screenshot / Link                                            | Path liên quan   | Điều học được                                                                        |
| -------------- | ------------------------------------------------------------ | ----------------- | ------------------------------------------------------------------------------------------ |
| Happy          | Lên lịch trình Đà Nẵng 3N2Đ với ngân sách 8 triệu | Planning          | Khi yêu cầu rõ ràng, AI tạo kế hoạch nhanh và khá hợp lý                        |
| Low-confidence | "Tôi muốn đi Nhật"                                       | Intent Collection | Thiếu dữ liệu quan trọng khiến AI không thể đưa ra kế hoạch đáng tin cậy     |
| Failure        | Tìm "lịch trình tối ưu nhất cho Đà Lạt"             | Decision Support  | Không tồn tại một lịch trình tối ưu tuyệt đối cho mọi người                  |
| Correction     | AI hỏi lại số ngày, ngân sách và sở thích           | Clarification     | Hỏi lại đúng lúc giúp giảm đáng kể khả năng tạo lịch trình không phù hợp |

### Observation nổi bật

Nhóm thử tự lập kế hoạch cho chuyến đi Đà Nẵng.

Workflow thực tế:

Google Search → Blog Review → Google Maps → Agoda → TikTok Review → Tổng hợp thủ công

Tổng thời gian khoảng 35–45 phút.

Khó khăn lớn nhất không phải là tìm địa điểm.

Khó khăn lớn nhất là quyết định:

* Đi đâu trước?
* Ở khu vực nào?
* Ngân sách có đủ không?
* Có bỏ sót địa điểm nổi bật nào không?

---

# 3. User / Review / Social Evidence

| Quote / Observation                                          | Nguồn                | User là ai?                  | Pain / Failure Mode         |
| ------------------------------------------------------------ | --------------------- | ----------------------------- | --------------------------- |
| "Mất cả buổi tối để lên lịch trình đi Phú Quốc." | Phỏng vấn nhanh     | Sinh viên                    | Planning tốn thời gian    |
| "Không biết nên ở khu vực nào để tiện đi lại."    | Travel Facebook Group | Du khách tự túc            | Khó đưa ra quyết định |
| "Đọc quá nhiều blog nhưng mỗi nơi nói một kiểu."   | Reddit Travel         | Người mới du lịch         | Quá tải thông tin        |
| "Tôi thường mở 5-6 tab cùng lúc để so sánh."        | Phỏng vấn nhanh     | Người đi du lịch tự túc | Workflow phân mảnh        |

Nếu chưa có đủ nguồn ngoài nhóm:

Đây là giả định ban đầu. Nhóm sẽ kiểm chứng thêm bằng cách phỏng vấn tối thiểu 3 người từng tự lên kế hoạch du lịch trước checkpoint M1 Day 06.

---

# 4. Competitor / Analog Evidence

| App / Model   | Họ xử lý thế nào?              | Pattern học được                  | Áp dụng trong 1 ngày? |
| ------------- | ----------------------------------- | ------------------------------------- | ------------------------ |
| Google Maps   | Gợi ý địa điểm và route      | Hiển thị trực quan trên bản đồ | Có                      |
| TripAdvisor   | Ranking + Review cộng đồng       | Social Proof                          | Có                      |
| Wonderplan AI | Sinh itinerary tự động           | AI Planning Flow                      | Có                      |
| ChatGPT       | Clarification trước khi trả lời | Intent Collection                     | Có                      |

---

# 5. Evidence → Insight

### Evidence nổi bật nhất

Người dùng không thiếu thông tin du lịch.

Ngược lại, họ đang phải xử lý quá nhiều thông tin từ nhiều nguồn khác nhau.

### Insight

User không chỉ gặp khó trong việc tìm địa điểm.

Thật ra họ cần hỗ trợ ra quyết định và tổng hợp lựa chọn thành một kế hoạch khả thi phù hợp với thời gian, ngân sách và sở thích cá nhân.

### Opportunity

AI có thể đóng vai trò một Travel Planning Copilot:

* Thu thập thông tin còn thiếu
* Tổng hợp thông tin từ nhiều nguồn
* Sinh kế hoạch du lịch sơ bộ

Để người dùng chỉnh sửa thay vì phải xây dựng toàn bộ kế hoạch từ đầu.

---

# 6. Evidence đổi SPEC như thế nào?

☑ Đổi Build Slice

☑ Đổi Auto/Aug Decision

☑ Đổi Failure Mode

### Thay đổi quan trọng

Trước evidence:

Nhóm muốn build một Travel Agent end-to-end có thể lên kế hoạch, gợi ý khách sạn, đặt dịch vụ và hỗ trợ toàn bộ chuyến đi.

Sau evidence:

Nhóm tập trung vào một build slice nhỏ hơn:

AI Agent hỗ trợ yêu cầu còn thiếu và từ đó gợi ý lịch trình cá nhân hoá theo yêu cầu.

### Lý do

Đây là painpoint xuất hiện rõ nhất trong self-use và có thể demo được trong thời gian giới hạn của Day 06.
