# Nộp bài (hạn 16:35, Ngày 11)

> **Google Drive Submission (5 file bài nộp):** [https://drive.google.com/drive/folders/1Zi2DzKekjX4JhPZG-hebXmrcMKEGH2gL](https://drive.google.com/drive/folders/1Zi2DzKekjX4JhPZG-hebXmrcMKEGH2gL)  
> Học viên: **Hoàng Thuận Thiên** — MSSV: **2A202603270**

Nộp đúng 5 file lên kênh nộp bài coach chỉ định. Không gửi file GT, không gửi ảnh và không đăng file lên kênh chung của lớp.

- [x] `hoangthuanthien-front.zip`: CVAT for images 1.1, **không kèm ảnh**; gồm task front (A01–A12) và front-extra nếu có làm.
- [x] `hoangthuanthien-fisheye.zip`: CVAT for images 1.1, **không kèm ảnh**; gồm task fisheye (B01–B08) và fisheye-extra nếu có làm.
- [x] `hoangthuanthien-manifest.json`: manifest bàn giao, không chấm điểm (xem [đặc tả bàn giao](docs/delivery_road_v1.0.md)).
- [x] `hoangthuanthien-qc1-for-hoangsykhiem.md`: Phiếu QC 1 đã điền theo [`templates/qc1_form.md`](templates/qc1_form.md).
- [x] `hoangthuanthien-report.md`: báo cáo theo [`templates/report.md`](templates/report.md).

Trước khi nộp:

- [x] Mọi job ở trạng thái **completed**.
- [x] Đã mở lại hai file zip và chạy `PYTHONPATH=src python3 -m road_lab.road_check lint hoangthuanthien-front.zip hoangthuanthien-fisheye.zip`; không còn dòng nào mức nặng. Nếu còn QC1-02 "chưa có L1/R1" ở ảnh thật sự không thấy vạch: đừng vẽ thêm vạch, gọi coach xác nhận và ghi mã ảnh vào phiếu.
- [x] Đã tạo manifest: thêm `--manifest hoangthuanthien-manifest.json --name hoangthuanthien --revision 1` vào lệnh trên; trong file, `contains_images` là `false`.
- [x] Mọi ảnh có đủ bốn tag, tag camera đúng.
- [x] Báo cáo có ảnh chụp màn hình và bảng kiểm file (mục 1).

Sửa sau buffer: trước khi export lại, chép hai zip và manifest cũ vào thư mục `r1/` trên máy (manifest cũ đổi tên thành `<tên>-manifest-r1.json`). Sau đó nộp hai file zip **cùng tên** và manifest mới với `--revision 2`. Ghi vào mục 4 của báo cáo đã sửa những gì.
