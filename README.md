# scaNN_Assignment

## Mô tả dự án

Bộ notebook này so sánh hai cách thực hiện truy vấn tương đồng (nearest neighbors) trên embedding text:

1. **ScaNN** — một thư viện tăng tốc Approximate Nearest Neighbors (ANN).
2. **Brute-force** — tính cosine similarity toàn bộ dataset (dùng để đối chiếu độ chính xác và thời gian).

Mục tiêu: đo hiệu năng (thời gian) khi làm việc với dataset lớn (ví dụ ~500.000 vectors).

---

## Liên kết Google Colab

* Notebook ScaNN: [https://colab.research.google.com/drive/1uhgY7Q1F76mHqaqXzGNEgGmfCGvGb8Yf#scrollTo=8FkHCYtE0yHA](https://colab.research.google.com/drive/1uhgY7Q1F76mHqaqXzGNEgGmfCGvGb8Yf#scrollTo=8FkHCYtE0yHA)

> Mở trực tiếp các link trên để chạy từng notebook trong môi trường Colab.

---

## Hướng dẫn nhanh

1. Mở Google Colab ở link trên.
2. Chạy tuần tự các ô (Run all) — Colab sẽ cài đặt các package cần thiết (nếu cần) và tải dữ liệu mẫu/embedding.

---

## Nội dung các file / notebook

* `ScanNN` notebook: cấu hình và build ScaNN + Brute-force làm ground truth. Chạy truy vấn đo thời gian và recall so với brute-force cho nhiều giá trị k.

---

## Tài liệu tham khảo & Credits

* ScaNN: [https://github.com/google-research/google-research/tree/master/scann](https://github.com/google-research/google-research/tree/master/scann)
* ScaNN for Alloy DB: [https://services.google.com/fh/files/misc/scann_for_alloydb_whitepaper.pdf](https://services.google.com/fh/files/misc/scann_for_alloydb_whitepaper.pdf)
* Google Colab và tài liệu các thư viện tương ứng.