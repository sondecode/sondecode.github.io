---
layout: post
title: "RAG là gì và tại sao mình thấy nó quan trọng hơn fine-tuning"
date: 2024-02-08 20:30:00 +0700
categories: ai
---

Khi mới tiếp cận thế giới LLM, mình cứ nghĩ để AI "biết" thêm thông tin thì phải fine-tune model. Train lại, tốn tiền, tốn thời gian.

Rồi mình đọc về **RAG — Retrieval-Augmented Generation** và mọi thứ thay đổi.

Ý tưởng cực kỳ đơn giản:
1. Bạn có một kho tài liệu riêng (docs nội bộ, FAQ, database...)
2. Khi user hỏi, hệ thống tìm kiếm những đoạn văn liên quan nhất từ kho đó
3. Nhét những đoạn đó vào context của LLM cùng với câu hỏi
4. LLM trả lời dựa trên cả câu hỏi lẫn context vừa tìm được

Không cần train lại model. Không cần GPU. Thêm tài liệu mới thì chỉ cần index thêm vào vector database.

Mình đã thử build một chatbot nội bộ nhỏ cho team dùng RAG. User có thể hỏi về document của project và nó trả lời đúng đến mức mọi người tưởng có người trực 24/7.

Chi phí thực tế: khoảng $5/tháng tiền API.

Đây là kiến trúc mình thấy practical nhất cho 80% use case "AI + dữ liệu riêng" trong doanh nghiệp. Không cần phức tạp hoá.
