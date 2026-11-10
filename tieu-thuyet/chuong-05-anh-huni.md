# Chương 5: Anh Huni và cuốn tài liệu dày cộp

Sáng thứ Ba, ngày thứ hai đi làm, anh Huni đặt lên bàn tôi một tập tài liệu in sẵn, đóng gáy lò xo, dày cỡ cuốn từ điển.

*Humanoid Platform – System Overview v3.2.*

– Em đọc dần dần nha, – anh nói, kéo ghế ngồi xuống cạnh tôi. – Không cần thuộc hết đâu. Đọc để biết con robot nó có gì trong người, cái gì nối với cái gì, cái gì hư thì robot té. Có gì không hiểu thì ghi ra, chiều anh em mình ngồi lại.

– Dạ.

– À, – anh chỉ vào trang đầu, – cái này là tiếng Anh hết á. Em đọc được không?

– Đọc thì được anh. Nói mới chết.

Anh Huni cười ha hả, vỗ vai tôi cái bốp:

– Vậy là được rồi! Robot nó không bắt em nói đâu. Mà anh nói em nghe, hồi mới vô anh cũng như em. Họp với ông Roger anh ngồi gật đầu suốt, về chỗ phải hỏi lại Dân ông nói gì. Sáu tháng là quen. Từ từ.

---

Hai tháng thử việc, tôi được giao một nhiệm vụ đơn giản: hiểu con robot.

Nghe thì đơn giản, nhưng làm thì không hề.

Con humanoid của C có hai mươi tám bậc tự do, tức hai mươi tám khớp có thể chuyển động độc lập. Mỗi chân sáu khớp, mỗi tay bảy khớp, cổ hai khớp. Mỗi khớp là một cụm động cơ với bộ giảm tốc và cảm biến vị trí riêng. Trong thân có bộ đo quán tính IMU để robot biết mình đang nghiêng bao nhiêu độ. Đầu có hai camera và một cảm biến chiều sâu. Ngực có một cảm biến lidar nhỏ quét xung quanh. Lưng là cục pin to bằng cái balo, nặng gần bảy ký.

Tất cả nói chuyện với nhau qua một mạng lưới phức tạp: board điều khiển cấp thấp, máy tính cấp cao, các tiến trình phần mềm gửi nhận dữ liệu hàng trăm lần mỗi giây.

Tôi đọc mỗi ngày từ sáng tới chiều. Đọc chỗ nào không hiểu thì tôi vẽ lại ra giấy. Vẽ không ra thì tôi chạy sang phòng lab, đứng nhìn con robot thật, tìm cho ra cái bộ phận mình vừa đọc nằm ở đâu.

Chiều nào anh Huni cũng ngồi với tôi nửa tiếng. Anh không giảng bài như thầy giáo. Anh kể chuyện.

– Cái khớp gối này nè, – anh chỉ vào bản vẽ, – hồi tháng sáu nó cháy một lần. Robot đang đi thì khựng lại, rồi ngồi phịch xuống như ông già mỏi chân. Cả team đứng nhìn, không ai nói được câu nào. Sau đó mới biết là do phần mềm gửi lệnh mô-men quá giới hạn liên tục ba phút. Từ đó tụi anh có thêm cái lớp giám sát này, – anh lật sang trang khác, – em đọc kỹ chỗ này nha. Sau này em làm gì đụng tới khớp thì phải qua lớp này.

Tôi ghi chép kín cả cuốn sổ.

---

Ở gần anh Huni được vài tuần, tôi hiểu được con người anh. Anh không cần nói gì nhiều về mình. Những việc nhỏ anh làm đã nói thay.

Anh là người tới sớm nhất và về muộn nhất, nhưng chưa bao giờ bắt ai ở lại. Sáu giờ chiều thấy ai còn ngồi, anh đi ngang gõ nhẹ lên bàn: "Về đi em, mai làm tiếp." Anh nhớ sinh nhật từng người trong team. Hôm sinh nhật anh Vũ, anh Huni lén mua bánh kem để trong tủ lạnh pantry từ trưa, giấu kỹ tới mức anh Vũ mở tủ lấy sữa mà không phát hiện ra.

Anh nói chuyện với ai cũng vui vẻ, từ ông Roger tới cô lao công dọn văn phòng mỗi tối. Anh gọi cô bằng tên, hỏi thăm đứa con trai cô năm nay thi lớp mười.

Nhưng điều làm tôi nể anh nhất xảy ra vào cuối tuần thứ hai.

Tôi vẽ lại sơ đồ luồng dữ liệu giữa các module, vì bản trong tài liệu đã cũ, nhiều chỗ không còn đúng. Tôi đưa anh Huni xem, anh bảo tốt, để anh đưa vào báo cáo tuần. Trong buổi họp chiều thứ Sáu, khi slide sơ đồ hiện lên, ông Roger gật gù:

– Nice. Very clear. Who made this, Huni?

Anh Huni không ngập ngừng một giây nào:

– Phong made it. Not me. Phong found the old one was wrong.

Ông Roger quay sang tôi, giơ ngón cái lên.

Tan họp, tôi đi theo anh ra pantry, ấp úng:

– Anh ơi, cái đó… anh đưa vào báo cáo của anh mà, anh cứ nhận cũng được…

Anh Huni đang rót cà phê, quay lại nhìn tôi, nhíu mày như thể tôi vừa nói một điều rất vô lý:

– Em làm thì là của em. Anh nhận thì anh thành cái gì?

Rồi anh đưa tôi ly cà phê vừa rót, rót cho mình ly khác.

Tôi đứng cầm ly cà phê, nhớ lại chuyện ở công ty cũ. Chuyện cái bản sửa lỗi đêm vợ anh đồng nghiệp chuyển dạ. Hồi đó tôi tự lắc đầu, tự nhường. Lần này có người không cho tôi nhường.

Hòa đồng, vui vẻ, thân thiện. Và liêm chính. Đó là bốn chữ tôi dùng để tả anh Huni, cả lúc đó lẫn bây giờ.

---

Nhịp làm việc của phòng AHN chạy đều như một cái đồng hồ.

Hai tuần một lần, sáng thứ Hai, cả team họp lập kế hoạch. Mỗi người nói mình sẽ làm gì trong hai tuần tới, ước lượng mất bao lâu, cần ai hỗ trợ. Anh Huni đứng ở bảng trắng, dán những mảnh giấy note màu thành từng cột: *Cần làm*, *Đang làm*, *Xong*.

Chiều thứ Sáu hằng tuần là họp báo cáo. Từng người lần lượt nói tuần này làm được gì, gặp vấn đề gì, đang kẹt chỗ nào. Ai kẹt thì cả phòng cùng xúm vào gỡ. Không ai bị mắng vì chậm. Người ta chỉ hỏi: "Em cần gì để làm tiếp?"

Họp thì toàn bằng tiếng Anh, vì có ông Roger.

Hai tuần đầu, mỗi lần họp là một lần tôi muốn độn thổ. Mọi người nói nhanh, chen thuật ngữ, đùa với nhau bằng những câu tôi không bắt kịp. Cả phòng cười mà tôi không biết cười vì cái gì, đành cười theo nửa giây sau, như phim lồng tiếng bị lệch tiếng.

Rồi một chiều thứ Sáu, giữa buổi họp, có một tờ giấy note màu xanh lá được đẩy sang chỗ tôi.

Là Dân, người ngồi ngay cạnh tôi. Cậu không nhìn tôi, mắt vẫn dán vào màn hình chiếu. Trên tờ giấy là chữ viết tay rất nhỏ, rất đều:

*Roger hỏi: tuần sau anh có cần thêm thời gian đọc phần IMU không. Trả lời: "Yes, two more days, please."*

Tôi nhìn tờ giấy, rồi ngẩng lên. Ông Roger đang nhìn tôi, chờ đợi.

– Yes… two more days, please.

– Okay, no problem.

Hết họp, tôi quay sang định cảm ơn. Dân đã đứng dậy, kẹp laptop dưới nách, đi thẳng ra pantry như thể chẳng có chuyện gì.

Từ hôm đó, buổi họp chiều thứ Sáu nào tôi cũng nhận được ít nhất một tờ giấy note. Có khi là bản dịch. Có khi là một từ vựng kèm nghĩa. Có lần chỉ là một hình mặt cười vẽ vội, ngay sau lúc tôi nói vấp liền ba chữ.

Tôi giữ hết những tờ giấy đó, kẹp trong cuốn sổ của mình.

Tối về phòng trọ, tôi bắt đầu tập nói tiếng Anh. Tôi mở mấy video luyện phát âm, đứng trước gương nói theo, lặp đi lặp lại những câu như *"I have finished the analysis of the IMU module"* cho tới khi lưỡi hết líu. Thằng Bảo đi ngang, nhìn tôi như nhìn người bị ma nhập.

– Mày tập nói với ai vậy?

– Với sếp.

– Sếp mày đâu?

– Trong gương.

– …Tao nói thiệt, mày cần ra ngoài nhiều hơn.

---

Cũng trong buổi họp cuối tuần thứ hai ấy, sau màn sơ đồ của anh Huni, tới lượt tôi báo cáo. Lần đầu tiên tôi nói một mạch gần hai phút bằng tiếng Anh mà không cần ai đỡ. Tôi trình bày đã đọc xong những phần nào, vẽ lại sơ đồ luồng dữ liệu nào, còn những câu hỏi nào chưa có lời giải.

Ngữ pháp vẫn sai. Phát âm vẫn lơ lớ. Nhưng tôi nói hết.

Ông Roger nghe xong, gật đầu:

– Good. You learn fast.

Dưới gầm bàn, Dân đẩy sang một tờ giấy note.

Lần này không có chữ nào cả. Chỉ có một ngón tay cái được vẽ bằng bút màu cam.
