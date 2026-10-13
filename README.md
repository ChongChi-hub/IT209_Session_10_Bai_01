# Báo cáo Thực hành DevOps - Session 10: Bài 1

- **Học viên:** Đào Trọng Trí
- **Mã sinh viên:** PTIT062
- **Lớp:** DevOps / Cloud Native Engineering
- **Bài tập:** Phân tích kiến trúc Container vs Virtual Machine & Khảo sát Docker Engine

## 1. Giới thiệu nội dung
Thư mục này chứa báo cáo kỹ thuật chi tiết (`REPORT.md`) phân tích sự khác biệt kiến trúc giữa ảo hóa phần cứng (VM/Hypervisor) và ảo hóa hệ điều hành (Container Engine), cơ chế cô lập của Linux Kernel (Namespaces, cgroups), và nhật ký thực thi thực tế của lệnh `docker info`, `docker version` trên máy chủ thực tế.

## 2. Cấu trúc thư mục
```text
SS10_HW01_DaoTrongTri_PTIT062/
├── README.md       # Tài liệu tổng quan bài nộp
└── REPORT.md       # Báo cáo kỹ thuật phân tích chuyên sâu (>300 từ) và log thực tế
```

## 3. Nội dung chính trong REPORT.md
- **Mục 1:** Lý do các doanh nghiệp hiện đại chuyển dịch từ VPS sang Docker Container.
- **Mục 2:** Bảng so sánh VM vs Container qua 5 tiêu chí: Dung lượng Image, Thời gian khởi động, Hao phí OS, Mức độ cô lập, Khả năng mở rộng; kèm sơ đồ Mermaid trực quan.
- **Mục 3:** Phân tích vai trò của Linux Namespaces (PID, NET, MNT, UTS, IPC, USER) và Linux Control Groups (cgroups v2).
- **Mục 4:** Trích xuất và giải thích các thông số hệ thống từ `docker info`.
- **Mục 5:** Toàn văn log kết quả chạy lệnh `docker version` và `docker info` không cần quyền sudo.
- **Mục 6:** Vị trí đặt placeholder `ImgEx` cho ảnh chụp màn hình minh chứng.

Chi tiết vui lòng xem tại tệp [REPORT.md](REPORT.md).
