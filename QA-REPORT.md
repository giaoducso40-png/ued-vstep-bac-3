# Báo cáo rà soát trước khi đóng gói

## Vòng 1 – Cấu trúc và nội dung VSTEP

Đã đối chiếu số phần và mục tiêu bậc 3. Ngân hàng tích hợp gồm 40 câu Đọc thuộc 4 phần, 35 câu Nghe thuộc 3 phần, 12 đề Viết và 18 bộ Nói. Bộ kiểm tra xác nhận 75 ID trắc nghiệm là duy nhất, đáp án đều nằm trong bốn lựa chọn và mỗi câu đều có giải thích/bằng chứng.

## Vòng 2 – UX/UI và khả năng truy cập

Đã rà CSS mobile-first, kích thước vùng bấm, font hệ thống, safe-area, điều hướng dưới, focus-visible, tương phản cao và reduced-motion. Bố cục chuyển về một cột trên màn hình nhỏ; thanh số câu chỉ cuộn ngang và không khóa cuộn dọc của trang. Khối giải thích được mở theo từng câu, có khoảng an toàn với thanh điều hướng dưới và tự cuộn vào vùng nhìn. Cần kiểm tra lại bằng thiết bị thật sau khi GitHub Pages cấp URL công khai, đặc biệt quyền micro trên Safari iOS.

## Vòng 3 – Mã nguồn và triển khai

Đã chạy ESLint, kiểm tra TypeScript, production build, kiểm định dữ liệu và bộ kiểm tra đường dẫn. Bản dựng dùng tài nguyên tương đối, không có backend, Service Worker hay API key. Đã phục vụ thử bằng HTTP tĩnh và nhận thành công HTML, CSS, JavaScript cùng trang 404; sau đó tiếp tục giải nén ZIP và kiểm tra lại từ chính gói phát hành.

## Vòng 4 – An toàn và thông báo

Đã rà lời tuyên bố: kết quả chỉ mang tính tham khảo, không phải chứng chỉ hoặc hệ thống chính thức. Bản ghi âm không tự tải lên máy chủ; tiến độ và bản nháp chỉ lưu trên trình duyệt. Nội dung mẫu là nội dung tự biên soạn và không gắn nhãn đề thi thật.

## Giới hạn đã ghi nhận

- Âm thanh dùng SpeechSynthesis và tự ưu tiên giọng English Natural/Neural/Enhanced do thiết bị cung cấp; người học có thể chọn giọng và tốc độ. Chất lượng thực tế phụ thuộc hệ điều hành/trình duyệt và không được coi là audio phòng thu hay audio đề thi thật.
- Dữ liệu lưu theo từng trình duyệt, không đồng bộ giữa thiết bị.
- Bài chẩn đoán và thi thử là bản rút gọn, không quy đổi trực tiếp sang chứng chỉ bậc 3.
