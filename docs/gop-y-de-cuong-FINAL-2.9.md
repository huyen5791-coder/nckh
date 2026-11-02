# Góp ý mô hình – Đề cương FINAL 2.9 (02/09/2026)

Bản đề cương này thay thế bản nháp `mo-hinh-nghien-cuu-CE-GI-GG.md`. Các góp ý dưới đây chỉ xét **mô hình và thiết kế kiểm định**, không sửa văn phong.

## A. Lỗi logic cần sửa (ảnh hưởng tới kết quả kiểm định)

### A1. H7, H8 không kiểm định được vì thiếu đường NLXT → TTX
- H7 (KTTH → NLXT → TTX) và H8 (ĐMCN → NLXT → TTX) cần có đường NLXT → TTX. Hình 1 và Bảng 2 không có đường này.
- Đoạn diễn giải sau H10 ("nếu chỉ H7, H8 có ý nghĩa, NLXT tác động trực tiếp đến kết quả") cũng cần đường này.
- **Sửa:** thêm đường NLXT → TTX. Không cần đặt thành giả thuyết riêng, có thể ghi là "đường cấu trúc cần cho kiểm định H7–H8".

### A2. Mô hình trung gian nối tiếp đang ép trung gian toàn phần
- Mô hình chuẩn (Hayes Model 6) có đủ các đường X → M2, tức KTTH → HQST và ĐMCN → HQST.
- Thiếu hai đường này thì mọi tác động lên HQST bị ép đi qua NLXT. Như vậy hệ số H5 bị thổi phồng và H9, H10 dễ "có ý nghĩa" một cách giả tạo.
- **Sửa:** đưa KTTH → HQST và ĐMCN → HQST vào ước lượng làm đường kiểm soát, không cần đặt giả thuyết.

### A3. Biến phụ thuộc chồng lấn với biến độc lập và biến trung gian
- TTX có chiều **"đổi mới sáng tạo xanh"**, trùng gần như hoàn toàn với ĐMCN xanh. Hệ quả: H2 mang tính đồng nghĩa lặp (ĐMCN → một tổ hợp có chứa ĐMCN), và HTMT nhiều khả năng vượt 0,85.
- Chiều **"môi trường"** của TTX dễ trùng với HQST. Hệ quả: H6 bị thổi phồng.
- **Sửa (khuyến nghị):**
  - Bỏ chiều "đổi mới sáng tạo xanh" khỏi TTX.
  - Định nghĩa chiều môi trường ở mức **kết quả** (phát thải, chất thải, tuân thủ đầu ra). Định nghĩa HQST ở mức **hiệu suất quy trình** (đầu ra/đầu vào). Ghi rõ ranh giới này trong Bảng 1.
- TTX còn 3 chiều: kinh tế xanh, môi trường, xuất khẩu xanh.

### A4. Đặt điều tiết trên đường trực tiếp mâu thuẫn với lập luận "phần lớn tác động đi qua kênh gián tiếp"
- H1 tự dự báo tác động trực tiếp nhỏ. H11 và H12 lại đều điều tiết đúng đường trực tiếp đó. Nếu trung gian là toàn phần thì đường được điều tiết xấp xỉ 0, và H11–H13 khó có ý nghĩa thống kê.
- Theo lý thuyết tín hiệu (mục 4.1.4), áp lực thị trường quyết định việc nỗ lực xanh **có được thị trường định giá hay không**. Đó là giai đoạn cuối của chuỗi (HQST → TTX, hoặc NLXT → TTX).
- **Sửa (khuyến nghị):** chuyển ÁPXQT sang điều tiết giai đoạn hai (HQST → TTX) và báo cáo **chỉ số trung gian có điều tiết** (index of moderated mediation, Hayes 2015). CSXTN có thể giữ ở giai đoạn một (KTTH/ĐMCN → NLXT), đúng với cơ chế tuân thủ ép doanh nghiệp xây dựng năng lực.
- Cách đặt này cũng làm H13 dễ lập luận hơn: hai loại áp lực khác nhau không chỉ về cường độ mà còn về **vị trí** tác động trong chuỗi.

### A5. Thang đo CSXTN trộn "áp lực" với "hỗ trợ", làm suy yếu chính đóng góp lý luận thứ nhất
- Định nghĩa CSXTN gồm cả yêu cầu tuân thủ lẫn hỗ trợ kỹ thuật, tín dụng xanh và ưu đãi tài chính. Hỗ trợ và tín dụng là cơ chế **nguồn lực/khuyến khích**, không phải cơ chế tuân thủ.
- Nếu CSXTN điều tiết dương thì không biết phần đó đến từ áp lực hay từ hỗ trợ. Như vậy luận điểm "tách hai cơ chế" bị nhiễu ngay trong thang đo.
- **Sửa:** CSXTN chỉ đo áp lực tuân thủ. Phần "tiếp cận hỗ trợ/tín dụng xanh" chuyển thành biến kiểm soát. Nếu cần, có thể tách thành biến riêng, nhưng làm vậy mô hình sẽ thêm phức tạp.

### A6. H13 cần thiết kế kiểm định rõ ràng
- Cả hai biến điều tiết phải nằm **đồng thời** trong cùng một mô hình. Trong khi đó bước 6 ghi là "kiểm định từng biến điều tiết độc lập", mâu thuẫn với yêu cầu này.
- So sánh hai hệ số tương tác đã chuẩn hóa bằng khoảng tin cậy bootstrap của hiệu số (β_ÁPXQT − β_CSXTN).
- Hai thang đo phải có cùng số bậc Likert và cùng mức độ cụ thể của item, nếu không thì so sánh cường độ sẽ thiếu công bằng.

## B. Phương pháp
1. **Bước 6:** "product indicator approach trong PLS-MGA" đang trộn hai kỹ thuật khác nhau. Khi có cấu trúc bậc hai kết hợp hoặc thang đo kết hợp, Hair và cộng sự khuyến nghị dùng **two-stage approach** cho biến tương tác. MGA là kỹ thuật riêng, chỉ dùng cho bước 8 (so sánh theo nhóm ngành hàng).
2. **Bước 5:** ghi "trực tiếp H1–H4, trung gian H5–H10", nhưng H5 và H6 là quan hệ trực tiếp. Đúng ra là trực tiếp H1–H6, trung gian H7–H10.
3. **Nội sinh:** dữ liệu cắt ngang nên có khả năng nhân quả ngược (doanh nghiệp tăng trưởng tốt mới có tiền đầu tư xanh). Nên bổ sung **Gaussian copula** (có sẵn trong SmartPLS 4) vào phần kiểm tra độ bền.
4. **CMB:** ULMC hiện bị phê phán nhiều. Nên dùng thêm **full collinearity VIF** (Kock, 2015) và một biến đánh dấu (marker variable). Việc dùng item bán khách quan cho chiều kinh tế và xuất khẩu xanh là điểm tốt, nên giữ.
5. **Số biến tương tác:** tổng cộng 5 biến tương tác (4 điều tiết + H14). Với N từ 300 trở lên thì vẫn chạy được, nhưng cần báo cáo f² và simple slope cho từng biến.

## C. Nhất quán nội bộ
- Mục 2.6 (chi phí giao dịch xanh) là lập luận hay nhưng chưa có biến nào trong mô hình tương ứng. Đề xuất đưa **"mức độ liên kết vùng nguyên liệu"** (tỷ lệ nguyên liệu qua hợp đồng liên kết hoặc có mã vùng trồng) vào làm biến kiểm soát. Nếu muốn khai thác sâu hơn, có thể đặt nó làm biến điều tiết H1 trong phân tích bổ sung.
- Hình 1: nhãn "H3" đang nằm cạnh đường ĐMCN → TTX, còn đường cong KTTH → NLXT không có nhãn. Cần sửa lại cho khớp với Bảng 2.
- Mục 3.2 ghi đối tượng nghiên cứu có "cảm nhận hiệu quả sinh thái", nhưng Bảng 1 lại gọi là "hiệu quả sinh thái". Nên thống nhất một tên gọi.
- Mục 5.4 có lỗi đánh máy: "300–504.20 phiếu".
- Mục 1.3 và 2.4 trích Wang và cộng sự (2019) với kết luận "dương dưới ngưỡng, âm trên ngưỡng", trong khi bản thảo "TTX – TMQT" trích một nghiên cứu về Vành đai Dương Tử với kết luận ngược lại (âm, rồi dương sau ngưỡng). Đây là hai bài khác nhau, nhưng nên trích cả hai để cho thấy chính sự ngược chiều này. Làm vậy sẽ củng cố khoảng trống thứ nhất.

## D. Tài liệu tham khảo cần đối chiếu lại số tập/trang
- Lanoie, Patry & Lajeunesse (2008), *Journal of Productivity Analysis*: theo hiểu biết của tôi là tập 30(2), tr. 121–128, không phải 36(3), tr. 301–317.
- Zhang, Rong & Ji (2019), *Resources, Conservation and Recycling*: tập 128 là năm 2018. Bài năm 2019 có thể thuộc tập 144. Cần kiểm tra lại.
- Yao, Liu & Sheng (2019), *Journal of Business Research*: tập 128 là năm 2021. Cần kiểm tra lại năm hoặc tập.
- Mol & Sonnenfeld (2000) và Teece (2018) có trong danh mục tài liệu nhưng không được trích trong bài.

## E. Mô hình sau khi chỉnh (đề xuất)
```
                    CSXTN (tuân thủ)                       ÁPXQT (thị trường)
                        |  điều tiết giai đoạn 1               |  điều tiết giai đoạn 2
                        v                                      v
 KTTH ──H3──►  NLXT ──H5──►  HQST ─────────H6──────────────────────► TTX (3 chiều:
 ĐMCN ──H4──►   │                                                     kinh tế xanh,
   │            └──────── NLXT → TTX (đường cần thêm cho H7, H8) ────►  môi trường,
   │                                                                    xuất khẩu xanh)
   ├── H1, H2: đường trực tiếp tới TTX
   ├── KTTH/ĐMCN → HQST: đường kiểm soát
   └── H14: KTTH × ĐMCN → TTX
 Kiểm soát: quy mô, tuổi, ngành hàng, tỷ lệ XK/DT, thị trường chính, liên kết vùng nguyên liệu, tiếp cận hỗ trợ/tín dụng xanh
```
