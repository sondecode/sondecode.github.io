---
layout: post
title: "Database index — thứ nhỏ tạo ra sự khác biệt khổng lồ"
date: 2025-04-15 21:30:00 +0700
categories: coding
---

Query của mình chạy mất 8 giây.

8 giây. Với một bảng chỉ có 100k records.

Lead nhìn vào SQL rồi hỏi: *"Em có index trên cột này chưa?"*

Mình không biết index là gì. Mình trả lời: *"Chưa ạ."*

Lead thêm một dòng:

```sql
CREATE INDEX idx_users_email ON users(email);
```

Query chạy trong 0.02 giây.

Mình ngồi nhìn màn hình không tin vào mắt mình. Từ 8 giây xuống 0.02 giây chỉ vì một dòng.

Từ đó mình học nghiêm túc về database optimization. Những thứ mình thấy quan trọng nhất:

**Index là mục lục của sách.** Không có mục lục, tìm một từ phải đọc từ đầu đến cuối. Có mục lục, nhảy thẳng đến trang đúng.

**Không phải cột nào cũng cần index.** Index chiếm không gian và làm chậm write operations. Index ở đúng chỗ thì tốt, index vô tội vạ thì tệ hơn không có.

**EXPLAIN ANALYZE là người bạn tốt nhất.** Luôn dùng nó để hiểu query plan trước khi optimize.

Bài học lớn hơn: performance problem thường có root cause đơn giản. Đừng vội add cache, đừng vội thay đổi architecture — kiểm tra cơ bản trước.
