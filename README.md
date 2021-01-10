# gitpage
EDA là phương pháp khai phá dữ liệu, phân tích dữ liệu. Trước tiên, cần import các thư viện numpy, pandas, seaborn, matplotlist... sau đó phải tìm kiếm file rồi tải về, tiến hành upload lên. Tiếp theo, phải kiểm tra xem dữ liệu có nhiều chỗ rỗng không bằng hàm isnull(), nếu thấy cột dữ liệu rỗng thì có thể drop. Đối với dữ liệu cột bị thiếu nếu là biến định lượng thì có thể thay thế bằng giá trị trung bình hoặc trung vị, nếu là biến phân loại thì thay thế bằng giá trị xuất hiện nhiều nhất. Sau đó thực hiện thống kê mô tả bằng hàm describe(). Ta sẽ xác định được các đại lượng: min, max, giá trị trung bình, giá trị trung vị, phương sai, độ lệch chuẩn,...cuối cùng là biểu diễn bằng biểu đồ. Biến định lượng sử dụng biểu đồ histogram bằng hàm hist(), biến phân loại loại sử dụng biểu đồ cột bằng hàm countplot(). Xem mối tương quan giữa 2 biến định lượng sử dụng biểu đồ scatter bằng hàm scatterplot(). Mối tương quan giữa biến định lượng và phân loại sử dụng biểu đồ boxplot bằng hàm boxplot().

Thống kê dữ liệu thì sử dụng hàm describe(). Dựa vào đó để phân tích các đại lượng thống kê.
- count: biểu diễn số lượng điểm trong dữ liệu.
- mean: giá trị trung bình.
- std: Độ lệch chuẩn.
- min: giá trị nhỏ nhất.
- 25%: phân vị 25%, gồm 25 phần tử từ 1 - 25
- 50%: phân vị 50%, gồm 25 phần tử từ 26 - 50
- 75%: phân vị 75%, gồm 25 phần tử từ 51 - 75
- max: giá trị lớn nhất.

Sử dụng df.hist(column="Điểm.1")
Trục y: Biểu thị giá trị điểm biến thiên từ min (điểm = 0)
đến max (điểm = 7), chia khoảng cách điểm.
Trục x: thể hiện số lượng điểm có giá trị được xác định ở cột y

Biểu đồ boxplot với x: Điểm.1, y: Giới tính
Nhận thấy: Có 1 giá trị 0, 2 đầu mút là giá trị điểm từ 3.5 đến 7.
Trong đó, phần màu xanh là sự tập trung của điểm xuất hiện nhiều lần.
Đường gạch đứng giữa phần màu xanh biểu thị giá trị trung bình số điểm của 64 sinh viên giới tính "Nữ".
Trong dữ liệu, cột giới tính có 1 giá trị là "Nam" nên phần Nam với điểm số là 5.5 nằm trên đường giá trị trung bình.
