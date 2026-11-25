# Báo cáo cá nhân — DaoNgocHan-2A202603779

## 1. Thông tin thành viên

- Họ tên: Đào Ngọc Hân
- MSSV: 2A202603779
- Email: daongochan1505@gmail.com
- Vai trong nhóm: Người gắn nhãn 1 (Người 3)

## 2. Phần việc phụ trách

- Theo dõi điều kiện hoàn thành ("Xong khi") của từng checkpoint A–E.
- Nhiệm vụ C (`report/team/bang_loi.md`): gắn nhãn độc lập cả 20 ca lỗi theo 5 loại Google PAIR, tổng hợp hai bộ nhãn với Người 4, tính tỉ lệ đồng thuận, viết quy tắc phân biệt ranh giới và hoàn thiện bảng khắc phục 5 ca.
- Nhiệm vụ D2: kiểm tra 5 câu "tách được tác động" và các luật dừng trong `report/team/pilot_plan.yaml`.
- Nhiệm vụ E1–E2 (`report/team/chi_so.md`): đặc tả 5 chỉ số (3 chỉ số cho sẵn + 1 chỉ số dùng & 1 chỉ số an toàn tự đề xuất), liệt kê tối thiểu 6 event có `trace_id`, kiểm tra chéo ánh xạ event → chỉ số, và viết bảng rủi ro kinh tế E2 từ bảng độ nhạy B.
- Duyệt chéo Gate 2a và rà soát cuối buổi: phản biện phần lỗi và chỉ số; kiểm tra nhãn `simulated`, không dùng từ cấm, đủ file hồ sơ và đủ 4 báo cáo cá nhân trước khi nộp.

## 3. Đóng góp cụ thể

- Hoàn thiện Nhiệm vụ C trong `report/team/bang_loi.md`: gắn đủ 20 ca lỗi theo 5 loại Google PAIR dựa trên nguyên nhân gốc (phân bố 4/5/4/4/3), đối chiếu với Người 4 đạt đồng thuận **20/20 = 100%**, chốt 5 quy tắc phân biệt cho các ca dễ lẫn, và chuẩn hóa bảng khắc phục 5 ca có đủ event đo được, ngưỡng và tần suất đồng bộ 100% với `report/team/chi_so.md`.
- Hoàn thiện và đối chiếu chốt 100% Nhiệm vụ E1–E2 trong `report/team/chi_so.md`: khớp hoàn toàn 3 chỉ số E1 từ đầu ra `src/lab13.py` của Người 2 (`82,83%`, `27,12%`, `4,25%`; phạm vi pilot `3,97%`), đề xuất thêm 1 chỉ số Dùng và 1 chỉ số An toàn, thiết kế 11 event đều có `trace_id`, kiểm tra chéo 5/5 chỉ số đều đo được, và lập 3 dòng rủi ro kinh tế E2 lấy số từ bảng B1/B3/B4/A4 trong `report/team/bang_chi_phi.md` (đều gắn nhãn `simulated`).
- Rà soát chất lượng (QA) toàn bộ hồ sơ nhóm sau PR #2, #3, #4: xác nhận 5 câu D2, 3 luật dừng và cú pháp không còn dấu `?` trong `report/team/pilot_plan.yaml`; kiểm tra 0 từ cấm trong `report/team/` và `TEAM.md`; tổng hợp danh sách các điểm cần chỉnh trên `bang_chi_phi.md`, `ho_so_launch_v0.md`, `group_report.md`, `TEAM.md` và nhắc bổ sung báo cáo cá nhân Người 1.
- *(Tại buổi duyệt chéo 17:00–17:45)* Tham gia phản biện phần lỗi và chỉ số Gate 2a, soát đủ 4 báo cáo cá nhân trước khi chốt nộp.

## 4. Bằng chứng

- Nhánh làm việc: `2A202603779_DaoNgocHan` (đồng bộ `origin/main` tại commit `20a5efb`, tạo Pull Request vào `main`).
- File `report/team/bang_loi.md`: đủ 2 bộ nhãn 20 ca (đồng thuận 20/20 = 100%), 5 quy tắc phân biệt ranh giới, bảng khắc phục 5 ca đủ 5 loại có event/ngưỡng/tần suất và vai trò phụ trách.
- File `report/team/chi_so.md`: 5 chỉ số E1 (3 chỉ số tính thử khớp `src/lab13.py` + 2 chỉ số tự đề xuất), 11 event có `trace_id`, kiểm tra chéo 5/5 chỉ số đo được, 3 dòng rủi ro kinh tế E2 gắn nhãn `simulated`.
- File báo cáo cá nhân: `report/team/2A202603779_DaoNgocHan.md`.

## 5. Công cụ AI đã dùng

- **Công cụ:** Antigravity AI Assistant.
- **Mục đích:** Hỗ trợ đồng bộ nhánh Git và tạo PR; kiểm chứng phép tính từ `src/logix_requests.csv` và `src/logix_runs.csv` đối chiếu với `src/lab13.py` và `report/team/bang_chi_phi.md`; hỗ trợ phân tích nguyên nhân gốc 20 ca lỗi theo khung Google PAIR, chuẩn hóa bảng khắc phục 5 ca và danh sách 11 event có `trace_id`; rà soát nhãn `simulated`, dấu `?`, từ cấm và tính nhất quán giữa các file hồ sơ.
- **Cách tự kiểm tra:** Đọc và tự kiểm tra lại từng nhãn lỗi trên cả 20 ca trong `docs/Ngay13_Lab13_De_bai_hoc_vien.docx` theo đúng 5 định nghĩa nguyên nhân gốc Google PAIR để đảm bảo nắm rõ lập luận khi bảo vệ Gate 2a; đối chiếu từng con số E1 và E2 với `docs/du_lieu_va_cong_thuc.md`, `report/team/bang_chi_phi.md` và script kiểm chứng trên hai file CSV; kiểm tra chéo tất cả tên event giữa `chi_so.md`, `bang_loi.md` và `pilot_plan.yaml`.

## 6. Tự đánh giá

- Hoàn thành đầy đủ các sản phẩm đầu ra phụ trách của Người 3 (`bang_loi.md`, `chi_so.md`, `2A202603779_DaoNgocHan.md`) và rà soát chéo toàn bộ hồ sơ nhóm đúng tiến độ trước mốc 17:00 gửi hội đồng Gate 2a.
- Sau khi tạo PR, tiếp tục rà soát lại 20 nhãn lỗi, phối hợp nhóm hoàn tất các điểm QA nhỏ trên `bang_chi_phi.md` / `ho_so_launch_v0.md` / `TEAM.md`, tham gia duyệt chéo Gate 2a và nộp link repo cá nhân trên LMS trước 23:59 GMT+7.
