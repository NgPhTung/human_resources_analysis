<img width="4150" height="2400" alt="image" src="https://github.com/user-attachments/assets/160cfee7-d1ae-4e93-bf60-3d4943332e0d" /># human_resources_analysis
Developed an end-to-end HR Analytics system for 22,214 records using SQL for ETL and Power BI for data modeling, delivering actionable insights into attrition rates, demographics, and workforce diversity to drive data-led retention and planning strategies.


# 1. Tổng quan nguồn dữ liệu

Dự án được thực hiện trên tập dữ liệu gồm 22.214 bản ghi, bao gồm các thuộc tính nhân sự chi tiết như: độ tuổi, giới tính, sắc tộc, phòng ban, vị trí công việc, địa điểm làm việc, ngày gia nhập và ngày nghỉ việc.

File dữ liệu: human_resource_raw_data.csv

#2. Chỉ số mục tiêu (North Star Metrics)

Phân tích tập trung vào 3 nhóm chỉ số cốt lõi để đánh giá sức khỏe doanh nghiệp:

- Tỷ lệ biến động nhân sự (Turnover Rate): Đo lường tỷ lệ nhân viên rời bỏ tổ chức so với quy mô tổng thể.

- Phân bổ nguồn lực (Employee Distribution): Cơ cấu nhân sự theo khu vực địa lý, phòng ban và chức danh.

- Thâm niên trung bình (Tenure): Thời gian gắn bó trung bình của nhân viên tại công ty.

# 3. Các chiều phân tích (Data Dimensions)

- Nhân khẩu học: Giới tính, Độ tuổi, Sắc tộc.

- Vận hành: Phòng ban, Vị trí công việc, Địa điểm.

- Thời gian: Dòng thời gian gia nhập và nghỉ việc.

# 4. Tóm tắt kết quả phân tích (Executive Summary)

Dự án đã bóc tách các xu hướng nhân sự trọng yếu, mang lại cái nhìn toàn cảnh về lực lượng lao động:

- Cơ cấu nhân lực: Đội ngũ nhân viên có sự cân bằng về giới tính, trong đó nhóm tuổi từ 31–40 chiếm tỷ trọng lớn nhất, đóng vai trò nòng cốt trong tổ chức.

- Phân tích biến động: Dữ liệu chỉ ra sự phân hóa rõ rệt về tỷ lệ nghỉ việc giữa các bộ phận. Trong đó, Kiểm toán (Auditing) và Pháp chế (Legal) là hai phòng ban có tỷ lệ biến động cao nhất, cần có các chính sách cải thiện môi trường làm việc đặc thù.

- Gắn bó tổ chức: Thâm niên trung bình của nhân viên đạt mức 7 năm, cho thấy mức độ ổn định khá tốt của doanh nghiệp.


![Dashboard trang 1](Human%20Resources%20Analyst_1.jpg)

![Dashboard trang 2](Human%20Resources%20Analyst_2.jpg)

# 5. Phân tích Chuyên sâu (Insights Deep Dive)

Các phát hiện quan trọng:

- Cơ cấu độ tuổi: Nhóm nhân viên từ 31–40 tuổi chiếm tỷ trọng cao nhất; các nhóm tuổi còn lại có sự phân bổ tương đối đồng đều, tạo nên một lực lượng lao động đa thế hệ.

- Cân bằng giới tính: Cơ cấu giới tính đạt mức cân bằng lý tưởng với 51.01% nam và 46.24% nữ, cùng một tỉ lệ nhỏ các nhóm bản dạng giới khác.

- Đa dạng sắc tộc: Lực lượng lao động có sự góp mặt của nhiều nhóm sắc tộc, dẫn đầu là nhóm White (5.2K nhân viên), tiếp theo là các nhóm Two or More Races, Black or African American và Asian.

- Biến động nhân sự (Turnover): Bộ phận Kiểm toán (Auditing) ghi nhận tỷ lệ nghỉ việc cao nhất doanh nghiệp, lên tới xấp xỉ 17%.

- Môi trường làm việc: Phần lớn đội ngũ (75%) làm việc trực tiếp tại trụ sở chính, trong khi 25% còn lại đang vận hành theo mô hình làm việc từ xa (Remote).

# 6. Đề xuất chiến lược (Recommendations)

Dựa trên các kết quả phân tích, tôi đề xuất các hành động sau:

- Tối ưu giữ chân nhân tài: Cần khảo sát sâu để tìm hiểu nguyên nhân gây ra tỷ lệ nghỉ việc cao tại bộ phận Kiểm toán và Pháp chế (do áp lực công việc hay mức độ hài lòng) để có phương án điều chỉnh kịp thời.

- Thúc đẩy bình đẳng và hòa nhập (D&I): Mặc dù tổ chức có sự đa dạng về sắc tộc, cần đảm bảo sự đại diện này đồng đều ở tất cả các cấp phòng ban thông qua các quy trình tuyển dụng không định kiến.

- Gắn kết nhân sự từ xa: Với 1/4 nhân sự làm việc remote, HR cần tăng cường các công cụ tương tác trực tuyến và các chương trình gắn kết đội ngũ để tránh cảm giác bị cô lập và duy trì hiệu suất.

# 7. Giả định và Hạn chế (Assumptions & Caveats)

- Giả định: Dữ liệu được coi là phản ánh đầy đủ thực trạng nhân sự hiện tại và cột new_termdate (ngày nghỉ việc) được ghi nhận chính xác trên hệ thống.

- Hạn chế: Phân tích mới chỉ dừng lại ở các chỉ số định lượng có sẵn. Nếu có thêm dữ liệu định tính như hiệu suất làm việc (KPI) hoặc điểm hài lòng (Employee Engagement Score), bức tranh về động lực vận hành của doanh nghiệp sẽ toàn diện hơn.
