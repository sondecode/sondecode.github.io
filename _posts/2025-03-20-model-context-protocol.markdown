---
layout: post
title: "Model context protocol — AI bắt đầu kết nối với thế giới thật"
date: 2025-03-20 21:00:00 +0700
categories: ai
---

MCP — Model Context Protocol. Anthropic release cái này cuối 2024 và mình chỉ bắt đầu thực sự hiểu nó gần đây.

Bình thường, LLM bị giới hạn trong context window của nó. Bạn cho vào text, nó trả ra text. Không biết gì về thế giới ngoài những gì bạn paste vào.

MCP thay đổi điều đó bằng cách cho phép LLM **kết nối với tools bên ngoài** một cách chuẩn hoá: đọc file hệ thống, query database, gọi API, mở browser, chạy code.

Mình setup thử MCP server cho Claude Desktop kết nối với filesystem và một PostgreSQL database local.

Rồi mình hỏi: *"Trong folder projects của tôi, dự án nào có nhiều TODO comment nhất?"*

Nó tự đọc files, đếm, trả lời. Mình không làm gì.

Đây là bước quan trọng hơn nhiều người nghĩ. Trước đây AI là "oracle" — bạn hỏi, nó trả lời từ bộ nhớ. Với MCP, AI bắt đầu trở thành **agent** — nó có thể tương tác với môi trường thực.

Khả năng ứng dụng: AI assistant biết codebase của bạn thực sự, AI có thể tự query database để trả lời câu hỏi business, AI có thể tự động hoá workflows phức tạp.

Ecosystem đang phát triển nhanh. Đây là thứ mình đang theo dõi sát nhất năm 2025.
