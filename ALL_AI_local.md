# 🚀 AI LOCAL VỚI OLLAMA - TỔNG HỢP LỆNH CÀI, TẢI, CHẠY, SỬ DỤNG

---

# 1. CÀI OLLAMA

Truy cập:

https://ollama.com/download

Tải về và cài đặt như phần mềm bình thường.

Kiểm tra đã cài thành công chưa:

```bash
ollama --version
```

---

# 2. TẢI MODEL AI

## Tải Gemma4 bản thường

```bash
ollama pull gemma4
```

---

## Tải Gemma4 bản mạnh hơn

```bash
ollama pull gemma4:31b
```

---

## Tải thêm một số model khác

### Llama3

```bash
ollama pull llama3
```

### Mistral

```bash
ollama pull mistral
```

### Qwen

```bash
ollama pull qwen
```

### Phi

```bash
ollama pull phi
```

---

# 3. CHẠY MODEL AI

## Chạy Gemma4

```bash
ollama run gemma4
```

---

## Chạy Gemma4 31B

```bash
ollama run gemma4:31b
```

---

## Chạy Llama3

```bash
ollama run llama3
```

---

## Chạy Mistral

```bash
ollama run mistral
```

---

# 4. CHAT VỚI AI

Sau khi chạy:

```bash
ollama run gemma4
```

terminal sẽ hiện:

```bash
>>>
```

gõ câu hỏi trực tiếp:

```bash
>>> viết code java đăng nhập mysql
>>> giải thích thuật toán bubble sort
>>> tạo website html css
```

AI sẽ trả lời ngay.

---

# 5. THOÁT KHỎI AI

```bash
/bye
```

hoặc:

```bash
Ctrl + C
```

---

# 6. XEM DANH SÁCH MODEL ĐÃ TẢI

```bash
ollama list
```

---

# 7. XEM THÔNG TIN MODEL

```bash
ollama show gemma4
```

---

# 8. XÓA MODEL

```bash
ollama rm gemma4
```

hoặc:

```bash
ollama rm gemma4:31b
```

---

# 9. TẢI LẠI / UPDATE MODEL

```bash
ollama pull gemma4
```

gõ lại lệnh pull sẽ tự cập nhật nếu có phiên bản mới.

---

# 10. CHẠY AI KHÔNG CẦN INTERNET

Sau khi đã tải model:

```bash
ollama pull gemma4
```

thì có thể tắt wifi và vẫn chạy:

```bash
ollama run gemma4
```

---

# 11. DÙNG AI 1 CÂU LỆNH KHÔNG CẦN VÀO CHAT MODE

```bash
ollama run gemma4 "viết code c# quản lý sinh viên"
```

AI sẽ trả lời luôn một lần.

---

# 12. CHẠY API LOCALHOST CHO DEV

Mở server ollama:

```bash
ollama serve
```

API local mặc định:

```bash
http://localhost:11434
```

Test bằng browser:

```bash
http://localhost:11434/api/tags
```

---

# 13. GỌI API TỪ CODE

## Ví dụ Python

```python
import requests

url = "http://localhost:11434/api/generate"

data = {
    "model": "gemma4",
    "prompt": "Viết code Python quản lý sinh viên"
}

response = requests.post(url, json=data)

print(response.text)
```

---

# 14. CÁC MODEL NÊN DÙNG

| Model | Lệnh tải | Mục đích |
|-------|----------|----------|
| Gemma4 | ollama pull gemma4 | đa năng |
| Gemma4:31b | ollama pull gemma4:31b | mạnh hơn |
| Llama3 | ollama pull llama3 | chat tốt |
| Mistral | ollama pull mistral | nhẹ |
| Qwen | ollama pull qwen | code ổn |
| Phi | ollama pull phi | máy yếu |

---

# 15. THƯ MỤC MODEL ĐƯỢC LƯU

Windows:

```bash
C:\Users\TênUser\.ollama\models
```

---

# 16. TOÀN BỘ LỆNH OLLAMA NHANH

```bash
ollama --version
ollama pull gemma4
ollama pull gemma4:31b
ollama pull llama3
ollama run gemma4
ollama run gemma4:31b
ollama run llama3
ollama list
ollama show gemma4
ollama rm gemma4
ollama serve
```

---

# 17. QUY TRÌNH SỬ DỤNG NHANH

## Lần đầu:

```bash
ollama pull gemma4
```

## Sau đó chạy:

```bash
ollama run gemma4
```

## Gõ prompt:

```bash
>>> viết code php login
```

## Thoát:

```bash
/bye
```

---

# DONE ✅

Máy tính lúc này đã trở thành AI local offline.
