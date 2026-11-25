# Báo cáo nhóm Strawberry · Lab 13

## 1. Thông tin nhóm

- **Nhóm Strawberry, lớp L3B.**
- **Nhóm trưởng** là Hồ Trọng Nghĩa. Nhóm có bốn thành viên, gồm Nghĩa, Mai Xuân Khang, Lương Thị Hồng Hạnh và Phạm Đăng Quang. [Danh sách và phân công](../../TEAM.md)

## 2. Mục tiêu và cách tiếp cận

Nhóm xây dựng hồ sơ Gate 2a để quyết định có nên thử nghiệm trợ lý hoàn phí LogiX-VN trong một pilot có đối chứng hay không. Đánh giá dựa trên chi phí cả hệ thống, mức độ sử dụng, lỗi và khả năng đo tác động. Dữ liệu giả lập đã được đối chiếu gồm **1.200 yêu cầu và 1.624 lượt chạy** từ 6 depot, với 20 mã nhân viên trong mẫu. [Dữ liệu yêu cầu](../../src/logix_requests.csv) · [Dữ liệu lượt chạy](../../src/logix_runs.csv)

## 3. Giải pháp

| Nhiệm vụ | Cách thực hiện và bằng chứng |
| --- | --- |
| A · Mô hình chi phí | Qua ba phép thử A1 rồi cộng chi phí của mọi lượt chạy và thời gian nhân viên. Tính chi phí trên mỗi việc thành công theo từng loại yêu cầu và xét chi phí cố định trong phạm vi pilot. [Mã tính](../../src/lab13.py) · [Bảng chi phí](bang_chi_phi.md) |
| B · Độ nhạy | Thay đổi từng yếu tố, xếp hạng ba yếu tố ảnh hưởng nhất, so giới hạn 1–3 lượt chạy và đo tác động của việc xem lại 100%. Dùng chi phí cả hệ thống để so với mức 12.000 đ cho một yêu cầu do nhân viên tự xử lý. [Bảng chi phí](bang_chi_phi.md) |
| C · Bảng lỗi | Hai thành viên gắn nhãn độc lập 20 ca rồi mới đối chiếu. Nhóm giữ lại hai bộ nhãn gốc và đề xuất cách phát hiện, khắc phục cùng người phụ trách cho một ca ở mỗi loại lỗi. [Bảng lỗi](bang_loi.md) |
| D · Thiết kế pilot | Tính cỡ mẫu hiệu dụng cho ba đơn vị phân nhóm. Chọn cách chia dựa trên cỡ mẫu và nguy cơ ảnh hưởng giữa các nhánh, rồi xác định ngưỡng chi phí, an toàn và mức sử dụng để dừng pilot. [Kế hoạch pilot](pilot_plan.yaml) |
| E · Chỉ số và hồ sơ | Tính ba chỉ số trên dữ liệu chạy thử, đề xuất thêm chỉ số sử dụng và an toàn, đặc tả event có `trace_id`, đưa rủi ro từ bảng độ nhạy vào hồ sơ một trang. [Chỉ số và rủi ro](chi_so.md) · [Hồ sơ launch v0](ho_so_launch_v0.md) |

## 4. Kết quả

Các kết quả A–E và đề xuất Gate 2a đang chờ nhóm thực hiện và kiểm tra. Khi chốt bài, mục này ghi chi phí mỗi việc thành công, chi phí toàn hệ thống trên mỗi yêu cầu, kết quả ba chỉ số, đồng thuận gắn nhãn, cỡ mẫu đã chọn và lý do của đề xuất cuối. Số tính từ hai cột thời lượng giả lập ghi nhãn `simulated`.

Nhận xét và điểm của hội đồng dành cho Strawberry được cập nhật sau buổi duyệt chéo. Phiếu trong repo ghi phần Strawberry chấm nhóm được giao. [Hồ sơ launch v0](ho_so_launch_v0.md) · [Phiếu chấm](phieu_cham.md)

## 5. Khó khăn và cách xử lý

Một điểm cần kiểm tra là giới hạn chạy lại có thể làm giảm chi phí của trợ lý nhưng làm tăng số yêu cầu chuyển cho nhân viên. Nhóm sẽ đối chiếu đồng thời chi phí mỗi việc thành công, số ca chuyển và chi phí toàn hệ thống ở từng giới hạn. Khi chọn đơn vị phân nhóm, nhóm sẽ kiểm tra cỡ mẫu hiệu dụng và ghi rõ đánh đổi nếu số cụm không đáp ứng mục tiêu phát hiện chênh lệch.

## 6. Tổng hợp đóng góp

Nghĩa phụ trách code A–B trước giờ giải lao, chỉ số và rủi ro kinh tế, đồng thời tổng hợp báo cáo. Quang đối chiếu số và tiếp quản code cho D1 và E1. Hạnh và Khang gắn nhãn độc lập ở CP3. Hạnh tổng hợp bảng lỗi và viết kế hoạch pilot, còn Khang tổng hợp hồ sơ launch và ghi phiếu chấm. Bằng chứng đóng góp được cập nhật theo kết quả từng checkpoint. [Chi tiết phân công](../../TEAM.md)

## 7. Hạn chế và hướng cải thiện

Dữ liệu chạy thử là giả lập và thiếu nhóm đối chứng, nên các chỉ số hiện có chỉ mô tả mẫu. Trong pilot, nhóm dự kiến đo lại thời gian xem xét và làm lại bằng event thực tế, theo dõi nguy cơ nhân viên chia sẻ gợi ý giữa các nhánh và báo cáo kết quả theo phạm vi yêu cầu đã chọn.

## 8. Tài liệu tham khảo

- [Đề Lab 13 và 20 ca lỗi](../../docs/Ngay13_Lab13_De_bai_hoc_vien.docx)
- [Dữ liệu, giả định và công thức của lab](../../docs/du_lieu_va_cong_thuc.md)
- [Checkpoint và tiêu chí chấm](../../CHECKPOINTS.md) · [Rubric](../../RUBRIC.md)
