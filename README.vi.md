# Dự Án Phân Tích Thống Kê AMOD 5240H

> **Language / 语言 / Ngôn ngữ:** [English](README.md) | [中文](README.zh.md) | [Tiếng Việt](README.vi.md)

## Thông Tin Khóa Học

- **Khóa học:** AMOD 5240H - Thống Kê Ứng Dụng
- **Giảng viên:** Dave Riegert
- **Học kỳ:** Mùa Đông 2026

## Thành Viên Nhóm

- Feng Qiu
- Keyao Li
- Ngoc Vy

## Tổng Quan Dự Án

Dự án này áp dụng các phương pháp thống kê được học trong AMOD 5240H để phân tích bộ dữ liệu thực tế. Phân tích bao gồm khám phá dữ liệu (EDA), mô hình hồi quy tuyến tính và kiểm định giả thuyết nhằm tìm hiểu các yếu tố ảnh hưởng đến kết quả học tập của học sinh trung học.

## Bộ Dữ Liệu

**Tên:** Bộ dữ liệu Kết quả Học sinh

**Nguồn:** [Kho Học Máy UCI](https://archive.ics.uci.edu/dataset/320/student+performance)

**Tệp:** `student-por.csv` (môn tiếng Bồ Đào Nha)

**Số mẫu:** 649 học sinh

**Đặc trưng:** 33 biến (30 biến dự đoán + 3 biến điểm số)

### Mô Tả Dữ Liệu

Bộ dữ liệu chứa thông tin kết quả học tập của học sinh từ hai trường trung học tại Bồ Đào Nha (Gabriel Pereira và Mousinho da Silveira), được thu thập trong năm học 2005–2006. Dữ liệu được lấy từ hồ sơ nhà trường (điểm số) và bảng câu hỏi học sinh (thông tin cá nhân và xã hội).

### Mô Tả Biến

#### Biến Mục Tiêu (Điểm Số)
| Biến | Mô tả | Phạm vi |
|------|-------|---------|
| G1 | Điểm kỳ 1 | 0–20 |
| G2 | Điểm kỳ 2 | 0–20 |
| G3 | Điểm cuối kỳ (biến mục tiêu chính) | 0–20 |

#### Đặc Điểm Nhân Khẩu Học
| Biến | Mô tả | Kiểu |
|------|-------|------|
| school | Trường học (GP hoặc MS) | Nhị phân |
| sex | Giới tính (F/M) | Nhị phân |
| age | Tuổi | Số (15–22) |
| address | Loại địa chỉ (U: Thành thị, R: Nông thôn) | Nhị phân |
| famsize | Quy mô gia đình (LE3: ≤3, GT3: >3) | Nhị phân |
| Pstatus | Tình trạng chung sống của cha mẹ (T: Cùng ở, A: Ly thân) | Nhị phân |

#### Thông Tin Cha Mẹ
| Biến | Mô tả | Kiểu |
|------|-------|------|
| Medu | Trình độ học vấn của mẹ (0–4) | Thứ bậc |
| Fedu | Trình độ học vấn của cha (0–4) | Thứ bậc |
| Mjob | Nghề nghiệp của mẹ | Danh nghĩa |
| Fjob | Nghề nghiệp của cha | Danh nghĩa |

#### Đặc Điểm Liên Quan Đến Trường Học
| Biến | Mô tả | Kiểu |
|------|-------|------|
| reason | Lý do chọn trường | Danh nghĩa |
| guardian | Người giám hộ của học sinh | Danh nghĩa |
| traveltime | Thời gian đi học (1–4) | Thứ bậc |
| studytime | Thời gian học mỗi tuần (1–4) | Thứ bậc |
| failures | Số lần trượt môn trong quá khứ | Số |
| schoolsup | Hỗ trợ giáo dục thêm từ trường | Nhị phân |
| famsup | Hỗ trợ học tập từ gia đình | Nhị phân |
| paid | Học thêm có trả phí | Nhị phân |
| activities | Tham gia hoạt động ngoại khóa | Nhị phân |
| nursery | Đã học mầm non | Nhị phân |
| higher | Muốn học lên cao | Nhị phân |
| internet | Có internet ở nhà | Nhị phân |

#### Yếu Tố Xã Hội / Hành Vi
| Biến | Mô tả | Kiểu |
|------|-------|------|
| romantic | Đang trong mối quan hệ tình cảm | Nhị phân |
| famrel | Chất lượng quan hệ gia đình (1–5) | Thứ bậc |
| freetime | Thời gian rảnh sau giờ học (1–5) | Thứ bậc |
| goout | Tần suất ra ngoài với bạn bè (1–5) | Thứ bậc |
| Dalc | Uống rượu ngày làm việc (1–5) | Thứ bậc |
| Walc | Uống rượu cuối tuần (1–5) | Thứ bậc |
| health | Tình trạng sức khỏe hiện tại (1–5) | Thứ bậc |
| absences | Số buổi vắng mặt | Số (0–93) |

## Phân Công Biến

| Thành viên | Biến phụ trách |
|-----------|---------------|
| Feng Qiu | `reason` |
| Ngoc Vy | `failures` |
| Keyao Li | `address` |

## Tiến Độ Dự Án

| Thành phần | Hạn nộp | Trọng số | Trạng thái |
|-----------|---------|---------|-----------|
| Phần 1: Dữ liệu & Biến | 13/02/2026 | 4% | Hoàn thành |
| Phần 2: EDA & Đề xuất phân tích | 06/03/2026 | 4% | Hoàn thành |
| Thuyết trình | 03/04/2026 | 4% | Hoàn thành |
| Phần 3: Báo cáo cuối kỳ | 10/04/2026 | 8% | Hoàn thành |

---

### Phần 1 — Dữ liệu & Biến ✅

- [x] Giới thiệu bộ dữ liệu
- [x] Mô tả biến
- [x] Bối cảnh nghiên cứu (tính phù hợp với hồi quy tuyến tính)
- [x] Đánh giá chất lượng dữ liệu (giá trị thiếu, ngoại lệ, làm sạch dữ liệu)

---

### Phần 2 — EDA & Đề Xuất Phân Tích ✅

#### EDA
- [x] `reason` (Feng Qiu)
- [x] `failures` (Ngoc Vy)
- [x] `address` (Keyao Li)

#### Các Mục Viết
- [x] Mục 2.1 Tóm tắt bộ dữ liệu
- [x] Mục 2.3 Câu hỏi nghiên cứu (hồi quy tuyến tính + ANOVA một chiều)
- [x] Mục 2.4 Kế hoạch phân tích
- [x] Mục 2.5 Thách thức tiềm ẩn
- [x] Phụ lục chứa nội dung Phần 1

---

### Phần 3 — Báo Cáo Cuối Kỳ [~8–12 trang] — Hạn nộp 10/04/2026

#### Nhiệm Vụ Nội Dung

- [x] **Tóm tắt điều hành** — đã bao gồm cả ba biến dự đoán (`reason`, `failures`, `address`) ✅
- [x] Giới thiệu và bối cảnh (Phần 1 đã chỉnh sửa) ← Feng ✅
- [x] Phân tích khám phá dữ liệu
  - [x] EDA `reason` ← Feng ✅
  - [x] EDA `failures` ← Vy ✅
  - [x] EDA `address` ← Keyao ✅
- [x] Phương pháp
  - [x] Tổng quan phương pháp và khung thống kê ← Vy ✅
  - [x] HQ đơn biến: G3 ~ `reason` (phương trình, F-test, t-test, CI 95%) ← Feng ✅
  - [x] HQ đơn biến: G3 ~ `failures` (phương trình, F-test, t-test) ← Vy ✅
  - [x] HQ đơn biến: G3 ~ `address` (phương trình, F-test, CI 95%) ← Keyao ✅
  - [x] Phát biểu và kiểm tra các giả định hồi quy tuyến tính ← Feng ✅
- [x] Kết quả
  - [x] ANOVA một chiều: G3 theo `reason` (F-stat, Levene's, Tukey HSD) ← Feng ✅
  - [x] ANOVA một chiều: G3 theo `failures` (F-stat, Tukey HSD) ← Vy ✅
  - [x] Kiểm định t hai mẫu độc lập: G3 theo `address` ← Keyao ✅
  - [x] Biểu đồ chẩn đoán mô hình `reason` (Residuals vs Fitted, Scale-Location, Q-Q) ← Feng ✅
  - [x] Biểu đồ chẩn đoán mô hình `failures` ← Vy ✅
  - [x] Xử lý G3 = 0 — đã loại bỏ và ghi lại lý do ← Feng ✅
- [x] Thảo luận
  - [x] Kết quả `reason` đã thảo luận ← Feng ✅
  - [x] Kết quả `address` đã thảo luận ← Keyao ✅
  - [x] Kết quả `failures` đã thảo luận ← Vy ✅
  - [x] Kiểm tra giả định mô hình ← Feng ✅
  - [x] Ghi nhận hạn chế ← Feng ✅
- [x] **Kết luận** — Mục 5 đã được thêm (5.1 Phát hiện chính, 5.2 Hàm ý thực tiễn, 5.3 Câu hỏi còn lại) ✅

#### Sửa Lỗi Định Dạng / Tuân Thủ Yêu Cầu

- [x] **Tóm tắt điều hành** — đã bổ sung đầy đủ cho cả ba biến ✅
- [x] **Mục Kết luận** — `## 5. Conclusion` đã được thêm ✅
- [x] **Số nhóm trên trang bìa** — đã thêm (Nhóm 6) ✅
- [x] **Code đã ẩn / Appendix đã thêm** — đã thiết lập `execute: echo: false` toàn cục trong YAML; toàn bộ 44 chunk đã được gán nhãn; đã thêm `\newpage` + `# Appendix: Full R Code` cuối tài liệu với `ref-label: !expr knitr::all_labels()` ✅
- [x] **Lỗi đánh số mục trong Part 1** — Các mục 1.5, 1.6, 1.7 đã đổi thành 1.4.1, 1.4.2, 1.4.3; tham chiếu chéo trong mục 1.4.3 đã được cập nhật ✅

---

### Thuyết Trình ✅ — Hoàn thành ngày 03/04/2026

## Kết Quả Chính (EDA)

### `reason` — Lý Do Chọn Trường
| Lý do | n | Điểm G3 TB | Độ lệch chuẩn |
|-------|---|-----------|--------------|
| reputation (danh tiếng) | 143 | 12.94 | 3.05 |
| home (gần nhà) | 149 | 12.18 | 2.95 |
| course (chương trình) | 285 | 11.55 | 3.11 |
| other (khác) | 72 | 10.69 | 3.93 |

Học sinh chọn trường vì danh tiếng đạt điểm cuối kỳ trung bình cao nhất. Nhóm "khác" có kết quả biến động lớn nhất. SLR: F(3, 630) = 10.5, p ≈ 0, R² = 4.8%. Tukey HSD: chỉ có reputation vs. course và reputation vs. other là có sự khác biệt có ý nghĩa thống kê.

### `failures` — Số Lần Trượt Môn Trước Đây
| Số lần trượt | n | Điểm G3 TB |
|-------------|---|-----------|
| 0 | 549 | 12.51 |
| 1 | 70 | 8.64 |
| 2 | 16 | 8.81 |
| 3 | 14 | 8.07 |

Chỉ một lần trượt môn đã liên quan đến việc giảm khoảng 4 điểm trong điểm cuối kỳ. Tác động này không có tính tích lũy rõ ràng khi số lần trượt tăng từ 1 đến 3.

### `address` — Loại Địa Chỉ Nhà
| Địa chỉ | n | Điểm G3 TB |
|---------|---|-----------|
| Thành thị (U) | 452 | 12.3 |
| Nông thôn (R) | 197 | 11.1 |

Học sinh thành thị có điểm trung bình cao hơn học sinh nông thôn khoảng 1.2 điểm. Cả hai nhóm đều có trường hợp điểm 0 (11 thành thị, 4 nông thôn). Học sinh thành thị cũng có trung vị cao hơn và khoảng tứ phân vị tập trung hơn.

## Cấu Trúc Kho Lưu Trữ

```
5240-project/
├── README.md                        # Tài liệu dự án (tiếng Anh)
├── README.zh.md                     # Tài liệu dự án (tiếng Trung)
├── README.vi.md                     # Tài liệu dự án (tiếng Việt)
├── 5240H Project.qmd                # Tài liệu phân tích Quarto chính
├── 5240H-Project.pdf                # Báo cáo đã xuất bản
├── student-por.csv                  # Bộ dữ liệu (môn tiếng Bồ Đào Nha)
├── references.bib                   # Danh mục tài liệu tham khảo
├── apa.csl                          # Định dạng trích dẫn APA
├── presentation/                    # Tài liệu thuyết trình
│   ├── Is Your GPA Your Fault?.key  # Slides Keynote
│   ├── 2015_TrentU PPT Template_FINAL2.potx
│   ├── presentation outline.md      # Đề cương slide (tiếng Anh)
│   ├── presentation outline.zh.md   # Đề cương slide (tiếng Trung)
│   └── presentation outline.vi.md   # Đề cương slide (tiếng Việt)
└── docs/                            # Tài liệu tham khảo
    ├── 5240-project-part0_overview-wi26.pdf
    ├── 5240-project-part1_background-wi26.pdf
    ├── Standard Operating Procedure_ Variable Screening.pdf
    ├── Project Revised.pdf
    └── How to Merge Main into Your Personal Branch via GitHub Desktop.md
```

## Công Cụ

- **R** — Phân tích thống kê
- **Quarto** — Xuất bản tài liệu
- **ggplot2** / **tidyverse** — Trực quan hóa và xử lý dữ liệu

## Giấy Phép

Bộ dữ liệu được cấp phép theo [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).

## Tài Liệu Tham Khảo

Cortez, P., & Silva, A. (2008). Using data mining to predict secondary school student performance. In *Proceedings of 5th Annual Future Business Technology Conference* (pp. 5-12). EUROSIS.

UCI Machine Learning Repository. (2014). Student Performance Dataset. https://archive.ics.uci.edu/dataset/320/student+performance

OECD. (2012). *Equity and quality in education: Supporting disadvantaged students and schools*. OECD Publishing.
