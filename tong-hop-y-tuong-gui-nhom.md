# Tổng hợp ý tưởng — Cuộc thi Khởi Nguyên 2026, Vòng 2
*Cập nhật để nhóm nắm tiến độ phát triển ý tưởng (chưa chốt cuối cùng)*

---

## 1. Nỗi đau xuất phát điểm

Sinh viên/người mới đi làm chưa có kinh nghiệm thường ghi vào CV những cụm từ chung chung như "nhiệt tình", "chủ động", "kỹ năng làm việc nhóm tốt" — đây là lời **tự nhận, không có bằng chứng cụ thể**. Nhà tuyển dụng không có cách nào kiểm chứng, dẫn đến CV của nhóm sinh viên chưa có kinh nghiệm mất giá trị thuyết phục.

→ Đây là vấn đề **bất cân xứng thông tin**: end-user (sinh viên) cần cách chứng minh kỹ năng mềm bằng bằng chứng cụ thể; buyer tiềm năng (nhà tuyển dụng/doanh nghiệp) cần cách lọc ứng viên đáng tin mà không tốn thời gian.

## 2. Đối tượng mục tiêu

- **End-user:** Sinh viên chưa có kinh nghiệm làm việc (chưa có "quá trình" để tự chứng minh)
- **Buyer (đang nghiêng về):** Doanh nghiệp/nhà tuyển dụng — cần công cụ sàng lọc ứng viên thực tập/entry-level đáng tin cậy hơn CV tự khai

*(Mô hình trường ĐH mua/tích hợp — đã cân nhắc nhưng đang không ưu tiên, vì dễ trùng với hướng ý tưởng cũ đã bị loại)*

## 3. Nguyên tắc thiết kế cốt lõi đã thống nhất

**Không làm sản phẩm "dạy" kỹ năng mềm (kiểu gia sư AI/Duolingo/ELSA Speak).** Lý do: kỹ năng mềm nên để con người dạy (giảng viên, mentor, chương trình đào tạo hiện có của trường); AI dạy thay dễ bị đánh giá là thiếu tính thực tế và giẫm chân người dạy thật.

**Mô hình tham chiếu ưa thích: "LeetCode, không phải Duolingo"** — tức là sản phẩm nên là một **sân chơi thực hành + minh chứng**, không phải nền tảng dạy từng bước.

**Băn khoăn hiện tại (quan trọng, đang giải quyết):** Ngay cả phương án "AI chấm theo rubric + xuất minh chứng có trích dẫn" (giống band descriptor IELTS) — dù đã cố tách vai trò "giám khảo" khỏi "gia sư" — người dùng vẫn cảm thấy còn dây dưa hình bóng "AI dạy con người cách làm điều gì đó". Đây là điểm mấu chốt cần nhóm cùng bàn kỹ trước khi chốt.

## 4. 10 hướng mô hình đang được cân nhắc

Đã liệt kê 10 biến thể, phân loại theo **vai trò AI đóng** (tạo ra đánh giá mới, hay chỉ là hạ tầng phục vụ con người vốn đã đánh giá):

| # | Tên gọi tạm | Cơ chế lõi | AI làm gì | Con người làm gì |
|---|---|---|---|---|
| 1 | Hồ Sơ Minh Chứng Số | Tổng hợp minh chứng có sẵn từ hoạt động thật (CLB, đồ án, tình nguyện) | Trích xuất & trình bày dữ liệu đã có | Tự tạo minh chứng từ hoạt động thật |
| 2 | Đánh Giá Chéo Có Cấu Trúc | SV đánh giá lẫn nhau sau dự án nhóm thật, theo tiêu chí chuẩn hoá | Tổng hợp điểm, phát hiện thiên vị | SV là người chấm |
| 3 | Nhật Ký Sự Kiện Kỹ Năng | SV tự ghi sự kiện thể hiện kỹ năng, có người liên quan xác nhận | Sổ ghi + xác thực | Người xác nhận là người thật |
| 4 | Sàn Thử Thách Từ Doanh Nghiệp | DN đăng bài toán thật, SV làm, chính DN chấm | Hạ tầng đăng bài + nộp bài | DN tự chấm |
| 5 | Sổ Tay Số Hoá Cho Mentor | Số hoá việc mentor đang chấm bằng miệng/giấy | Template ghi chấm nhanh | Mentor vẫn chấm |
| 6 | Xác Thực Chứng Chỉ Liên Trường | Chuẩn hoá chứng chỉ rời rạc giữa các trường | Đối chiếu, chuẩn hoá | Trường tự cấp như cũ |
| 7 | Nhật Ký Tự Phản Ánh Có Khung Dẫn | SV viết lại trải nghiệm theo khung câu hỏi chuẩn (kiểu STAR) | Đưa khung câu hỏi | SV tự kể trải nghiệm |
| 8 | Pool Giám Khảo Con Người Từ Xa | Chuyên gia/HR/SV năm cuối chấm bài từ xa qua nền tảng | Ghép cặp, logistics | Người thật chấm 100% |
| 9 | Điểm Tín Nhiệm Từ Dữ Liệu Có Sẵn | Gộp dữ liệu rời rạc đã có (điểm CLB, thực tập, khoá học) | Tổng hợp, chuẩn hoá | Các đơn vị gốc đã tự đánh giá |
| 10 | Công Cụ Hỗ Trợ Lớp Học Đảo Ngược | GV dạy trực tiếp, nền tảng cấp kịch bản luyện + ghi lại | Ngân hàng tình huống + công cụ ghi | GV chấm 100% |

**Ba hướng né sạch nhất việc "AI đóng vai người dạy/phán xét":** #2, #4, #8 — vì người chấm luôn là con người thật, AI chỉ làm hạ tầng.
- #2: rẻ/nhanh nhất để làm MVP
- #4: gắn chặt nhất với hướng buyer là doanh nghiệp
- #8: chuyên nghiệp nhất nhưng khó vận hành nhất trong thời gian ngắn

## 5. Nghiên cứu thị trường có thể làm ngay (đề xuất cho phần QTKD)

- Đếm tần suất cụm từ mơ hồ ("năng động", "chủ động"...) trong mẫu CV/tin tuyển dụng thực tập sinh trên TopCV
- Khảo sát nhanh vài HR/nhà tuyển dụng: có tin các dòng tự nhận kỹ năng mềm trong CV không?
- Khảo sát sinh viên đã có chứng chỉ kỹ năng mềm ở trường: quy trình đánh giá hiện tại là gì, có thực chất không (đang có bộ câu hỏi mini IDI sẵn để đi hỏi)

## 6. Chưa chốt — cần nhóm cùng quyết định

1. Chọn 1 trong 10 hướng (hoặc biến thể mới) làm hướng chính để đào sâu
2. Mô hình buyer cuối cùng (nghiêng B2B nhưng chưa chốt hẳn)
3. Cách giải quyết dứt điểm băn khoăn "AI dạy hay không dạy" — đặc biệt nếu chọn hướng #2/#4/#8 thì băn khoăn này gần như được giải quyết tự nhiên vì AI không chấm

**Deadline nộp bài: 12h00 ngày 08/07/2026** — còn khoảng 5 ngày, cần chốt hướng chính trong 1-2 ngày tới để còn thời gian làm slide + mockup UX/UI.
