# 03 — Individual Reflection

**Học viên:** Dương Mạnh Phong — 2A202601557

---

## 1. Vai trò trong nhóm

Ở buổi hội tụ Phase 3, mình có mặt và pitch candidate của mình (tổng hợp notes ôn tập / đối chiếu bài nộp với rubric). Candidate cuối cùng nhóm chọn — "nhân viên nghiệp vụ phải chờ vài ngày để nhận số liệu bán hàng/tồn kho từ đội Data" — không phải ý của mình, nhưng khi nghe nhóm trình bày mình thấy nó có actor rõ hơn (Sales, Sales Operations, Data Analyst) và ảnh hưởng nhiều người hơn candidate cá nhân của mình, vốn chỉ gói gọn trong trải nghiệm của một học viên.

Phần mình đóng góp nhiều nhất là **viết và phản biện Problem Statement** (Phase 5.3 và 6.2). Mình là người rà lại xem field Impact và Boundary đã đủ cụ thể chưa, và cũng là người nhắc nhóm ghi rõ baseline "2-3 ngày" chỉ là ước lượng chứ chưa có ticket log thật — điều này sau đó thể hiện trong ghi chú ở đầu group-report ("chưa có biên bản pitch các candidate còn lại, interview, survey hoặc ticket log").

## 2. Cách dùng AI

Ở phần scan cá nhân, mình tự liệt kê các việc lặp lại/tốn thời gian trong tuần trước, sau đó dùng AI để hỏi thêm góc nhìn theo 4 lăng kính. AI gợi ý thêm được vài ý như "tìm tài liệu cũ" và "theo dõi deadline nhiều nguồn" — hai ý này giúp mình nhớ lại và viết cụ thể hơn cho problem #1 và #8. Nhưng có ý AI đưa ra kiểu "trợ lý học tập AI toàn năng" thì mình bỏ, vì nó không gắn với một workflow cụ thể nào mình từng trải qua, chỉ nghe hay chứ không phải pain thật.

Ở phần group-report, khi phản biện Problem Statement, việc dùng AI để hỏi ngược "field Impact đã có con số chưa, Boundary đã nói rõ AI KHÔNG được làm gì chưa" giúp nhóm phát hiện ra baseline "2-3 ngày" đang bị viết như một sự thật trong khi thực ra là giả định — nhóm phải sửa lại thành "giả thuyết baseline, không phải kết quả đo". Đây là lúc AI đóng vai trò phản biện hữu ích, chứ không tự quyết định gì thay nhóm.

Có một điểm mình còn phân vân: khi so sánh Rule/Workflow/Agent, ban đầu hướng "Agent tự chọn nguồn, tự lập kế hoạch nhiều query" nghe khá hấp dẫn vì linh hoạt hơn. Nhưng nhóm (và cả phần phản biện của AI) chỉ ra rủi ro về quyền truy cập rộng, khó audit, blast radius lớn khi chưa có baseline và golden set — nên nhóm quyết định dừng ở mức Workflow, không chọn Agent.

## 3. Học được gì

So với candidate cá nhân của mình (workflow đơn giản, rủi ro thấp, chỉ ảnh hưởng một người), candidate nhóm chọn phức tạp hơn hẳn: nhiều actor (Sales, Sales Operations, Data Analyst), cần Semantic RAG, SQL Guardrails, và có rủi ro thật về bảo mật dữ liệu nếu policy sai. Điều này dạy mình rằng một bài toán "nghe hợp lý" ở mức cá nhân không tự động scale lên mức tổ chức — càng nhiều actor thì càng cần nhiều lớp kiểm soát (rule/guardrail) trước khi nghĩ đến mức tự động cao hơn.

Trước lab này, nếu là mình một mình, có lẽ mình sẽ có xu hướng chốt nhanh hơn kiểu "cứ thử AI xem sao". Nhưng sau khi đi qua Phase 4-6 với nhóm, mình thấy phần khó nhất không phải là "AI có làm được không" mà là "có đủ dữ liệu và người chịu trách nhiệm để tin vào kết quả AI đưa ra không" — đây là bài học lớn nhất với mình từ lab này.

## 4. Nếu làm lại sẽ đổi gì

Cảm giác chung của mình: mặc dù hiểu lý do nhóm quyết định **Not Yet** (chưa có baseline đo thật, chưa có curated data mart/semantic model, chưa chỉ định được Data Owner), mình vẫn thấy nhóm hơi quá thận trọng. Với những câu hỏi "phổ biến, KPI đã định nghĩa sẵn" (nhóm A trong bảng phân loại ticket), mình nghĩ có thể pilot ngay ở mức Rule/template cho nhóm câu hỏi hẹp đó trong lúc song song đi validate phần còn lại, thay vì để cả bài toán đứng yên chờ đủ điều kiện.

Nếu làm lại từ đầu, mình sẽ ép nhóm có ít nhất một nguồn dữ liệu thật trước khi bước sang Phase 5, thay vì đào sâu workflow trên một baseline chưa kiểm chứng.
