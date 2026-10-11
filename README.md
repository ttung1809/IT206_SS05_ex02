# BÀI 5: THIẾT KẾ QUY TRÌNH QUẢN LÝ AC – DoD – MoSCoW

Dự án: RikkeiGo – Ứng dụng đặt xe Vai trò: Lan – Scrum Master Mục tiêu: Xây dựng quy trình chuẩn để mọi Story mới được đánh giá, hoàn thiện và đưa vào Sprint dựa trên tiêu chí rõ ràng, không phụ thuộc vào ý kiến chủ quan của các bộ phận.

## Phần 1 – Thiết kế quy trình 5 bước

Bước 1. Tiếp nhận và ghi nhận Story

Chịu trách nhiệm: Product Owner (Đức), phối hợp với bên đề xuất.

* Ghi nhận nhu cầu, người dùng mục tiêu, giá trị mang lại và lý do cần thực hiện.

* Kiểm tra Story có trùng lặp hoặc nằm ngoài phạm vi sản phẩm không.

Điều kiện chuyển bước:

Story có nội dung rõ ràng và xác định được giá trị mong muốn.

Bước 2. Xây dựng Acceptance Criteria (AC)

Chịu trách nhiệm: Product Owner và Developers, trao đổi với bên đề xuất.

* Viết từ 3–7 AC theo cấu trúc Given – When – Then.

* AC phải cụ thể, kiểm thử được và thống nhất các trường hợp thành công, thất bại quan trọng.

Điều kiện chuyển bước:

Các bên hiểu thống nhất hành vi cần đạt và có thể kiểm thử từng AC.

Bước 3. Kiểm tra Definition of Done (DoD)

Chịu trách nhiệm: Developers; Scrum Master hỗ trợ đội hiểu và tuân thủ.

* Đối chiếu Story với DoD chung của đội, chẳng hạn: code hoàn thành, đã review, kiểm thử đạt, không còn lỗi nghiêm trọng và tài liệu cần thiết được cập nhật.

* DoD áp dụng thống nhất cho mọi Story; không tự ý hạ tiêu chuẩn để kịp phát hành.

Điều kiện chuyển bước:

Story được xác nhận có thể thực hiện và kiểm chứng theo DoD chung; các rủi ro, phụ thuộc được làm rõ.

Bước 4. Ưu tiên bằng MoSCoW

Chịu trách nhiệm: Product Owner (Đức); Scrum Master (Lan) hỗ trợ điều phối.

* Gán Must, Should, Could hoặc Won't dựa trên mục tiêu của lần phát hành, tác động nghiệp vụ, rủi ro và giải pháp thay thế.

* Must chiếm khoảng 60% năng lực dự kiến; Won't phải được thông báo rõ cho các bên liên quan.

Điều kiện chuyển bước:

Story có nhãn, lý do ưu tiên và vị trí rõ ràng trong Product Backlog của bản phát hành.

Bước 5. Refinement và chọn Story vào Sprint

Chịu trách nhiệm: Developers và Product Owner; Scrum Master hỗ trợ quy trình.

* Làm rõ phạm vi, ước lượng công sức và xem xét năng lực thực tế của Sprint.

* Developers chọn lượng công việc phù hợp trong Sprint Planning; Product Owner làm rõ mục tiêu và thứ tự ưu tiên.

Điều kiện hoàn tất:

Story có AC rõ ràng, phù hợp DoD, được ưu tiên và được Developers thống nhất đưa vào Sprint theo năng lực.

Nguyên tắc xuyên suốt: AC xác định Story cần làm gì và điều kiện nghiệm thu; DoD xác định mức chất lượng tối thiểu để công việc được xem là hoàn thành; MoSCoW xác định mức ưu tiên cho một lần phát hành.

## Phần 2 – Xử lý tình huống phát sinh

### Tình huống 1: Marketing yêu cầu đưa ngay Story “Tặng mã giới thiệu bạn bè” vào Sprint đang chạy nhưng chưa có AC

Cách xử lý:

Lan không đồng ý đưa Story vào Sprint ngay chỉ vì Marketing yêu cầu. Đức tiếp nhận Story vào Product Backlog, phối hợp với Marketing và Developers hoàn thiện 3–7 AC, sau đó đánh giá mức ưu tiên và công sức. Nếu thực sự cần thay đổi giữa Sprint, Product Owner trao đổi với Developers để đánh giá tác động; không được làm ảnh hưởng hoặc gây nguy hiểm cho Sprint Goal. Nếu phạm vi công việc cần thay đổi, PO và Developers thương lượng lại phạm vi; nếu Sprint Goal trở nên lỗi thời, chỉ Product Owner mới có thể hủy Sprint.

Ví dụ AC theo Given – When – Then:

AC mẫu

Story: Tặng mã giới thiệu bạn bè

Given: Người dùng đã đăng nhập và có mã giới thiệu hợp lệ.

When: Người dùng chọn chức năng chia sẻ mã giới thiệu.

Then: Hệ thống hiển thị mã giới thiệu và cho phép người dùng sao chép mã để gửi cho bạn bè.

AC trên mới là một tiêu chí mẫu. Trước khi đưa Story vào Sprint, đội cần bổ sung các AC còn lại, ví dụ: xử lý mã không hợp lệ, điều kiện nhận thưởng và chống nhận thưởng trùng, nếu thuộc phạm vi yêu cầu.

### Tình huống 2: Marketing, Chăm sóc khách hàng và Vận hành đều cho rằng yêu cầu của mình là Must

Cách xử lý:

Lan yêu cầu Đức đánh giá từng Story theo cùng một bộ tiêu chí: mức độ cần thiết để đạt mục tiêu phát hành, tác động nếu không thực hiện, rủi ro nghiệp vụ và khả năng thay thế. Product Owner quyết định thứ tự ưu tiên của Product Backlog, không dựa vào chức danh hoặc mức độ gây áp lực; Developers cung cấp ước lượng để bảo đảm khối lượng phù hợp với năng lực Sprint. Must cần chiếm khoảng 60% năng lực dự kiến, nhưng đây là mục tiêu lập kế hoạch chứ không phải lý do để gán nhãn Must một cách máy móc.

Ví dụ gán nhãn MoSCoW:

| Story                                       | Nhãn   | Lý do                                                                                                  |
| ------------------------------------------- | ------ | ------------------------------------------------------------------------------------------------------ |
| Sửa lỗi tính sai cước khuyến mãi            | Must   | Nếu không sửa, khách hàng có thể bị thu sai tiền; ảnh hưởng trực tiếp đến tính đúng đắn của nghiệp vụ. |
| Chat với tài xế                             | Should | Khách vẫn có thể gọi điện, nên có giải pháp thay thế trong bản phát hành hiện tại.                     |
| Giao diện trang trí chương trình khuyến mãi | Could  | Tăng tính hấp dẫn nhưng không quyết định khả năng áp dụng mã và tính cước chính xác.                   |
| Hẹn giờ đặt xe trước                        | Won't  | Tạm loại khỏi phạm vi bản phát hành này để tập trung nguồn lực; phải thông báo rõ cho bên yêu cầu.     |

## Kết luận

Quy trình 5 bước giúp RikkeiGo quản lý Story từ lúc tiếp nhận đến khi vào Sprint một cách thống nhất. AC bảo đảm yêu cầu rõ ràng và kiểm thử được; DoD duy trì chất lượng chung; MoSCoW giúp PO ưu tiên dựa trên giá trị phát hành; Developers quyết định lượng công việc phù hợp trong Sprint Planning.

Scrum Master không tự quyết định mọi Story là Must hay trực tiếp giao việc cho Developers. Vai trò của Lan là tạo điều kiện cho quy trình minh bạch, giúp đội xử lý bất đồng và bảo đảm các nguyên tắc Scrum được tuân thủ.
