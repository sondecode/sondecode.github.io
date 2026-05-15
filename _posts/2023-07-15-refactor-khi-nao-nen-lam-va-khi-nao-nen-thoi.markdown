---
layout: post
title: "Refactor — khi nào nên làm và khi nào nên thôi"
date: 2023-07-15 19:30:00 +0700
categories: coding
---

Có một câu nói nổi tiếng trong ngành: *"If it ain't broke, don't fix it."*

Mình từng ghét câu này. Bây giờ mình hiểu nó hơn.

Tuần trước mình dành 2 ngày để refactor một module cũ. Không ai yêu cầu. Mình tự thấy code xấu nên muốn làm lại cho đẹp. Kết quả: module đó đẹp hơn thật, nhưng introduce 3 bug mới mà mình mất thêm 1 ngày để fix.

Sprint đó mình trễ deadline.

Bài học xương máu: **refactor phải có lý do cụ thể.**

Mình bây giờ chỉ refactor khi:
1. Code đó đang gây bug thực sự
2. Code đó cần thêm feature mới và cấu trúc hiện tại cản trở
3. Code đó được review và team thống nhất là technical debt cần giải quyết

Refactor vì "nhìn xấu" hay "mình muốn dùng pattern mới" — đó là lý do của tác giả, không phải của business.

Sự thật khó nghe: **code không cần đẹp, code cần chạy đúng và maintain được.** Đẹp là bonus.

Mình vẫn đang học để cân bằng giữa perfectionism và pragmatism. Chưa xong nhưng đang tiến bộ.
