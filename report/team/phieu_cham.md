# Phiếu chấm hội đồng Gate 2a

Nhóm số n chấm nhóm số n + 1. Nhóm cuối chấm nhóm 1. Điểm dựa trên bằng chứng trong hồ sơ đội trình.

- Nhóm chấm (hội đồng): Strawberry (L3B).
- Nhóm được chấm: 4thangtay (L3B).
- Hồ sơ dùng để chấm: [Launch v0 tại commit `00df789e1fbc67da243eace57d557a17a1ff0eab`](https://github.com/Basrot/K5-L3B-DAY13-4thangtay-LaunchEconomics/blob/00df789e1fbc67da243eace57d557a17a1ff0eab/report/team/ho_so_launch_v0.md).

| Tiêu chí | 0 điểm | 5 điểm | 10 điểm | Điểm | Lý do (có số) |
| --- | --- | --- | --- | ---: | --- |
| Đề xuất khớp bằng chứng | Mâu thuẫn với số của chính nhóm | Khớp nhưng bỏ qua một con số bất lợi | Khớp, nêu cả con số bất lợi và cách xử lý | **10** | Go có điều kiện thừa nhận kịch bản xem lại 100% làm chi phí cả hệ thống **12.850–13.466 đ/yêu cầu**, cao hơn mốc **12.000 đ** `[simulated]`. Nhóm đặt điều kiện tỉ lệ sửa hoặc bỏ dưới **15% trong một tuần**, đạt ngưỡng an toàn và dự báo toàn hệ thống ≤12.000 đ/yêu cầu trước khi giảm xem lại. [Hồ sơ launch](https://github.com/Basrot/K5-L3B-DAY13-4thangtay-LaunchEconomics/blob/00df789e1fbc67da243eace57d557a17a1ff0eab/report/team/ho_so_launch_v0.md) · [B4](https://github.com/Basrot/K5-L3B-DAY13-4thangtay-LaunchEconomics/blob/00df789e1fbc67da243eace57d557a17a1ff0eab/report/team/bang_chi_phi.md) |
| Số giả lập và phạm vi | Thiếu nhãn và áp dụng cho mọi yêu cầu | Có nhãn hoặc phạm vi thu hẹp | Đủ nhãn và phạm vi thu hẹp có lý do bằng số | **10** | Bản cập nhật gắn `[simulated]` cho ba chỉ số E1 tại mục 4, các lần dẫn lại trong `chi_so.md` và phần bàn giao E1 của `bang_chi_phi.md`. Pilot giới hạn ở `noi_dia` và `hang_nang`, loại `quoc_te` do 1,88× định mức và hoãn `doi_tac` do tỉ lệ thành công 54,4%. [Hồ sơ launch](https://github.com/Basrot/K5-L3B-DAY13-4thangtay-LaunchEconomics/blob/00df789e1fbc67da243eace57d557a17a1ff0eab/report/team/ho_so_launch_v0.md) · [Đặc tả chỉ số](https://github.com/Basrot/K5-L3B-DAY13-4thangtay-LaunchEconomics/blob/00df789e1fbc67da243eace57d557a17a1ff0eab/report/team/chi_so.md) · [Bảng chi phí](https://github.com/Basrot/K5-L3B-DAY13-4thangtay-LaunchEconomics/blob/00df789e1fbc67da243eace57d557a17a1ff0eab/report/team/bang_chi_phi.md) |
| Pilot ra được quyết định | Không đối chứng hoặc thiếu cỡ mẫu | Đủ cỡ mẫu, luật dừng chung chung | Tách được tác động, đủ mẫu, luật dừng có ngưỡng, thời hạn, người có quyền dừng | **10** | Chia ngẫu nhiên có đối chứng theo nhân viên, **20 + 20**, cần **5.980 yêu cầu/nhánh** (859 hiệu dụng) và đủ 7 ngày theo dõi. Luật dừng nêu ngưỡng an toàn, chi phí và mức dùng; cổng rollout giao Giám đốc vận hành giữ nguyên bước nếu thiếu dữ liệu hoặc dự báo vượt 12.000 đ/yêu cầu. [Kế hoạch pilot](https://github.com/Basrot/K5-L3B-DAY13-4thangtay-LaunchEconomics/blob/00df789e1fbc67da243eace57d557a17a1ff0eab/report/team/pilot_plan.yaml) |
| **Tổng** | | | | **30/30** | |

**Quyết định của hội đồng:** Go có điều kiện.

**Lý do:** Bản cập nhật đã gắn nhãn giả lập tại các lần xuất hiện của E1 và nêu điều kiện không tăng bước khi dự báo chi phí toàn hệ thống vượt định mức. Go có điều kiện phù hợp với bằng chứng chi phí vượt ngưỡng ở kịch bản xem lại 100% và các điều kiện an toàn cần đạt trước khi mở rộng.

**Một câu hỏi cho đội trình:** Ở bước bốn người với 100% gợi ý được xem lại, chi phí cả hệ thống tính theo **đồng/yêu cầu** là bao nhiêu sau khi cộng phần nhân viên xử lý thay và ghi rõ cách phân bổ 40 triệu đ/tháng? Từ phép tính đó, nhóm đặt giới hạn thời gian xem lại bao nhiêu phút/ca để giữ chi phí ở mức 12.000 đ/yêu cầu?

**Câu trả lời của đội trình (phản hồi bằng văn bản trong bản cập nhật):** Theo mốc 45.000 yêu cầu/tháng toàn hệ thống và cách phân bổ A4, xem lại 100% cho **12.850 đ/yêu cầu** nếu làm lại 9 phút/ca và **13.466 đ/yêu cầu** nếu làm lại 15,3 phút/ca `[simulated]`. Chi phí gồm nhân viên xử lý thay 82 yêu cầu và khoảng **1.066.667 đ** cố định phân bổ cho 900 việc thành công `[simulated]`. Giới hạn xem lại tương ứng là **4,56** và **4,24 phút/ca** `[simulated]`. [Phân tích B4](https://github.com/Basrot/K5-L3B-DAY13-4thangtay-LaunchEconomics/blob/00df789e1fbc67da243eace57d557a17a1ff0eab/report/team/bang_chi_phi.md)
