---
layout: post
title: "System design cho người mới — đừng overcomplicate"
date: 2024-09-05 21:00:00 +0700
categories: coding
---

Có một thứ mình thấy trong giới dev Việt Nam: nhiều người thích nói về microservices, Kafka, Kubernetes ngay cả khi sản phẩm của họ có 100 users.

Mình từng là người đó.

Hồi làm side project, mình thiết kế một kiến trúc microservices hoành tráng: 5 services riêng biệt, message queue, API gateway, service mesh. Mất 3 tuần setup infrastructure.

Rồi mình mất hứng và bỏ dự án trước khi viết được business logic.

Bài học: **complexity phải match với scale thực tế.**

Cho 90% sản phẩm giai đoạn đầu, một monolith đơn giản với database tốt là đủ. Không cần microservices. Không cần message queue. Chỉ cần code chạy được và user dùng được.

Martin Fowler có câu: *"Don't even consider microservices unless you have a system that's too complex to manage as a monolith."*

Khi nào scale đến điểm cần tách? Khi bạn biết chỗ nào là bottleneck thực sự. Không phải đoán trước.

**YAGNI — You Ain't Gonna Need It.** Đây là nguyên tắc mình nhắc mình mỗi khi bắt đầu nghĩ đến "nhưng nếu sau này cần thì sao".

Sau này sẽ tính sau. Bây giờ cứ ship đã.
