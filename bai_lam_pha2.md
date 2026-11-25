# BÀI LÀM PHA 2 

- **Họ tên: Đỗ nguyễn Trung Kiên**
- **Lớp: KS26-CNTT1**
- **Link repository Pha2: https://github.com/TkIen-hue/KS-26-CNTT1_PromptAI_H02_Pha2.git**
- **Công cụ AI đã dùng (ChatGPT/Claude/Gemini):**

> Pha 2 (20 phút cuối). Mỗi mục: mở cuộc trò chuyện mới, gửi nguyên văn prompt đã viết trong bai_lam_pha1.md, dán câu trả lời và link chia sẻ vào đây. Xong, kéo thả file này vào repository Pha2.

## 4.2. Trích xuất tin nhắn đặt vé ra JSON

**KET QUA AI**

```text
{
  "TN1": {
    "ma_goi": null,
    "ngay_su_kien": "2026-12-20",
    "nguoi_lon": 2,
    "tre_em": 1,
    "loai_ve": "thuong",
    "ghi_chu": null
  },
  "TN2": {
    "ma_goi": "FZ",
    "ngay_su_kien": "2027-01-05",
    "nguoi_lon": 3,
    "tre_em": 0,
    "loai_ve": null,
    "ghi_chu": "hỗ trợ xe lăn"
  },
  "TN3": {
    "ma_goi": null,
    "ngay_su_kien": null,
    "nguoi_lon": 4,
    "tre_em": 0,
    "loai_ve": "vip",
    "ghi_chu": "hỗ trợ tìm chỗ"
  }
}
```

**Link trò chuyện: https://share.gemini.google/JmzQmyaIOLeK**

## 4.3. Báo giá vé bằng Chain-of-Thought

**KET QUA AI**

```text
- Căn cứ vào bảng giá vé và các quy tắc tính giá trong tài liệu đính kèm, dưới đây là quy trình phân tích và tính toán chi tiết cho yêu cầu báo giá của nhóm cổ động viên mua gói SVT (đơn giá 1.200.000 đồng/người lớn; lưu ý: thông tin về việc áp dụng riêng cho trận bán kết không có trong tài liệu đính kèm, hệ thống tính theo bảng giá chung của gói SVT):
1. Xác định số người lớn:
- Nhóm cổ động viên có 5 người lớn.
2. Xác định độ tuổi của trẻ em và số trẻ em:
- Nhóm gồm 2 trẻ em ở độ tuổi 8 tuổi và 10 tuổi (thuộc nhóm từ 5 đến 11 tuổi) cùng 1 bé 3 tuổi (thuộc nhóm dưới 5 tuổi).
- Tính tiền vé của người lớn và trẻ em:
- Đơn giá gói SVT cho người lớn là 1.200.000 đồng/người. Tiền vé của 5 người lớn là: 5 × 1.200.000 = 6.000.000 đồng.
- Trẻ em từ 5 đến 11 tuổi được tính 70% giá người lớn, tức là 1.200.000 × 70% = 840.000 đồng/trẻ em. Tiền vé cho 2 trẻ em (8 tuổi và 10 tuổi) là: 2 × 840.000 = 1.680.000 đồng.
- Bé 3 tuổi thuộc diện dưới 5 tuổi nên được miễn phí (0 đồng).
- Tổng tiền vé trước khi giảm giá của nhóm là: 6.000.000 + 1.680.000 + 0 = 7.680.000 đồng.
- Phân tích để xác định nhóm giảm giá:
-Theo quy tắc tính giá, nhóm có từ 5 người lớn trở lên được giảm 5% trên tổng tiền vé (bao gồm tiền người lớn và tiền trẻ em). Do nhóm có đúng 5 người lớn nên đủ điều kiện hưởng mức giảm 5%.
- Số tiền được giảm là: 7.680.000 × 5% = 384.000 đồng.
- Tiền vé sau khi giảm giá là: 7.680.000 - 384.000 = 7.296.000 đồng.
- Xác định và tính phụ thu khi có người chọn ghế ưu tiên:
- Theo quy định, phụ thu khu ghế ưu tiên là 300.000 đồng/người và khoản phụ thu này không được áp dụng giảm giá. Trong nhóm có 1 người lớn chọn khu ghế ưu tiên nên tiền phụ thu là: 1 × 300.000 = 300.000 đồng.
- Tính tổng tiền của nhóm:
- Áp dụng công thức Tổng tiền = Tiền vé sau giảm + Phụ thu: 7.296.000 + 300.000 = 7.596.000
- đồng.7.596.000 đồng
```

**Link trò chuyện: https://share.gemini.google/zHqVCImlpflv**

### b) Kiểm tra kết quả AI

Đúng. 

## 4.4. Dây chuyền xử lý khiếu nại – kết quả Trạm 1

**KET QUA AI**

```json
{
  "loai_su_co": "sai_khu_vuc",
  "so_khach": 2,
  "so_hiep_bi_anh_huong": 2,
  "tom_tat": "2 khán giả vé SVT bị xếp khu không mái 2 hiệp đầu, ghế ướt do mưa."
}

```

**Link trò chuyện: https://share.gemini.google/15p8mDCP16m8**

## 4.5. Prompt chấm bài theo Rubric

**KET QUA AI**

```text
(Dán câu trả lời của AI vào đây (bấm nút Copy dưới câu trả lời) – xoá dòng này)
```

**Link trò chuyện:**
