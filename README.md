# Phương pháp
Phát hiện tin giả dựa trên các thuật toán học máy: 
- SVM
- Naive Bayes
- k-NN

# Độ đo:
- Precision
- Recall
- F1
# Dữ liệu: Bộ dữ liệu FakeNewsNet gồm các file:
- gossipcop_fake.csv
- gossipcop_real.csv
- politifact_fake.csv
- politifact_real.csv

# Cấu hình cài đặt:
 * Cài đặt python 3.6+ trở lên
 * Cài đặt các thư viện trong file requirements.txt: pip install -r requirements.txt
 * Cài đặt thêm các thư viện khác trong file requirements
(Để cài đặt thêm các thư viện: Dùng lệnh pip install tên_thư_viện

# Mô tả các file
 * DataPrep.py: Tiền xử lý dữ liệu
 * FeatureSelection.py: 

Thực hiện trích xuất và lựa chọn đặc trưng từ các thư viện sci-kit. 

Để lựa chọn đặc trưng, sử dụng các phương pháp như túi từ và n-gram đơn giản.
 * classifier.py: 

Xây dựng các bộ phân loại để dự đoán phát hiện tin tức giả. 

Các đặc trưng được trích xuất sẽ được đưa vào các bộ phân loại khác nhau. 
 * prediction.py

Bộ phân loại cuối cùng được chọn và hoạt động tốt nhất là SVM.

Run cmd: python prediction.py
 * FND-dataset_gossipcop.ipynb: Đánh giá các mô hình trên bộ dữ liệu Gossipcop
 * FND-dataset_politifact.ipynb: Đánh giá các mô hình trên bộ dữ liệu PolitiFact