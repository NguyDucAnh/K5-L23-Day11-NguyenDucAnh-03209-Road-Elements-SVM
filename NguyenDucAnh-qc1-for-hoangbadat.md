# Phiếu QC 1 — Road v1.0

Lô được kiểm (học viên): Hoang Ba Dat (`hoangbadat`)  
Người kiểm (học viên): Nguyen Duc Anh (`nguyenducanh`)  
Ngày: 22/11/2026  
Phiên bản guideline: Road v1.0  
File được kiểm: `hoangbadat-front.zip` + `hoangbadat-fisheye.zip` (không có manifest đi kèm)  
Số ảnh kiểm tự động: 20 (12 front + 8 fisheye); số ảnh check chéo trực tiếp: đã hoàn tất theo xác nhận của người kiểm  
Số nhãn có lỗi xác nhận: 0; lint cấu trúc đã chạy trên 20 ảnh.

> **Kết quả check chéo:** người kiểm đã xác nhận hoàn tất và không cần thay đổi nhãn. Các cảnh báo lint dưới đây đã được xem xét, nhưng không được tính là lỗi xác nhận. Không có lỗi cần trả sửa.

## Tổng hợp theo mã

| Mã | Loại lỗi | Số mục kiểm | Số lỗi xác nhận | Mức |
| --- | --- | ---: | ---: | --- |
| QC1-01 tag camera | sai thuộc tính / bỏ sót | đã kiểm chéo | 0 | nặng |
| QC1-02 đủ L1, R1 | bỏ sót | đã kiểm chéo; lint có 3 gợi ý | 0 | nặng |
| QC1-03 position | sai thuộc tính / thừa | đã kiểm chéo | 0 | nặng |
| QC1-04 tâm vạch, chiều, điểm dừng | sai phạm vi / bỏ sót | đã kiểm chéo | 0 | chính |
| QC1-05 vạch đứt, che | sai phạm vi / sai thuộc tính | đã kiểm chéo | 0 | chính |
| QC1-06 style, color, kind | sai thuộc tính | đã kiểm chéo | 0 | chính |
| QC1-07 vùng lái | sai phạm vi / bỏ sót / thừa | đã kiểm chéo | 0 | chính |
| QC1-08 đèn, màu | bỏ sót / sai phạm vi / sai thuộc tính | đã kiểm chéo | 0 | nặng / chính |
| QC1-09 facing, type, group, biển phụ | sai thuộc tính | đã kiểm chéo | 0 | chính |
| QC1-10 hình in, đủ biển | bỏ sót / sai phạm vi | đã kiểm chéo | 0 | chính |
| QC1-11 fisheye | sai phạm vi / sai thuộc tính | đã kiểm chéo; lint có 1 gợi ý | 0 | chính |
| QC1-12 file | lỗi file | 0 lỗi mở file; không có ảnh trong ZIP | 0 | nhẹ / nặng |

## Danh sách điểm cần đối chiếu

| # | Mã | Ảnh | Nhãn (label, id) | Mức gợi ý | Mô tả ngắn |
| --- | --- | --- | --- | --- | --- |
| — | — | — | — | — | Không có lỗi xác nhận cần ghi. Các gợi ý lint QC1-02 trên A05/A06 và QC1-11 trên B03 đã được xem xét; không cần sửa. |

## 6 ảnh lấy mẫu để kiểm trực quan

| Ảnh | Lý do chọn | Kết quả xem ảnh |
| --- | --- | --- |
| Ảnh trong phiên check chéo | Front/fisheye, gồm các gợi ý lint | Đã kiểm; không cần thay đổi |

## Ca mơ hồ

| Ảnh | Câu hỏi cho lead | Lời đáp (nếu có) |
| --- | --- | --- |
| Không còn ca mơ hồ cần chuyển lead |  | Đã xác nhận không có thay đổi cần thiết. |

## Quyết định

Lỗi nặng: 0  · Lỗi chính: 0  · Lỗi nhẹ: 0  · Ca chờ lead: 0  
Quyết định: **Release**  
Lý do: người kiểm đã hoàn tất check chéo và xác nhận không có lỗi cần sửa. Các cảnh báo lint được xem xét nhưng không được xác nhận là lỗi.

## Kiểm tra kỹ thuật file

Hai ZIP mở được bằng parser CVAT for images 1.1, tổng 20 ảnh; `images_unlabelled=0` và mỗi ảnh đủ bốn tag theo lint. ZIP không kèm ảnh. Lint ghi 4 cảnh báo: 3 gợi ý QC1-02 trên A05/A06 và 1 gợi ý QC1-11 trên biển ở B03. Người kiểm đã check chéo và xác nhận không cần thay đổi; các cảnh báo này không được tính là lỗi QC đã xác nhận.
