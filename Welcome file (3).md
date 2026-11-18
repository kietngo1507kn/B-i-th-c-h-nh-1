## I. Mẫu Prompt Thiết Kế (Prompt Template)

Bạn có thể sử dụng mẫu prompt dưới đây để giao nhiệm vụ cho AI:

Plaintext

```
Bạn là một chuyên gia lập kế hoạch tài chính cá nhân. Nhiệm vụ của bạn là xây dựng bảng phân bổ ngân sách tháng dựa trên dữ liệu đầu vào dưới đây, đảm bảo kiểm soát chặt chẽ dòng tiền, hoàn thành mục tiêu tiết kiệm tối thiểu và trả nợ đúng hạn.

### Dữ liệu đầu vào:
- Tổng thu nhập tháng (Gross): 25.000.000 VNĐ
- Thuế và khấu trừ bắt buộc: 2.000.000 VNĐ
- Chi phí cố định bắt buộc (Nhà, điện, nước, viễn thông): 6.000.000 VNĐ
- Các khoản nợ cần trả tối thiểu: 4.000.000 VNĐ
- Mục tiêu tiết kiệm tối thiểu: 5.000.000 VNĐ

### Quy tắc xử lý & Kỷ luật tính toán:
Hãy suy nghĩ từng bước một và tính toán chi tiết trước khi đưa ra quyết định. Bắt buộc hiển thị đầy đủ các phép tính cộng trừ nhân chia trung gian, không được nhảy cóc ra kết quả cuối cùng. Vạch ra quy trình lập luận gồm 4 bước:
- Bước 1: Tính toán tổng thu nhập khả dụng sau khi trừ thuế và chi phí cố định bắt buộc.
- Bước 2: Phân bổ khoản tiền trả nợ tối thiểu và tính số dư còn lại.
- Bước 3: Trích lập quỹ tiết kiệm theo tỷ lệ cam kết và tính số dư tiếp theo.
- Bước 4: Chia phần còn lại cho chi tiêu linh hoạt.

### Yêu cầu cấu trúc đầu ra:
Trình bày kết quả thành hai phần rõ rệt:
- Phần 1: Nhật ký suy luận logic (Reasoning Steps) trình bày chi tiết từng bước với công thức và con số trung gian.
- Phần 2: Bảng phân bổ ngân sách cuối cùng bằng Markdown Table với các cột: Hạng mục, Số tiền (VNĐ), Tỷ lệ %, Ghi chú. (Đảm bảo tổng tỷ lệ phần trăm bằng chính xác 100.00%).

```

## II. Ví dụ Minh Họa Thực Tế (Execution Demo)

Dưới đây là kết quả mẫu khi AI thực thi prompt trên theo đúng các ràng buộc kỹ thuật:

### Phần 1: Nhật ký suy luận logic (Reasoning Steps)

-   **Dữ liệu ban đầu:**
    
    -   Tổng thu nhập (Gross):  25.000.000 VNĐ25.000.000\text{ VNĐ}25.000.000 VNĐ
        
    -   Thuế & khấu trừ bắt buộc:  2.000.000 VNĐ2.000.000\text{ VNĐ}2.000.000 VNĐ
        
    -   Chi phí cố định bắt buộc:  6.000.000 VNĐ6.000.000\text{ VNĐ}6.000.000 VNĐ
        
    -   Trả nợ tối thiểu:  4.000.000 VNĐ4.000.000\text{ VNĐ}4.000.000 VNĐ
        
    -   Quỹ tiết kiệm tối thiểu:  5.000.000 VNĐ5.000.000\text{ VNĐ}5.000.000 VNĐ
        
-   **Bước 1: Tính tổng thu nhập khả dụng sau thuế và chi phí cố định bắt buộc**
    
    -   Công thức:  Thu nhập sau thueˆˊ=Tổng thu nhập−Thueˆˊ vaˋ khaˆˊu trừ\text{Thu nhập sau thuế} = \text{Tổng thu nhập} - \text{Thuế và khấu trừ}Thu nhập sau thueˆˊ=Tổng thu nhập−Thueˆˊ vaˋ khaˆˊu trừ
        
    -   Phép tính:  25.000.000−2.000.000=23.000.000 VNĐ25.000.000 - 2.000.000 = 23.000.000\text{ VNĐ}25.000.000−2.000.000=23.000.000 VNĐ
        
    -   Công thức:  Soˆˊ dư sau chi phıˊ coˆˊ định=Thu nhập sau thueˆˊ−Chi phıˊ coˆˊ định ba˘ˊt buộc\text{Số dư sau chi phí cố định} = \text{Thu nhập sau thuế} - \text{Chi phí cố định bắt buộc}Soˆˊ dư sau chi phıˊ coˆˊ  định=Thu nhập sau thueˆˊ−Chi phıˊ coˆˊ  định ba˘ˊt buộc
        
    -   Phép tính trung gian:  23.000.000−6.000.000=17.000.000 VNĐ23.000.000 - 6.000.000 = 17.000.000\text{ VNĐ}23.000.000−6.000.000=17.000.000 VNĐ
        
-   **Bước 2: Phân bổ khoản tiền trả nợ tối thiểu và tính số dư**
    
    -   Khoản trả nợ tối thiểu:  4.000.000 VNĐ4.000.000\text{ VNĐ}4.000.000 VNĐ
        
    -   Công thức:  Soˆˊ dư sau trả nợ=Soˆˊ dư ở Bước 1−Trả nợ toˆˊi thiểu\text{Số dư sau trả nợ} = \text{Số dư ở Bước 1} - \text{Trả nợ tối thiểu}Soˆˊ dư sau trả nợ=Soˆˊ dư ở Bước 1−Trả nợ toˆˊi thiểu
        
    -   Phép tính trung gian:  17.000.000−4.000.000=13.000.000 VNĐ17.000.000 - 4.000.000 = 13.000.000\text{ VNĐ}17.000.000−4.000.000=13.000.000 VNĐ
        
-   **Bước 3: Trích lập quỹ tiết kiệm theo tỷ lệ cam kết**
    
    -   Quỹ tiết kiệm mục tiêu:  5.000.000 VNĐ5.000.000\text{ VNĐ}5.000.000 VNĐ
        
    -   Công thức:  Soˆˊ dư sau tieˆˊt kiệm=Soˆˊ dư ở Bước 2−Quy˜ tieˆˊt kiệm\text{Số dư sau tiết kiệm} = \text{Số dư ở Bước 2} - \text{Quỹ tiết kiệm}Soˆˊ dư sau tieˆˊt kiệm=Soˆˊ dư ở Bước 2−Quy˜​ tieˆˊt kiệm
        
    -   Phép tính trung gian:  13.000.000−5.000.000=8.000.000 VNĐ13.000.000 - 5.000.000 = 8.000.000\text{ VNĐ}13.000.000−5.000.000=8.000.000 VNĐ
        
-   **Bước 4: Chia phần còn lại cho chi tiêu linh hoạt (quy tắc 50/30/20 cải tiến)**
    
    -   Phần còn lại sau khi hoàn tất các nghĩa vụ cố định, nợ và tiết kiệm chính là ngân sách chi tiêu linh hoạt (ăn uống, giải trí, phát sinh).
        
    -   Phép tính:  8.000.000 VNĐ8.000.000\text{ VNĐ}8.000.000 VNĐ
        
    -   Kiểm tra tính đúng đắn tổng tiền:Tổng=2.000.000+6.000.000+4.000.000+5.000.000+8.000.000=25.000.000 VNĐ\text{Tổng} = 2.000.000 + 6.000.000 + 4.000.000 + 5.000.000 + 8.000.000 = 25.000.000\text{ VNĐ}Tổng=2.000.000+6.000.000+4.000.000+5.000.000+8.000.000=25.000.000 VNĐ (Khớp 100% tổng thu nhập).
        
-   **Kiểm tra tính tỷ lệ % (Tính trên Tổng thu nhập 25.000.000 VNĐ):**
    
    -   Thuế & Khấu trừ:  2.000.00025.000.000×100%=8.00%\frac{2.000.000}{25.000.000} \times 100\% = 8.00\%25.000.0002.000.000​×100%=8.00%
        
    -   Chi phí cố định:  6.000.00025.000.000×100%=24.00%\frac{6.000.000}{25.000.000} \times 100\% = 24.00\%25.000.0006.000.000​×100%=24.00%
        
    -   Trả nợ tối thiểu:  4.000.00025.000.000×100%=16.00%\frac{4.000.000}{25.000.000} \times 100\% = 16.00\%25.000.0004.000.000​×100%=16.00%
        
    -   Quỹ tiết kiệm:  5.000.00025.000.000×100%=20.00%\frac{5.000.000}{25.000.000} \times 100\% = 20.00\%25.000.0005.000.000​×100%=20.00%
        
    -   Chi tiêu linh hoạt:  8.000.00025.000.000×100%=32.00%\frac{8.000.000}{25.000.000} \times 100\% = 32.00\%25.000.0008.000.000​×100%=32.00%
        
    -   Tổng tỷ lệ:  8.00%+24.00%+16.00%+20.00%+32.00%=100.00%8.00\% + 24.00\% + 16.00\% + 20.00\% + 32.00\% = 100.00\%8.00%+24.00%+16.00%+20.00%+32.00%=100.00%
        

### Phần 2: Bảng phân bổ ngân sách cuối cùng


Ghi chú |Số tiền (VNĐ) |Tỷ lệ % | Ghi chú |
|--|--|--|--| 
|**Thuế & Khấu trừ bắt buộc**|  2.000.000|8,00% | Trừ trực tiếp trước khi nhận lương|
| **Chi phí cố định** |6.000.000|24,00%|Tiền nhà, điện, nước, internet|
|**Trả nợ tối thiểu**|4.000.000|16,00%|Đảm bảo không bị phạt quá hạn|
|**Quỹ tiết kiệm**|5.000.000|20,00%|Đạt mục tiêu tối thiểu (20%+)|
|**Chi tiêu linh hoạt**|8.000.000|32,00%|Ăn uống, di chuyển, giải trí, phát sinh|
|**Tổng cộng**|25.000.000|100,00%|Cân đối thu - chi hoàn hảo|
