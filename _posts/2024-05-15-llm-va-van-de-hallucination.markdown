---
layout: post
title: "LLM và vấn đề hallucination — khi AI tự tin mà sai"
date: 2024-05-15 21:30:00 +0700
categories: ai
---

Tuần trước mình dùng ChatGPT để tra một API endpoint của một thư viện. Nó cho mình đoạn code trông rất đúng, có format đẹp, có comment rõ ràng.

Mình copy vào, chạy — lỗi ngay. Đi kiểm tra documentation thật, function đó không tồn tại.

ChatGPT đã **hallucinate** — tạo ra thông tin trông thuyết phục nhưng hoàn toàn sai.

Đây là vấn đề cơ bản của LLM hiện tại. Model không "biết" theo nghĩa thực sự — nó dự đoán token tiếp theo dựa trên pattern. Khi không có đủ thông tin chính xác, nó vẫn generate ra câu trả lời nghe có vẻ hợp lý.

Điều nguy hiểm: **nó không nói "tôi không biết"**. Nó nói với giọng tự tin như thể biết chắc.

Cách mình phòng tránh:
- Không bao giờ tin code AI generate mà không test
- Với thông tin factual (API, version, tên function), luôn cross-check với official docs
- Dùng AI tốt nhất cho "understand concept" và "explore ideas", không phải nguồn truth tuyệt đối

AI là công cụ rất mạnh. Nhưng công cụ mạnh cần dùng đúng cách. Người dùng naive nhất là người tin tất cả mọi thứ AI nói.

Tư duy phản biện vẫn là kỹ năng không thể thay thế.
