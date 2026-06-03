# Thin SPEC

## 1. Track, Product và User

**Track:** AI Agent

**Product:** AI Travel Planner Agent

**User cụ thể:**

Người đi du lịch tự túc, chưa có lịch trình và không muốn mất hàng giờ nghiên cứu thông tin trước chuyến đi.

**Nhóm có phải user thật không?**

Có. Tất cả thành viên đều từng tự lên kế hoạch du lịch và gặp khó khăn trong việc tổng hợp thông tin.

---

## 2. Evidence Summary

| Evidence                                           | Nguồn          | User/Pain          | SPEC thay đổi                      |
| -------------------------------------------------- | --------------- | ------------------ | ------------------------------------ |
| Mất 35–45 phút để tự lập lịch trình       | Self-use        | Workflow quá dài | Tập trung vào itinerary generation |
| Thiếu dữ liệu đầu vào làm AI trả lời kém | Observation     | Thiếu trust       | Thêm clarification loop             |
| Quá tải thông tin từ nhiều nguồn             | Review + Social | Decision fatigue   | Tập trung decision support          |

---

## 3. Pain Statement

Người đi du lịch tự túc gặp khó khăn ở bước lập kế hoạch.

Vì phải tìm kiếm, đối chiếu và tổng hợp thông tin từ nhiều nguồn khác nhau.

Dẫn tới mất nhiều thời gian chuẩn bị và khó đưa ra quyết định.

Bằng chứng chính là self-use observation và phản hồi từ cộng đồng du lịch.

---

## 4. Build Slice

Cho người đang chuẩn bị một chuyến du lịch.

Prototype sẽ dùng AI để:

1. Thu thập intent còn thiếu.
2. Hiểu ngân sách, thời gian và sở thích.
3. Tạo itinerary 3 ngày sơ bộ.
4. Hiển thị itinerary trên bản đồ.

### Output

* Itinerary theo ngày
* Danh sách địa điểm
* Route trực quan trên bản đồ

### Failure Mode

Thông tin đầu vào không đủ hoặc quá mơ hồ.

### Mitigation

AI hỏi lại trước khi lập kế hoạch.

---

## 5. Auto/Aug Decision

☑ Augmentation

### Lý do

AI không thay người dùng quyết định chuyến đi.

AI chỉ tạo kế hoạch sơ bộ và hỗ trợ ra quyết định.

Người dùng vẫn là người lựa chọn lịch trình cuối cùng.

### Human Role

Decider

---

## 6. Four Paths

| Path           | Prototype phải thể hiện gì                            |
| -------------- | --------------------------------------------------------- |
| Happy          | User cung cấp đầy đủ thông tin → AI tạo itinerary |
| Low-confidence | Thiếu ngân sách hoặc thời gian → AI hỏi lại       |
| Failure        | AI tạo lịch trình vượt quá ngân sách thực tế    |
| Correction     | User chỉnh ngân sách → AI tạo lại lịch trình      |

---

## 7. Failure Mode Nguy Hiểm Nhất

### Trigger

User yêu cầu:

"Tôi muốn đi Đà Lạt 3 ngày với 5 triệu."

### Failure

AI sinh lịch trình có tổng chi phí thực tế vượt xa ngân sách.

### Impact

Người dùng mất niềm tin vào hệ thống.

### Mitigation

* Hiển thị estimated budget
* Cho phép regenerate
* Cho phép user chỉnh ràng buộc

### Owner

[Tên thành viên]

---

## 8. Owner Plan Day 06

| Thành viên | Việc phụ trách     | Deliverable  |
| ------------ | --------------------- | ------------ |
| Member 1     | Research & Validation | Evidence     |
| Member 2     | SPEC & Documentation  | Thin SPEC    |
| Member 3     | Agent Workflow        | Flow Diagram |
| Member 4     | Agent Development     | Prototype    |
| Member 5     | Failure Testing       | Test Cases   |
| Member 6     | Demo & Pitch          | Demo Script  |
