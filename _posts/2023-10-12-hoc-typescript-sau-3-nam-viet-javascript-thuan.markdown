---
layout: post
title: "Học TypeScript sau 3 năm viết JavaScript thuần"
date: 2023-10-12 20:00:00 +0700
categories: coding
---

*"Mày học TypeScript chưa? Bây giờ không biết TypeScript là tụt hậu rồi đó."*

Câu đó của thằng bạn làm mình quyết định ngồi vào học TypeScript — dù trước đó mình đã trì hoãn hơn một năm.

Ba ngày đầu mình muốn bỏ cuộc. Cái cảm giác viết `const name: string = "Son"` thay vì `const name = "Son"` nghe vô nghĩa lắm. Trình biên dịch cứ đỏ gạch chân khắp nơi. Mình gọi nó là "TypeScript cà khịa".

Nhưng đến tuần thứ hai, mọi thứ bắt đầu click.

Cái lúc mình viết một function nhận vào một object phức tạp, và IDE tự gợi ý đúng các property — lúc đó mình mới hiểu TypeScript không phải để làm khó mình, mà để giúp mình.

Sau 2 tháng: mình không muốn quay lại JS thuần nữa.

Một vài điều mình ước biết sớm hơn:
- `any` là kẻ thù. Tránh xa.
- `interface` và `type` gần như giống nhau nhưng có khác biệt tế nhị — học kỹ phần này.
- Đừng cố type hết mọi thứ ngay từ đầu. Để TypeScript infer khi có thể.

Công nghệ thay đổi nhanh. Nhưng cái mindset "viết code an toàn, rõ ràng" thì không bao giờ lỗi thời.
