---
layout: post
title: "Tôi đã build một app nhỏ với GPT-4 API trong một tuần"
date: 2023-11-18 22:00:00 +0700
categories: ai
---

Tuần trước mình build xong một cái app nho nhỏ: người dùng nhập vào một đoạn text tiếng Việt lộn xộn, app sẽ trả về bản được tổ chức lại thành cấu trúc rõ ràng — dạng bullet points, headers, và summary.

Nghe phức tạp nhưng thực ra chỉ là:

1. Frontend React đơn giản
2. Backend Express.js nhận text input
3. Gọi GPT-4 API với một system prompt được viết kỹ
4. Trả về kết quả cho frontend

Tổng cộng khoảng 300 dòng code thực sự. Mình build trong khoảng 5-6 tiếng tổng cộng trong tuần.

**Thứ tốn thời gian nhất không phải là code — mà là viết prompt.**

Mình mất hơn 2 tiếng để iterate cái system prompt cho đến khi output đủ nhất quán. Thay một từ, output thay đổi kiểu khác. Thêm một câu ví dụ, accuracy tăng hẳn.

Prompt engineering thực sự là một kỹ năng. Không phải ai cũng biết.

App này mình chưa release vì chưa xử lý rate limiting và cost control. Nhưng bài học quan trọng nhất: **với LLM API, sản phẩm nhanh hơn bạn nghĩ rất nhiều. Bottleneck là ý tưởng và prompt, không phải code.**
