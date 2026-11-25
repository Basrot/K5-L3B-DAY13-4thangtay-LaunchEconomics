# Hồ sơ launch v0 · Trợ lý hoàn phí LogiX-VN · Gate 2a

Một trang. Cột trạng thái chỉ nhận: **Xong, có bằng chứng · Chưa · Giả lập**. Mục nào dựa trên cột `_simulated` ghi Giả lập. Người phụ trách là một vai trò, không ghi "cả đội". Gate 2a chỉ duyệt kế hoạch pilot: không viết như thể trợ lý đã được duyệt chạy chính thức (xem quy tắc 5 trong `README.md`). Tuyệt đối không dùng thuật ngữ chạy chính thức ngoài đời thực.

Nhóm: 4thangtay · Lớp: L3B

| Mục | Con số chính | Trạng thái | Người phụ trách |
| --- | --- | --- | --- |
| 1 · Chi phí mỗi việc thành công | 4.472 đ [simulated] (toàn mẫu); 2.696 đ [sim] (nội địa); 8.221 đ [sim] (hàng nặng); gồm cố định: 4.599 đ [sim] (0,38×) | Giả lập | Kỹ sư trưởng mô hình chi phí |
| 2 · Ba yếu tố nhạy nhất | 1. Làm lại (+51,8%, lên 6.787 đ); 2. Xem lại (+40,7%, lên 6.292 đ); 3. Lương (+23,1%, lên 5.506 đ) [simulated] | Giả lập | Chuyên viên phân tích độ nhạy |
| 3 · So với nhân viên tự làm | 0,38× ở 45.000 yc/tháng và 0,48× ở nửa khối lượng (phạm vi noi_dia + hang_nang) so với mốc 12.000 đ [simulated] | Giả lập | Chuyên viên phân tích độ nhạy |
| 4 · Chỉ số chính, chỉ số dùng, chỉ số an toàn | Chính: 82,83% (994/1.200); Dùng: 27,12% (48/177); An toàn: 4,25% toàn mẫu (3,97% trong phạm vi) [đợt chạy thử, chưa đối chứng] | Xong, có bằng chứng | Kỹ sư đo lường và chất lượng |
| 5 · Bảng lỗi và cách khắc phục | 20 ca gắn nhãn (đồng thuận 100%, 20/20), 5 ca khắc phục đo bằng event | Xong, có bằng chứng | Trưởng nhóm kiểm soát chất lượng |
| 6 · Pilot plan | 20 nhân viên/nhóm (40 cụm), MDE 6 điểm (859 yc/nhóm, m ≥ 299), 3 luật dừng NẾU-TRONG-THÌ-KHÔNG THÌ | Xong, có bằng chứng | Giám đốc vận hành LogiX-VN |
| 7 · Rủi ro kinh tế | Làm lại gấp đôi (+51,8%, lên 6.787 đ); Xem lại 100% kéo dài (0,98×–1,03× baseline 12.000 đ); Khối lượng giảm 50% (+2.370 đ/yc) [simulated] | Giả lập | PM trợ lý hoàn phí |

**Đề xuất:** Go có điều kiện

**Điều kiện cụ thể:**
- Chỉ triển khai pilot trong phạm vi hẹp gồm `noi_dia` và `hang_nang`; loại trừ `quoc_te` và `doi_tac`.
- Giám đốc vận hành kích hoạt luật dừng an toàn: ngắt trợ lý trong 30 phút nếu tỉ lệ mở lại cao hơn đối chứng ≥ 2 điểm hoặc vượt trần 6%; đồng thời dừng rollout khi có ít nhất 1 ca hoàn trùng trong 3 ngày liên tiếp.
- Giữ mức xem lại 100% trong bước rollout 0.10 và chỉ giảm xem lại khi tỉ lệ sửa/bỏ < 15%.
- Người phụ trách kiểm tra: Giám đốc vận hành LogiX-VN & PM trợ lý hoàn phí. Ngày kiểm tra mốc tiếp theo: 2027-01-05.
