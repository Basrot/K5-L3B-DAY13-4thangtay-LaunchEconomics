# Hồ sơ launch v0 · Trợ lý hoàn phí LogiX-VN · Gate 2a

Nhóm Strawberry · Lớp L3B · Pilot chỉ gồm `noi_dia` và `hang_nang`. Loại `quoc_te` vì chi phí mỗi việc thành công bằng **1,88×** định mức `[simulated]`. Hoãn `doi_tac` vì tỉ lệ thành công chỉ **54,4%** `[simulated]`. [Căn cứ A3](bang_chi_phi.md)

| Mục | Con số chính | Trạng thái | Người phụ trách |
| --- | --- | --- | --- |
| 1 · Chi phí mỗi việc thành công | Toàn mẫu **4.472 đ/việc** `[simulated]`. Phạm vi **4.599 đ/việc** `[simulated]` gồm cố định ở mức giả định 45.000 yêu cầu/tháng. | Giả lập | Kỹ sư trưởng agent |
| 2 · Ba yếu tố nhạy nhất | Kết quả độ nhạy `[simulated]`: tiền làm lại ×2 **+51,8%**, tiền xem lại ×2 **+40,7%**, lương +25% làm chi phí tăng **23,1%**. | Giả lập | Kỹ sư trưởng agent |
| 3 · So với nhân viên tự làm | Cả hệ thống **5.217 đ/yêu cầu** `[simulated]` trong phạm vi, gồm xử lý thủ công và cố định. Định mức làm tay của đề là **12.000 đ/yêu cầu**. | Giả lập | PM trợ lý hoàn phí |
| 4 · Chỉ số chính, chỉ số dùng, chỉ số an toàn | Trên **mẫu giả lập của lab**, **82,83%** `[simulated]` đóng ≤24 giờ và không mở lại 7 ngày, **27,12%** `[simulated]` sửa hoặc bỏ gợi ý, **4,25%** `[simulated]` mở lại trong 7 ngày. | Giả lập | Kỹ sư trưởng dữ liệu |
| 5 · Bảng lỗi và cách khắc phục | Hai bộ nhãn trùng **20/20 ca (100%)** và có năm biện pháp. Hai thành viên gắn nhãn độc lập trước khi đối chiếu. | Xong, có bằng chứng | Người phụ trách tổng hợp CP3 |
| 6 · Pilot plan | **20 nhân viên/nhánh**, thu **5.980 yêu cầu/nhánh** (859 hiệu dụng), theo dõi **7 ngày** sau khi đóng và có **3 luật dừng**. Ngưỡng chênh mở lại **2 điểm** áp dụng từ bước 10 người. Power **64%** nếu chênh 5 điểm. | Xong, có bằng chứng | Giám đốc vận hành |
| 7 · Rủi ro kinh tế | Xem lại 100% cho **12.850–13.559 đ/yêu cầu** `[simulated]` gồm thủ công và cố định (kịch bản làm lại 9–16,25 phút), cao hơn **12.000 đ/yêu cầu**. | Giả lập | Trưởng nhóm CSKH |

[Căn cứ tính](2A202603722_MaiXuanKhang.md#4-bằng-chứng) · [Bảng lỗi](bang_loi.md) · [Kế hoạch pilot](pilot_plan.yaml)

Để trở lại Gate 2a, Kỹ sư trưởng agent xác nhận xử lý hai ca 7 và 20. Kỹ sư trưởng dữ liệu kiểm tra các event có `trace_id`. Trưởng nhóm CSKH xác nhận phương án xem lại giữ chi phí hệ thống ≤ 12.000 đ/yêu cầu. Giám đốc vận hành xác nhận đủ nhân viên, lịch thu mẫu và thời gian theo dõi.

**Đề xuất:** No-go
