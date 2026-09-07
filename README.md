# Analyzing the Job Market: Trends, Skills, and insights (10/2025 - 11/2025)

Bài tập lớn môn học: Phân tích Dữ liệu (Data Analysis Project)

Sinh viên thực hiện: Võ Hoàng Thịnh

Trường: Đại học Mở Thành phố Hồ Chí Minh (Ho Chi Minh City Open University)

Chuyên ngành: Khoa học Dữ liệu (Computer Science - Data Science)

 # 1. Giới thiệu Dự án (Introduction)
Trong bối cảnh thị trường tuyển dụng ngành Dữ liệu (Data Analytics) đang cạnh tranh gay gắt, việc nắm bắt chính xác xu hướng công nghệ, nhu cầu kỹ năng và mức lương là chìa khóa quan trọng cho định hướng nghề nghiệp của một Data Analyst.

Dự án này thực hiện việc thu thập, làm sạch và khai thác dữ liệu từ hàng ngàn tin tuyển dụng thực tế nhằm trả lời cho các câu hỏi trọng tâm:

Ngôn ngữ lập trình và công cụ nào đang thống trị thị trường tuyển dụng?

Mức thu nhập trung bình và cấu trúc trả lương (theo giờ, theo năm) phân hóa ra sao?

Những kỹ năng cốt lõi nào mà một Data Analyst thực tập/mới ra trường bắt buộc phải trang bị?

#  2. Công nghệ & Thư viện sử dụng (Tech Stack)
Dự án được xây dựng hoàn toàn bằng ngôn ngữ Python thông qua môi trường Jupyter Notebook, sử dụng các thư viện chuyên sâu cho xử lý và trực quan hóa dữ liệu:

Xử lý dữ liệu (Data Manipulation): Pandas, NumPy

Xử lý ngôn ngữ tự nhiên & Tokenize: NLTK (word_tokenize, MWETokenizer) để trích xuất từ khóa kỹ năng từ mô tả công việc.

Trực quan hóa dữ liệu (Data Visualization): Matplotlib để vẽ biểu đồ thống kê chuyên nghiệp.

# 3. Quy trình xử lý dữ liệu (Data Pipeline & Preprocessing)
Tập dữ liệu đầu vào gồm các tin tuyển dụng (gsearch_jobs.csv) đã trải qua các bước xử lý kỹ thuật nghiêm ngặt:

Làm sạch dữ liệu (Data Cleansing): Loại bỏ các giá trị null, chuẩn hóa định dạng ngày tháng (datetime), loại bỏ ký tự nhiễu.

Chuẩn hóa mức lương (Salary Standardization):

Tách cột lương thô thành mức tối thiểu (salary_min), tối đa (salary_max), trung bình (salary_avg) và tần suất trả lương (salary_rate).

Quy đổi toàn bộ các mức lương theo giờ (hourly) hoặc theo tháng về chung một chuẩn Lương năm quy đổi (salary_standardized) để dễ dàng so sánh.

Trích xuất từ khóa kỹ năng (Keyword Tokenization): Sử dụng NLTK để chuyển đổi văn bản mô tả công việc (description) thành các token chữ thường, xử lý các cụm từ ghép (như Power BI, Data Lake, Machine Learning) và lọc qua danh sách từ khóa chuẩn (Programming languages, Libraries, Analyst tools, Cloud tools).

# 4. Kết quả & Phân tích chuyên sâu (Key Findings & Insights)
A. Thống kê tổng quan dữ liệu
Tổng số bản ghi: 1,820 tin tuyển dụng được phân tích.

Thời gian thu thập: Dữ liệu được theo dõi và ghi nhận qua chuỗi thời gian dài, đảm bảo tính khách quan của thị trường.

B. Top Ngôn ngữ lập trình thiết yếu cho Data Analyst
Dựa trên phân tích tần suất xuất hiện của các ngôn ngữ lập trình trong tin tuyển dụng, kết quả cho thấy sự thống trị tuyệt đối của nhóm công cụ cốt lõi:

SQL (chiếm ~55% tin tuyển dụng): Vẫn giữ vững ngôi vương là kỹ năng quan trọng nhất mà bất kỳ nhà phân tích dữ liệu nào cũng phải nắm vững để truy xuất dữ liệu từ cơ sở dữ liệu quan hệ.

Python (~32%): Ngôn ngữ lập trình số một cho việc làm sạch dữ liệu, tự động hóa và xây dựng mô hình phân tích.

R (~24%): Vẫn duy trì sức hút ổn định trong môi trường nghiên cứu và thống kê chuyên sâu.

SAS & các ngôn ngữ khác: Xuất hiện với tỷ lệ thấp hơn, thường phục vụ cho các doanh nghiệp tài chính hoặc hệ thống legacy lớn.

# Business Insight: Đối với sinh viên hoặc ứng viên vị trí Data Analyst Intern, việc thành thạo bộ đôi SQL và Python là điều kiện tiên quyết để vượt qua vòng hồ sơ tại hơn một nửa số công ty tuyển dụng.

# 5. Hướng dẫn sử dụng & Khám phá mã nguồn (How to Run)
Clone repository này về máy:


Bash
git clone https://github.com/Th1nhph0/analyzingJobMarket.git


Cài đặt các thư viện phụ thuộc:


Bash

pip install pandas numpy matplotlib nltk

Mở file báo cáo mã nguồn đầy đủ để xem chi tiết biểu đồ và các bước phân tích:

Jupyter Notebook: PTDL.ipynb

Dự án hoàn thành nhằm mục đích nâng cao năng lực thực chiến về xử lý dữ liệu và làm tài liệu minh chứng năng lực (Portfolio) ứng tuyển vị trí Data Analyst Intern.
