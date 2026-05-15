---
layout: post
title: "Viết test — thứ mình ghét nhất và bây giờ không thể thiếu"
date: 2024-07-03 20:30:00 +0700
categories: coding
---

Confession: mình đã đi làm 2 năm mà gần như không viết test.

Không phải vì không biết. Là vì không thích. Viết test tốn thêm thời gian, feature đã chạy rồi thì cần gì test thêm, deadline gấp không kịp.

Rồi một ngày mình refactor một module và break một tính năng quan trọng. Không phát hiện ra. Ship lên production. Users báo bug. Mất 2 tiếng fix và 30 phút viết apology cho team.

Hôm đó mình ngồi xuống và viết retrospec cho bản thân: *"Nếu có unit test, cái này đã bị catch ngay lần chạy CI đầu tiên."*

Từ đó mình thay đổi.

Mình không cố viết 100% test coverage — đó là unrealistic với team nhỏ. Mình áp dụng nguyên tắc **"test những gì quan trọng"**:

- Business logic cốt lõi? Test kỹ.
- Edge cases đã từng gây bug? Test hết.
- Utility function đơn giản? Có thể skip.

Sau 3 tháng, mình nhận ra viết test không làm mình chậm hơn. Nó làm mình **tự tin hơn khi thay đổi code**. Đó là thứ quan trọng hơn.

Testing không phải overhead. Testing là safety net. Và mình cần safety net vì mình không phải người hoàn hảo.
