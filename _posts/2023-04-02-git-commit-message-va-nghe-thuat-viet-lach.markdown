---
layout: post
title: "Git commit message và nghệ thuật viết lách"
date: 2023-04-02 21:00:00 +0700
categories: coding
---

Hôm nay lead review PR của mình và comment một câu: *"Commit message của em viết như ghi vội nhắn tin, anh không hiểu cái này fix cái gì."*

Nhìn lại lịch sử commit thì thấy ngại thật:

```
fix bug
update
wip
fix again
ok done
final
final 2
FINAL ACTUALLY FINAL
```

Mình nghĩ mình không phải người duy nhất làm vậy.

Nhưng sau khi bị lead nhắc, mình bắt đầu đọc về **Conventional Commits** và thấy nó hay hơn mình tưởng. Format đơn giản: `type(scope): description`. Ví dụ:

- `fix(auth): handle null token on login`
- `feat(profile): add avatar upload`
- `docs(readme): update setup instructions`

Nhìn lại lịch sử repo sau một tuần áp dụng thấy rõ ràng hẳn. Biết ngay cái gì thay đổi, thay đổi ở đâu, vì sao.

Mình cũng nhận ra: viết commit message tốt cũng giống viết văn — phải rõ ràng, súc tích, và nghĩ đến người đọc. Người đọc ở đây là đồng nghiệp tương lai, hoặc chính mình sau 3 tháng.

Kỹ năng tưởng nhỏ nhưng nó phân biệt người code nghiêm túc và người chỉ làm cho xong.
