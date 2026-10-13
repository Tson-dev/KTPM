**Bên dưới là nội dung markdown được covert từ pdf gốc**

**CỘNG HÒA XÃ HỘI CHỦNGHĨA VIỆT NAM Độc lập - Tựdo - Hạnh phúc** 

TRƯỜNG ĐẠI HỌC ĐÀ LẠT **KHOA CÔNG NGHỆTHÔNG TIN** 

# **HƯỚNG DẪN THỰC HIỆN ĐỀTÀI MÔN KIỂM THỬPHẦN MỀM Giảng viên: Nguyễn ThếLâm** 

## **1. Mục tiêu đềtài** 

Đềtài cuối kỳđược thiết kếnhằm giúp sinh viên: 

-  Trực tiếp tiếp cận, đọc hiểu kiến trúc và thiết lập môi trường chạy cho các hệthống phần mềm thực tế(có độphức tạp cao, đang được sửdụng rộng rãi). 

-  Vượt ra ngoài các bài kiểm thửcơ bản đểnghiên cứu và triển khai một trong các kỹthuật kiểm thửnâng cao (Property-Based Testing, Mutation Testing, Fuzzing,...). 

-  Tổchức làm việc nhóm theo quy trình phát triển phần mềm chuẩn mực (sửdụng Git, công cụ quản lý Task như Jira/Trello, viết báo cáo kỹthuật và phân vai rõ ràng). 

## **2. Nội dung thực hiện yêu cầu** 

### **2.1. Nội dung đềtài** 

Mỗi nhóm cần hoàn thành **hai phần bắt buộc** tương ứng với 2 giai đoạn của dựán. 

### **Phần 1: Phân tích hệthống và thiết lập môi trường (System Analysis & Setup)** 

Nhóm sẽchọn 1 dựán (Repo) từdanh sách được cung cấp. Tại bước này, nhóm đóng vai trò như các kỹsư QA mới tham gia dựán (on-boarding). 

 Nhiệm vụ: 

- Đọc hiểu cấu trúc mã nguồn, nhận diện các module/dependency chính. 

- Phân tích và vẽlại kiến trúc hệthống, luồng dữliệu (Data flow) của 3-5 nghiệp vụtrọng tâm. 

- Cài đặt hệthống chạy thành công trên máy cá nhân (Local) hoặc qua Docker. 

- Lập tài liệu hướng dẫn cài đặt (Môi trường, runtime, biến môi trường, lệnh build/run, seed data). 

1 

### **Phần 2: Ứng dụng kỹthuật kiểm thửnâng cao (Advanced Testing Implementation)** 

Nhóm chọn 1 kỹthuật kiểm thửnâng cao từdanh sách đểáp dụng vào hệthống đã setup ởPhần 1. 

 Nhiệm vụ: 

- Nghiên cứu cơ sởlý thuyết, giới hạn và tiêu chí áp dụng của kỹthuật đã chọn. 

- Thiết kếKịch bản kiểm thử(Test Model / Test Scenarios / Test Cases) tập trung vào các luồng nghiệp vụcốt lõi hoặc module tiềm ẩn nhiều rủi ro nhất. 

- Triển khai viết mã kiểm thửtựđộng (Automation Script / Harness). 

- Chạy kiểm thử, thu thập Log/Metrics, phát hiện lỗi (Defect) hoặc chứng minh độbao phủ (Coverage/Score), sau đó tiến hành phân tích nguyên nhân cốt lõi (Root Cause Analysis). 

### **2.2. Quy định vềnhóm** 

**Quy mô nhóm:** 3 - 5 sinh viên/nhóm. 

**Hình thức:** Làm việc nhóm theo mô hình Agile/Scrum. Mỗi nhóm đóng vai trò là một "Đội Đảm bảo Chất lượng"(QA Team) độc lập, tiếp nhận và kiểm thửmột dựán mã nguồn mởthực tế. **Nguyên tắc chọn đềtài:** Hai nhóm không thểchọn chung cùng một tổhợp [Dựán (Repo) + Kỹ thuật kiểm thử]. Mỗi tổhợp Repo + Kỹthuật chỉcho phép tối đa 01 nhóm đăng ký thực hiện. 

#### **Cách thức đăng ký:** 

-  Các nhóm gửi đềtài đăng ký theo mẫu (mỗi nhóm gửi tối đa 3 đềtài là 3 nguyện vọng ưu tiên) vào email: lam.th.ngn@gmail.com. 

-  Trường hợp 2 nhóm chung 1 đềtài, đềtài gửi sớm hơn sẽđược chấp nhận trước, nhóm còn lại sẽ chuyển xuống nguyện vọng 2 hoặc 3 nếu vẫn bịtrùng. 

## **3. Cấu trúc cơ bản cho mọi tổhợp/đềtài** 

Đểđảm bảo các nhóm được đánh giá trên cùng một khung tiêu chuẩn, dù chọn tổhợp Repo và Kỹ thuật nào, các nhóm cũng phải thực hiện và trình bày báo cáo cơ bản theo cấu trúc này: 

-  **Phần A:** Mô tảmục tiêu hệthống, actor/use case chính, cây thư mục/module, dependency và luồng dữliệu. 

-  **Phần B:** Vẽít nhất 01 sơ đồkiến trúc ởmức component/container và giải thích 3-5 module liên quan trực tiếp tới phần kiểm thử. 

-  **Phần C:** Tài liệu hóa môi trường, phiên bản, lệnh build/run, DB/service, seed data; cung cấp bằng chứng hệthống chạy thành công và ít nhất 03 luồng nghiệp vụchạy được. 

-  **Phần D:** Trình bày nguyên lý, lý do chọn phạm vi, giảđịnh, rủi ro và tiêu chí pass/fail của kỹ thuật được chọn. 

-  **Phần E:** Thiết kếTest Model/Scenario/Case hoặc Artefact tương đương theo kỹthuật; chỉrõ input, precondition, expected result/invariant và dữliệu test. 

-  **Phần F:** Chứa mã nguồn test/harness/script có thểchạy lại tựđộng; cung cấp file README chứa lệnh chạy và dependency. 

2 

-  **Phần G:** Log/report/metrics, danh sách lỗi (defect) hoặc hành vi bất thường, và phân tích nguyên nhân; Nếu không tìm thấy lỗi, phải chứng minh coverage/score/threshold đã đạt. 

-  **Phần H:** Lưu cứng (pin) commit/tag của repo, lưu cấu hình test và mô tảcách đểngười khác có thểchạy lại test trên máy mới. 

## **4. Lịch trình và các cột mốc (Milestones)** 

Dựán được quản lý theo dạng các Sprint. Các mốc thời gian cụthể: 

|**Mốc thời gian**|**Sựkiện**|**Yêu cầu cần đạt (Deliverables)**|
|---|---|---|
|**18/9**|**Hạn chót Đăng ký Đề**<br>**tài**|Nhóm chốt danh sách thành viên, Repo đã chọn<br>và Kỹthuật kiểm thửsẽáp dụng. Chốt Commit<br>SHA/Tag của Repo đểcốđịnh phiên bản. Thiết<br>lập xong công cụquản lý dựán (Trello/Jira).|
|**20/10**|**Báo**<br>**cáo**<br>**Giữa**<br>**kỳ**<br>**(Milestone 2)**|Demo hệthống chạy thành công trên máy tính.<br>Trình bày sơ đồkiến trúc, tài liệu on-boarding. Báo<br>cáo kếhoạch áp dụng kỹthuật kiểm thử(Phạm vi<br>test, giảđịnh, tiêu chí đánh giá).|
|**Ngày thi cuối**<br>**kỳ**<br>**theo**<br>**lịch**<br>**nhà**<br>**trường**|**Bảo vệCuối kỳ(Final**<br>**Defense)**|Thuyết trình toàn bộdựán. Demo chạy script au-<br>tomation. Nộp toàn bộmã nguồn kiểm thửvà Báo<br>cáo tổng kết. _(Lưu ý: Báo cáo nộp trước khi bảo_|
|(thường<br>là<br>tháng 12)||_vệ1 tuần)_. Đánh giá chéo (Peer-review) giữa các<br>thành viên.|



**LƯU Ý:** Sinh viên lưu ý quản lý thời gian chặt chẽ. Hệthống mã nguồn mởrất đồsộ, hãy **giới hạn phạm vi (Scope) phù hợp** (ví dụ: chỉkiểm thửmodule thanh toán, luồng duyệt tài liệu...) thay vì ôm đồm toàn bộhệthống. 

## **5. Quy trình làm việc** 

Bài tập lớn khuyến khích các nhóm làm việc có tổchức và phối hợp nhịp nhàng: 

-  Nhóm nên tựphân chia công việc hợp lý (ví dụ: người lo cài đặt môi trường, người viết kịch bản, người code test...). 

-  Nên sửdụng các công cụnhư Trello, Jira hoặc Github Projects đểdễdàng theo dõi tiến độcông việc chung. 

-  Khuyến khích dùng Git đểquản lý mã nguồn. Các ghi chú quan trọng hoặc hướng dẫn chạy code nên được viết tóm tắt trong file README đểcác thành viên khác dễnắm bắt. 

## **6. Yêu cầu báo cáo và tiêu chí đánh giá đềtài nhóm** 

Điểm của đềtài sẽcân nhắc cả **sản phẩm đạt được** và **sựnỗlực, quá trình phối hợp** của nhóm. Dưới đây là một sốtiêu chí tham khảo cho báo cáo và buổi bảo vệ: 

3 

### **A. Đánh giá báo cáo chuyên môn và mã nguồn** 

-  Báo cáo trình bày được mục tiêu hệthống, vẽlại được luồng dữliệu cơ bản ởmức dễhiểu. 

-  Có hướng dẫn cài đặt môi trường rõ ràng đểgiảng viên có thểdựng lại và chạy thử(khuyến khích dùng Docker nếu có thể). 

-  Cho thấy nhóm hiểu được kỹthuật kiểm thửđang áp dụng và biết cách vận dụng vào dựán. 

-  Các kịch bản kiểm thử(scenarios) có mô tảcụthể. Mã nguồn test nên gọn gàng, ưu tiên có thể chạy tựđộng và sinh ra kết quả. 

-  Từkết quảchạy test, nhóm có thểchỉra được lỗi phần mềm (nếu có) hoặc giải thích được ý nghĩa của các log/kết quảthu được. 

### **B. Đánh giá quản trịdựán và thuyết trình** 

-  Có lịch sửcông việc và commit (Git) đểcho thấy sựtham gia đều đặn của các thành viên. 

-  Slide báo cáo có bốcục gọn gàng. Sinh viên trình bày tựtin, dễhiểu và có sựphối hợp tốt khi báo cáo. 

-  Cốgắng trảlời đúng trọng tâm các câu hỏi góp ý từgiảng viên. 

### **C. Đánh giá đóng góp cá nhân (Peer Evaluation)** 

-  Cuối kỳ, nhóm sẽcó phần đánh giá chéo mức độđóng góp của từng thành viên. Điểm cá nhân có thểđược điều chỉnh đôi chút so với điểm chung dựa trên mức độtham gia thực tếvào bài tập lớn. 

4 

## **Phụlục 1: danh sách repo mã nguồn mở** 

### **1.1. Gợi ý chọn repo theo năng lực nhóm** 

-  **Nhóm mới tiếp cận dựán mã nguồn mở:** R01 Spring PetClinic, R02 Mealie, R03 Snipe-IT, R04 nopCommerce. 

-  **Nhóm khá, có kinh nghiệm Docker/web/API:** R05 Cal.com, R06 Directus, R07 Outline, R08 Paperless-ngx, R09 Chatwoot. 

-  **Nhóm mạnh, có thểđọc monorepo/multi-service:** R10 Twenty, R11 Plane, R12 Saleor, R13 Immich, R14 Jellyfin, R15 Mattermost, R16 Appsmith. 

### **1.2. Các lưu ý khi chốt repo** 

-  Khuyến nghịđối với repo quy mô lớn (R09 - R16): Nên khóa phiên bản theo release/tag và cho phép nhóm dùng Docker/Docker Compose. Không nên yêu cầu sinh viên hiểu toàn bộcodebase; chỉcần phân rã 3 - 5 module hoặc luồng chính có liên quan trực tiếp tới phần kiểm thử. 

-  Nên chốt tag/release cụthểvà lưu lại commit SHA trong đềtài đểtránh main branch thay đổi giữa học kỳgây vỡtest. 

-  Yêu cầu nhóm tựlập tài liệu cài đặt từmáy sạch (phiên bản runtime, DB, Docker, biến môi trường, port, seed data và lệnh chạy). 

-  Cho phép giới hạn phạm vi, ví dụchỉkiểm thửmodule booking, checkout, asset checkout, document workflow hoặc một nhóm API. 

-  Một sốdựán dùng AGPL/BSL/custom license. Sinh viên cần đọc kỹfile LICENSE nếu có ý định phân phối lại bản build hoặc mã sửa đổi. Với môn học, nên ưu tiên clone/run/test trong môi trường học tập nội bộ. 

### **1.3. Danh sách chi tiết các repo** 

|**Mã**|**Repo / Lĩnh vực**|**Stack**<br>**&**<br>**Kiến**<br>**trúc**|**Độkhó**|**Nhãn**||**Kỹ**<br>**thuật**|**Ghi chú**|
|---|---|---|---|---|---|---|---|
|**R01**|**spring-**<br>**projects/spring-**<br>**petclinic**<br>Quản<br>lý<br>phòng<br>khám thú y|Java,<br>Spring<br>Boot,<br>Thymeleaf;<br>MySQL/PostgreSQL<br>Testcontainers|;<br>Dễ- vừa<br>_⋆◦◦_|API,<br>DATA|WF,|K01,<br>K03,<br>K06,<br>K08,<br>K16|Rất phù hợp<br>cho nhóm lần<br>đầu đọc mã<br>nguồn mở.|
|**R02**|**mealie-**<br>**recipes/mealie**<br>Quản lý công thức,<br>thực đơn|Python<br>backend<br>+ Vue/TypeScript<br>frontend;<br>REST<br>API|Dễ- vừa<br>_⋆◦◦_|UI,<br><br>WF,<br>DATA|API,|K01,<br>K05,<br>K06,<br>K10,<br>K11|Phạm vi chức<br>năng<br>vừa<br>phải, dễxây<br>dựng<br>test<br>scenario.|
|**R03**|**grokability/snipe-**<br>**it**<br>Quản<br>lý<br>tài<br>sản<br>CNTT|PHP,<br>Laravel<br>12; DB quan hệ;<br>Docker|Vừa<br>_⋆⋆◦_|UI,<br><br>WF,<br>DATA<br>SEC|API,<br>,|K06,<br>K08,<br>K10,<br>K15,<br>K16|Tốt cho kiểm<br>thử<br>phân<br>quyền,<br>dữ<br>liệu biên.|



5 

|**Mã**|**Repo / Lĩnh vực**|**Stack**<br>**&**<br>**Kiến**<br>**trúc**|**Độkhó**|**Nhãn**|**Kỹ**<br>**thuật**|**Ghi chú**|
|---|---|---|---|---|---|---|
|**R04**|**nopSolutions/nop**<br>Thương<br>mại<br>điện<br>tử|**Commerce**<br>C#,<br>ASP.NET<br>Core, SQL Server;<br>kiến trúc plugin|Vừa<br>_⋆⋆◦_|UI,<br>API,<br>WF,<br>DATA,<br>PERF,<br>SEC|K06,<br>K07,<br>K08,<br>K10,<br>K15|Nghiệp<br>vụ<br>phong<br>phú;<br>phù hợp kiểm<br>thử<br>tổ<br>hợp,<br>hiệu năng.|
|**R05**|**calcom/cal.com**<br>Hạ<br>tầng<br>đặt<br>lịch/scheduling|TypeScript,<br>Next.js,<br>Post-<br>greSQL; monorepo|Vừa<br>-<br>khó<br>_⋆⋆◦_|UI,<br>API,<br>WF,<br>DATA,<br>CONC|K02,<br>K05,<br>K06,<br>K10,<br>K15|Đặc biệt phù<br>hợp kiểm thử<br>stateful<br>và<br>concurrency.|
|**R06**|**directus/directus**<br>Headless<br>CMS<br>/<br>data platform|TypeScript/Node.js,<br>Vue;<br>REST<br>&<br>GraphQL; Docker|Dễ- vừa<br>_⋆⋆◦_|UI,<br>API,<br>DATA,<br>SEC,<br>PERF|K04,<br>K05,<br>K07,<br>K08,<br>K16|Dễdựng; lý<br>tưởng<br>cho<br>API<br>schema<br>testing, phân<br>quyền.|
|**R07**|**outline/outline**<br>Knowledge<br>base<br>cộng tác|TypeScript, React,<br>Node.js;<br>Post-<br>greSQL/Redis|Vừa<br>-<br>khó<br>_⋆⋆◦_|UI,<br>WF,<br>DATA,<br>REAL-<br>TIME|K02,<br>K10,<br>K11,<br>K15,<br>K16|Tốt cho kiểm<br>thửworkflow<br>tài liệu, phân<br>quyền, visual.|
|**R08**|**paperless-**<br>**ngx/paperless-**<br>**ngx**<br>Quản lý tài liệu,<br>OCR|Python/Django<br>+<br>Angular; OCR/ML<br>pipeline|Vừa<br>_⋆⋆◦_|UI,<br>API,<br>DATA,<br>FILE,<br>ASYNC|K01,<br>K05,<br>K09,<br>K12,<br>K16|Phù<br>hợp<br>fuzzing<br>file/input,<br>resilience<br>pipeline.|
|**R09**|**chatwoot/chatwoo**<br>Customer<br>support<br>đa kênh|**t**<br>Ruby<br>on<br>Rails<br>+<br>Vue;<br>Post-<br>greSQL/Redis;<br>realtime|Vừa<br>-<br>khó<br>_⋆⋆⋆_|UI,<br>API,<br>WF,<br>RE-<br>ALTIME,<br>DIST|K02,<br>K04,<br>K07,<br>K12,<br>K15|Nhiều<br>state,<br>event và con-<br>currency<br>để<br>tạo test sâu.|
|**R10**|**twentyhq/twenty**<br>CRM hiện đại|TypeScript,<br>NestJS,<br>React,<br>PostgreSQL;<br>monorepo|Khó<br>_⋆⋆⋆_|UI,<br>API,<br>WF,<br>PERF,<br>CONC|K04,<br>K05,<br>K07,<br>K10,<br>K15|Tốt cho nhóm<br>mạnh<br>Type-<br>Script;<br>kiến<br>trúc đủlớn.|
|**R11**|**makeplane/plane**<br>Quản<br>lý<br>dự<br>án/issue/sprint|TypeScript<br>+<br>Python/Django;<br>PostgreSQL, Redis|Khó<br>_⋆⋆⋆_|UI,<br>API,<br>WF,<br>DIST,<br>CONC|K02,<br>K04,<br>K07,<br>K12,<br>K15|Tốt<br>cho<br>model-based<br>testing (work-<br>flow quản lý<br>issue).|
|**R12**|**saleor/saleor**<br>Headless commerce<br>API|Python/Django,<br>GraphQL;<br>API-<br>first|Khó<br>_⋆⋆⋆_|API,<br>WF,<br>DATA,<br>PERF,<br>SEC|K04,<br>K05,<br>K07,<br>K08,<br>K15|Mạnh<br>back-<br>end/API;<br>kiểm<br>thử<br>GraphQL,<br>webhook.|



6 

|**Mã**|**Repo / Lĩnh vực**|**Stack**<br>**&**<br>**Kiến**<br>**trúc**|**Độkhó**|**Nhãn**|**Kỹ**<br>**thuật**|**Ghi chú**|
|---|---|---|---|---|---|---|
|**R13**|**immich-**<br>**app/immich**<br>Quản lý ảnh/video<br>tựhost|TypeScript/NestJS<br>+<br>Svelte;<br>Post-<br>greSQL,<br>ML<br>service|Khó<br>_⋆⋆⋆_|UI,<br>API,<br>FILE,<br>DIST,<br>PERF,<br>CONC|K01,<br>K09,<br>K12,<br>K13,<br>K15|Nổi<br>bật<br>nhưng<br>nặng<br>tài<br>nguyên,<br>cần cấu hình<br>máy tốt.|
|**R14**|**jellyfin/jellyfin**<br>Media server back-<br>end|C#/.NET, ffmpeg,<br>REST/API|Vừa<br>-<br>khó<br>_⋆⋆⋆_|API,<br>FILE,<br>PERF,<br>DIST|K05,<br>K07,<br>K09,<br>K12,<br>K14|Tốt cho hiệu<br>năng, fuzzing<br>media;<br>cần<br>lưu ý ffmpeg.|
|**R15**|**mattermost/matte**<br>Nền tảng chat cho<br>team dev|**rmost**<br>TypeScript + Go;<br>monorepo; realtime|Khó<br>_⋆⋆⋆_|UI,<br>API,<br>REAL-<br>TIME,<br>DIST,<br>PERF,<br>CONC|K04,<br>K07,<br>K12,<br>K15,<br>K16|Quy mô lớn,<br>kiểm<br>thử<br>hệ<br>thống<br>production-<br>grade.|
|**R16**|**appsmithorg/apps**<br>Low-code platform|**mith**<br>TypeScript/Java;<br>frontend<br>+<br>back-<br>end; sandbox|Khó<br>_⋆⋆⋆_|UI,<br>API,<br>DIST,<br>PERF,<br>SEC|K04,<br>K07,<br>K08,<br>K10,<br>K15|Codebase<br>lớn;<br>dành<br>cho nhóm có<br>năng lực đọc<br>monorepo.|



7 

## **Phụlục 2: danh sách kỹthuật kiểm thửnâng cao** 

Danh sách các kỹthuật có thểsinh ra các kịch bản test (artefact) cụthể, chạy được tựđộng: 

|**Mã**|**Kỹthuật**|**Ý tưởng cốt lõi**|**Đối**<br>**tượng**<br>**phù**<br>**hợp**|**Công cụ**|**Đầu ra**|**Khó**|
|---|---|---|---|---|---|---|
|**K01**|**Property-**<br>**Based Test-**<br>**ing**|Xác định tính chất<br>đúng<br>(invariant);<br>sinh nhiều dữliệu,<br>shrink ca lỗi.|Hàm xửlý, valida-<br>tion, API có input<br>phong phú.|Hypothesis,<br>jqwik, fast-<br>check|_≥_3 property;<br>sinh<br>test<br>tự<br>động;<br>lưu<br>counterexam-<br>ple.|_⋆⋆◦_|
|**K02**|**Model-**<br>**Based**<br>**/**<br>**Stateful**|Mô<br>hình<br>hóa<br>hệ<br>thống<br>bằng<br>state/transition;<br>tựsinh chuỗi hành<br>động.|Booking,<br>issue<br>workflow,<br>chat,<br>checkout.|GraphWalke<br>Hypothesis|r,<br>Sơ đồState;<br>coverage<br>trạng<br>thái;<br>_≥_<br>3<br>chuỗi<br>nhánh.|_⋆⋆⋆_|
|**K03**|**Mutation**<br>**Testing**|Chèn "mutant"vào<br>mã nguồn; bộtest<br>tốt phải phát hiện<br>và làm mutant thất<br>bại.|Module có unit test<br>ổn định, business<br>logic.|Stryker,<br>PIT, mut-<br>mut|Baseline<br>tests; báo cáo<br>killed/survived<br>so sánh score.|;<br>_⋆⋆◦_|
|**K04**|**Contract**<br>**Testing**|Contract<br>sinh<br>từ<br>consumer và replay<br>tại<br>provider<br>để<br>tránh<br>breaking<br>change.|Frontend-backend,<br>microservice, API.|Pact|Xác<br>định<br>consumer-<br>provider; _≥_5<br>interactions;<br>demo.|_⋆⋆⋆_|
|**K05**|**Schema-**<br>**Based**<br>**API**<br>**/ Fuzz**|Dùng<br>Ope-<br>nAPI/GraphQL<br>để<br>sinh<br>request<br>hợp lệ/lỗi và test<br>invariant/status.|Repo<br>API-<br>first,<br>có<br>Ope-<br>nAPI/GraphQL.|Schemathesi<br>Postman|s,<br>Chạy schema<br>tests;<br>lưu<br>reproducer;<br>thống kê lỗi.|_⋆⋆◦_|
|**K06**|**Combinatoria**<br>**/ Pairwise**|**l**<br>Giảm không gian tổ<br>hợp bằng pairwise<br>thay vì vét cạn tích<br>Descartes.|Form nhiều tham<br>số, role, cấu hình,<br>filter.|Microsoft<br>PICT|Sinh pairwise;<br>so<br>sánh<br>với<br>exhaustive;<br>chạy mẫu.|_⋆◦◦_|
|**K07**|**Performance**<br>**(Load/Stress**|**)**<br>Đo<br>latency,<br>throughput,<br>er-<br>ror rate dưới tải<br>thực tếvà cực hạn.|API,<br>chat,<br>com-<br>merce,<br>media,<br>nhiều user.|k6,<br>JMe-<br>ter,<br>Gatling|Workload<br>model;<br>_≥_<br>3<br>profile<br>tải;<br>biểu đồRPS.|_⋆⋆◦_|
|**K08**|**DAST (Dy-**<br>**namic Secu-**<br>**rity)**|Chủđộng gửi pay-<br>load tấn công để<br>tìm lỗhổng web<br>phổbiến.|Web app có auth,<br>API, form, session.|OWASP<br>ZAP|Chỉ<br>quét<br>local;<br>pas-<br>sive/active<br>scan;<br>verify<br>thủcông.|_⋆⋆◦_|
|**K09**|**Fuzz**<br>**Test-**<br>**ing**|Sinh<br>input<br>tốc<br>độ<br>cực<br>lớn<br>để<br>tìm<br>crash,<br>hang,<br>memory<br>bug,<br>lỗi<br>parser.|Parser, file xửlý,<br>import/export.|libFuzzer/A|FL++/Jazzer<br>Fuzz<br>tar-<br>get;<br>corpus<br>ban<br>đầu;<br>minimized<br>input.|_⋆⋆⋆_|



8 

|**Mã**|**Kỹthuật**|**Ý tưởng cốt lõi**|**Đối**<br>**tượng**<br>**phù**<br>**hợp**|**Công cụ**|**Đầu ra**||**Khó**|
|---|---|---|---|---|---|---|---|
|**K10**|**Visual**<br>**Re-**<br>**gression**<br>**Testing**|So sánh screenshot<br>với ảnh gốc (base-<br>line) đểtìm thay<br>đổi<br>UI<br>ngoài<br>ý<br>muốn.|Web UI ổn định,<br>dashboard, editor.|Playwright|Có<br>ba<br>_≥_<br>8<br>hình;<br>tional<br>regressi|seline;<br>màn<br>inten-<br>vs<br>on.|_⋆◦◦_|
|**K11**|**Automated**<br>**Accessibil-**<br>**ity**|Tựđộng kiểm tra<br>WCAG,<br>kết<br>hợp<br>kiểm tra dùng bàn<br>phím thủcông.|Web<br>UI,<br>form,<br>modal, navigation.|axe-core,<br>Playwright|Chạy<br>phân<br>lỗi; kiể<br>keyboar|axe;<br>nhóm<br>m tra<br>d.|_⋆◦◦_|
|**K12**|**Fault Injec-**<br>**tion**<br>**/**<br>**Re-**<br>**silience**|Gây<br>latency,<br>net-<br>work down đểkiểm<br>tra<br>retry,<br>circuit-<br>breaker, fallback.|Ứng dụng nhiều de-<br>pendency (DB, Re-<br>dis...).|Toxiproxy,<br>Docker<br>Compose|Lập<br>model;<br>scenario<br>automa<br>injectio|Fault<br>_≥_<br>4<br>s;<br>ted<br>n.|_⋆⋆⋆_|
|**K13**|**Metamorphic**<br>**Testing**|Kiểm tra quan hệ<br>nhiều lần chạy sau<br>khi biến đổi input<br>(không cần oracle).|Search, data trans-<br>form, recommenda-<br>tion.|Tự<br>xây,<br>Hypothesis|_≥_<br>3<br>morphi<br>relation<br>động so|meta-<br>c<br>s;<br>tự<br> sánh.|_⋆⋆⋆_|
|**K14**|**Differential**<br>**Testing**|Chạy 1 input trên<br>2 version/config và<br>tìm ra khác biệt<br>hành vi.|API<br>version,<br>DB<br>backend,<br>bản<br>cũ/mới.|Tự<br>xây,<br>Hypothesis|Hai<br>trường<br>phân<br>danh s<br>defect.|môi<br>test;<br>loại<br>ách lỗi|_⋆⋆⋆_|
|**K15**|**Concurrency**<br>**/ Race**|Tạo nhiều request<br>đồng thời đểtìm<br>lỗi double booking,<br>lost update.|Booking, cart, chat,<br>realtime, inventory.|k6,<br>Play-<br>wright<br>parallel|Xác<br>invarian<br>_≥_<br>3<br>scenario|định<br>t;<br>race<br>s.|_⋆⋆⋆_|
|**K16**|**Ephemeral**<br>**Integration**|Khởi<br>tạo<br>depen-<br>dency<br>thật<br>trong<br>Docker<br>(tránh<br>mock sai lệch) cho<br>test.|Backend<br>có<br>DB/cache/broker.|Testcontaine<br>Docker|rs,<br>Fixture<br>tainer;<br>integrat<br>tests.|con-<br>_≥_<br>5<br>ion|_⋆⋆◦_|



## **Phụlục 3: quy tắc ghép tổhợp repo** _×_ **kỹthuật** 

Không phải Repo nào cũng phù hợp với mọi Kỹthuật. Sinh viên cần tham khảo bảng quy tắc dưới đây đểchọn tổhợp khảthi: 

|**Kỹthuật**|**Nên ghép khi**|**Tránh hoặc điều kiện không nên**<br>**ghép**|
|---|---|---|
|**K01**<br>**Property-**|Ưu tiên module có hàm xửlý|Không ép vào UI thuần hoặc quy|
|**based**|logic, validation rõ ràng.|trình workflow quá phụthuộc môi<br>trường.|
|**K02 Model-based**|Ưu tiên R05, R07, R09, R11, R12<br>hoặc workflow có lưu trạng thái.|Không dùng nếu nhóm chỉkiểm thử<br>một endpoint CRUD đơn giản.|



9 

|**Kỹthuật**|**Nên ghép khi**|**Tránh hoặc điều kiện không nên**<br>**ghép**|
|---|---|---|
|**K03 Mutation**|Repo/module phải có unit test ổn<br>định, build nhanh.|Tránh test toàn bộmonorepo rất<br>lớn; giới hạn lại 1 package/module.|
|**K04 Contract**|Phải có ranh giới API rõ ràng giữa<br>phía consumer - provider.|Nếu<br>repo<br>monolith<br>không<br>có<br>client/provider tách biệt thì không<br>áp dụng.|
|**K05 Schema-based**|Dự<br>án<br>có<br>sẵn<br>file<br>Ope-<br>nAPI/GraphQL<br>hoặc<br>có<br>thể<br>trích schema.|Không phù hợp nếu không có API<br>(vd: công cụdesktop/media local).|
|**K06 Pairwise**|Dựán có form điền nhiều tham<br>số, cấu hình, bộlọc tìm kiếm.|Dễbịquá đơn giản nếu chỉsinh case<br>ra Excel mà không code script chạy.|
|**K07 Performance**|Chọn được luồng đọc/ghi đại diện<br>và có sẵn script tạo dữliệu tải.|Chỉload test ởlocal/lab; tuyệt<br>đối<br>không<br>bắn<br>tải<br>vào<br>public<br>server/demo.|
|**K08 DAST**|Ưu tiên trang có luồng đăng nhập,<br>form phân quyền, session.|Chỉquét instance cài ởmáy Local.<br>Cấm quét các hệthống Internet.|
|**K09 Fuzz**|Ưu tiên parser, xửlý file tải lên,<br>chức năng Import/Export.|Cần tạo bộHarness rõ ràng; tránh<br>việc fuzz mù mờtoàn bộhệthống.|
|**K10 Visual regres-**<br>**sion**|UI ổn định và có thểcốđịnh được<br>kích thước browser/data.|Không tốt với trang realtime đổi<br>dữliệu liên tục nếu không làm giả<br>(mock).|
|**K11 Accessibility**|Ưu tiên UI có chứa form, modal,<br>menu điều hướng, dashboard.|Bắt buộc bổsung phần tựtay kiểm<br>tra phím (keyboard), không chỉchạy<br>tool.|
|**K12 Fault injection**|Hệthống phụthuộc nhiều qua<br>mạng (gọi DB, Redis, Worker<br>node).|Không cần thiết với ứng dụng chạy<br>1 tiến trình độc lập không gọi dịch<br>vụ.|
|**K13 Metamorphic**|Có thểxác định quan hệbiến đổi<br>dữliệu (vd: sắp xếp, bộlọc).|Không dùng nếu nhóm không hiểu<br>và không giải thích được "Oracle<br>Problem".|
|**K14 Differential**|Cần 2 phiên bản hoặc 2 cấu hình<br>khác nhau dùng chung hợp đồng<br>API.|Phải lọc được khác biệt hợp lệtrước<br>khi gán nhãn đó là lỗi (defect).|
|**K15 Concurrency**|Ưu tiên chức năng đặt chỗ(book-<br>ing), giỏhàng, kho hàng, chat.|Phải kiểm tra tính nhất quán dữliệu<br>ởCSDL, không chỉgọi API mù.|
|**K16 Testcontainers**|Dự<br>án<br>Backend<br>kết<br>nối<br>với<br>DB/cache/message broker.|Chú ý giới hạn sốlượng dependency<br>đểmáycá nhân sinh viên chạyđược.|



10 

## **Phụlục 4: nguồn tham khảo** 

### **4.1. Link kho chứa mã nguồn (GitHub Repositories)** 

-  **R01:** `https://github.com/spring-projects/spring-petclinic` 

-  **R02:** `https://github.com/mealie-recipes/mealie` 

-  **R03:** `https://github.com/grokability/snipe-it` 

-  **R04:** `https://github.com/nopSolutions/nopCommerce` 

-  **R05:** `https://github.com/calcom/cal.com` 

-  **R06:** `https://github.com/directus/directus` 

-  **R07:** `https://github.com/outline/outline` 

-  **R08:** `https://github.com/paperless-ngx/paperless-ngx` 

-  **R09:** `https://github.com/chatwoot/chatwoot` 

-  **R10:** `https://github.com/twentyhq/twenty` 

-  **R11:** `https://github.com/makeplane/plane` 

-  **R12:** `https://github.com/saleor/saleor` 

-  **R13:** `https://github.com/immich-app/immich` 

-  **R14:** `https://github.com/jellyfin/jellyfin` 

-  **R15:** `https://github.com/mattermost/mattermost` 

-  **R16:** `https://github.com/appsmithorg/appsmith` 

### **4.2. Tài liệu & công cụkỹthuật kiểm thử** 

-  **Property-Based Testing - Hypothesis:** `https://hypothesis.readthedocs.io/` 

-  **Model-Based Testing - GraphWalker:** `https://graphwalker.github.io/` 

-  **Mutation Testing - Stryker Mutator:** `https://stryker-mutator.io/docs/` 

-  **Contract Testing - Pact:** `https://docs.pact.io/` 

-  **Schema-Based API - Schemathesis:** `https://schemathesis.github.io/schemathesis/` 

-  **Pairwise Testing - Microsoft PICT:** `https://github.com/microsoft/pict` 

-  **Performance Testing - k6:** `https://grafana.com/docs/k6/latest/` 

-  **DAST - OWASP ZAP:** `https://www.zaproxy.org/docs/` 

-  **Fuzz Testing - OSS-Fuzz:** `https://github.com/google/oss-fuzz` 

-  **Visual Regression - Playwright:** `https://playwright.dev/docs/test-snapshots` 

-  **Accessibility Testing - axe-core:** `https://github.com/dequelabs/axe-core` 

11 

-  **Fault Injection - Toxiproxy:** `https://github.com/Shopify/toxiproxy` 

-  **Ephemeral Integration - Testcontainers:** `https://testcontainers.com/` 

12 

