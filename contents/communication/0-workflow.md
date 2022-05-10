# Workflow

**[⮌ Index](../index.md)** |

Làm thế nào để làm tốt việc trao đổi với khách hàng? đây là câu hỏi không chỉ BrSE, comtor, mà của cả vị trí developer nữa.
Trong công ty bây giờ không chỉ có các dự án với khách hàng Nhật, mà còn dự án với bên Mỹ, nơi mà developer được trực tiếp trao đổi và nhận công việc từ phía khách hàng.
Trong tình huống này thì các trao đổi hiệu quả là cần thiết hơn bao giờ hết.

Nếu bạn là người đang phải chịu trách nhiệm trao đổi với khách hàng nhưng vẫn đang loay hoay, hoặc đã làm tốt rồi nhưng vẫn muốn tham khảo cách làm khác thì có thể đọc qua một số gạch đầu dòng sau.
Dưới đây là guide dành cho BrSE hoặc comtor, nhưng chúng ta có thể mở rộng hơn, dành cho những ai đang phải trao đổi với khách hàng.

## 1. Những yêu cầu tối thiểu mà khách hàng yêu cầu mình phải làm được

### 1.1 Estimate

- Khi nhận spec thì phải đưa ra được estimate
- Với các task phức tạp, thời gian làm khoảng 8h trở lên thì phải đưa ra được hướng làm cho khách hàng biết
  - Sẽ thêm bảng xxx
  - Thêm cột yyy và bảng zzzz
  - Thêm màn hình aaaa thay vì sửa màn hình bbbb
- Cần đưa ra lí do của hướng làm của mình
- Với các thông tin mình đưa ra (estimate/hướng làm), sau khi đã báo với khách hàng qua Slack thì phải ghi lại vào Trello/Github hoặc đâu đó để làm evidence

### 1.2 Confirm spec

- Các câu hỏi confirm spec
  - Không hỏi kiểu `Cái này/cái kia là cái gì`
  - Phải hỏi kiểu giả định như `Mình đang hiểu XXXXX có nghĩa là YYYY, thế có phải không?`
- Khách hàng cần biết được phía bên VN đang hiểu ra sao (đúng hay sai không quan trọng ở giai đoạn này)
  - Từ cách hiểu của bên VN thì khách hàng mới biết là nên làm gì tiếp theo
- Khách hàng sẽ cần mình nói nội dung một cách cụ thể hơn khi hỏi
  - Thậm chí có lúc khách hàng sẽ yêu cầu mình viết lại câu hỏi để dành cho người không hiểu gì về kỹ thuật
  - Sẽ có lúc khách hàng muốn bên VN cũng chủ động đưa ra những việc muốn khách hàng làm

### 1.3 Confirm hướng làm

- Sẽ có trường hợp phát sinh nhiều hướng giải quyết vấn đề. Thường thì bên VN sẽ họp và chốt luôn.
- Tuy nhiên tùy vào mức độ ảnh hưởng đến với dự án/khách hàng mà mình sẽ phải đưa ra để hỏi khách hàng
- Cách đưa ra sẽ như sau
  - Phương án 1: cách làm + điểm cộng + điểm trừ
  - Phương án 2: cách làm + điểm cộng + điểm trừ
  - Phương án 3: ....
- Sau đó đưa luôn phương án mà phía team VN mong muốn làm và lí do
- Đưa được ra đầy đủ thông tin như trên thì trách nhiệm chốt phương án, chịu điểm trừ sẽ được đẩy cho khách hàng, team VN đã làm hết trách nhiệm
- Cần note lại các phương án mình đưa ra vào Trello/Github
- Sau này khách hàng chốt phương án nào thì cũng đưa tiếp vào Trello/Github để làm evidence
- Cố gắng đưa ra được tối thiểu 3 phương án cho khách hàng, tránh việc mình chốt phương án làm tùy tiện, sau này có phát sinh gì thì sẽ bị khách hàng claim và phạt

### 1.4 Trao đổi với dev (trong trường hợp mình phải phụ trách thêm người khác)

- Dev cũng là 1 điểm tiếp nhận thông tin, nên cũng sẽ dễ có sai lệch phát sinh
- Đặc thù dự án spec không rõ ràng, nên khả năng hiểu nhầm yêu cầu rất dễ xảy ra
- Khi dịch spec, mô tả yêu cầu nên mô tả trên màn hình
  - Nếu trong spec khách hàng đưa đã có ảnh mô tả thì tốt
  - Nếu spec không có ảnh thì sau khi dev đọc, mình nên ngồi cạnh lại 1 lần nữa để xem cách hiểu của dev có gì sai lệch hay không?
- Các phương án làm/estimate ở trên chỉ có được sau khi dev hiểu cái cần làm
  - Các phương án đưa ra chính là các phương án của dev

### 1.5 Develop

- Bước phát triển là việc của Dev, tuy nhiên BrSE/người trao đổi spec cũng cần để ý xem có vấn đề gì phát sinh hay không?
- Khi khách hàng đổi spec giữa chừng, cần bổ sung thông tin vào ticket, báo dev estimate lại
- Bổ sung spec chứ ko được sửa spec ban đầu: để lưu evidence việc đổi spec giữa chừng
- Nguyên tắc là spec thay đổi = estimate lại
- Nếu có thay đổi con số estimate thì cần báo lại khách hàng, thậm chí lùi schedule của các phần khác nếu mức độ ảnh hưởng lớn

### 1.6 Kiểm tra sản phẩm

- Khi mình là người trao đổi thì bản thân sẽ phải có trách nhiệm kiểm tra sản phẩm rồi mới báo khách hàng
- Chỉ kiểm tra sau khi dev đã làm và test (nếu bản thân mình không phải là người làm)
- Tuy nhiên, việc test phải có evidence thì mới được chấp nhận
- Ảnh chụp màn hình
- Video quay thao tác
- Checklist
- Unit Test

### 1.7 Báo cáo hoàn thành

- Thường khách hàng sẽ yêu cầu mình tạo Pull Request khi mình làm xong
- Trong Pull Request sẽ có
- Danh sách những việc mình đã làm
- Các evidence của mình
- Các điểm chưa xong và lý do
- Về evidence
- Do khách hàng không biết tên thật ai làm dự án nào
- Trong các evidence chỉ nên dùng các từ chung chung như: test, dev,... tránh dùng tên riêng/cá nhân

### 1.8 Báo cáo công việc hàng ngày

- Do lượng dự án lớn, khách hàng bận nên sẽ ko nắm rõ được ai đã/đang/sẽ làm gì
- Việc báo cáo công việc hàng ngày sẽ giúp khách hàng dễ điều chuyển công việc hơn

## 2. Những yêu cầu khách hàng mong muốn mình làm thêm để support cho khách hàng, giúp công việc trôi chảy hơn

- Tự xem email lỗi, SENTRY để phát hiện lỗi trước khi khách hàng báo
- Khách hàng khá bận, thường chỉ biết được là có lỗi khi user kêu, khi đó thì vấn đề thường đã muộn
- Đưa ra đề xuất các tính năng muốn cải tiến dự án
- Lý do
- Hướng làm
- Estimate

## Nhiều ý quá, có thể tóm tắt lại ngắn gọn dễ hiểu, dễ nhớ hơn không?

Mỗi vị trí trên flow trao đổi Khách hàng --> BrSE/người trao đổi --> Dev đều là con người, do đó sai lệch nhận thức là việc luôn luôn xảy ra. Từ sai lệch nhận thức sẽ dẫn đến sai lệch về output.

Việc của người chịu trách nhiệm trao đổi là coi sai lệch đó là issue, và với mỗi giai đoạn sẽ phải tìm cách xóa bay sai lệch đó, xử lý sai lệch trước khi nó biến thành output. Sai lệch càng ít, các bên sẽ hiểu nhau hơn, output làm ra sẽ đúng hơn với yêu cầu.

Tất cả các ý ở trên đều chỉ nhằm mục tiêu giảm sai lệch về nhận thức. Nên nếu người trao đổi tự mình ý thức được sai lệch, luôn mong muốn giải quyết sai lệch thì sẽ ko cần phải mở guide này ra đọc hay học vẹt gì cả.

---
**[⮌ Index](../index.md)** |
