## D8 - Learning Progress Prediction 
### Yêu cầu về môi trường:
- Python version: 3.9+
- Môi trường: Google Colab
- Ram tối thiểu: 8GB
### Yêu cầu cài đặt:
Để cài đặt môi trường, chạy lệnh sau trong notebook:<br>
```bash
pip install -q xgboost scikit-learn pandas numpy matplotlib seaborn tensorflow
```
### How to run:
- Bước 1: Tải file admission.csv, academic_records.csv và test.csv
- Bước 2:
  + Chạy file `[D8]_Data_Aggregation_&_ Integration.ipynb` để tổng hợp dữ liệu
  + Dữ liệu thu được sau khi chạy là **train_data_processed.csv** và **valid_data_processed.csv**
- Bước 3:
  + Chạy file `[D8]_Preprocessing.ipynb` để tiền xử lý dữ liệu đồng thời thêm dữ liệu quá khứ cho file test
  + Dữ liệu thu được sau khi chạy là **train_df.csv, valid_df.csv, test_df.csv**
- Bước 4:
  + Chạy file `[D8]_Model_Training.ipynb` để huấn luyện mô hình và dự đoán trên tập test
  + File **submission.csv** được tải về máy
### Cấu trúc dự án
- data/
  + train_df.csv
  + valid_df.csv
  + test_df.csv
- models/
  + student_performance_model.pkl
- notebooks/
  + [D8] Data_Aggregation_&_Integration.ipynb
  + [D8] Preprocessing.ipynb
  + [D8] Model_Training.ipynb
- README.md
- requirements.txt
