---
layout: post
title: "Code review — nghệ thuật nhận xét mà không làm người ta buồn"
date: 2024-04-10 20:00:00 +0700
categories: coding
---

Hôm nay mình review PR của một bạn intern mới vào team.

Nhìn vào code, mình thấy nhiều chỗ có thể cải thiện: naming convention không nhất quán, một vài chỗ logic có thể đơn giản hơn, thiếu error handling ở một số case quan trọng.

Câu hỏi mình tự hỏi trước khi gõ comment: *"Mình muốn bạn ấy học, hay mình muốn chứng minh mình biết nhiều hơn?"*

Đây là sự khác biệt giữa code review giúp người và code review làm người sợ.

Một vài nguyên tắc mình đang thực hành:

**Khen trước khi chỉ ra vấn đề.** Tìm ít nhất một điều làm tốt và nói ra. Không phải khen xã giao mà là khen thật.

**Giải thích tại sao, không chỉ nói phải làm gì.** Thay vì *"Đổi tên biến này"* thì viết *"Tên biến `x` không rõ nghĩa, đặt là `userAge` sẽ giúp người đọc hiểu ngay không cần đọc context."*

**Dùng câu hỏi thay vì câu mệnh lệnh.** *"Bạn đã nghĩ đến trường hợp null ở đây chưa?"* nhẹ hơn *"Thiếu null check."*

**Phân biệt blocking và non-blocking.** Không phải comment nào cũng là lý do để từ chối merge. Ghi rõ `[blocking]` hay `[suggestion]`.

Code review là kỹ năng mềm quan trọng nhất trong công việc lập trình nhóm. Mình vẫn đang học.
