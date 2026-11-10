# Chương 6: Những con số biết nhúc nhích

Sáng thứ Hai đầu tuần thứ ba, ông Roger gọi tôi vào phòng họp kính, đúng căn phòng hôm phỏng vấn.

Lần này không có Dân ngồi bên. Chỉ có tôi, ông Roger, và một cái bảng trắng.

– Phong, – ông nói chậm rãi, – I have a task for you. Your first real task.

Ông cầm bút, vẽ lên bảng một hình chữ nhật, ghi chữ *Robot*. Cách đó một khoảng, ông vẽ một hình chữ nhật khác, ghi chữ *Operator*, rồi vẽ một mũi tên nối hai bên, ở giữa ông viết chữ *Network*.

– We need software, – ông gõ bút lên mũi tên, – so that a person can connect to the robot from far away. See what the robot sees, read its status, and control it. Move the arms, the head, later maybe walking. We call it teleoperation. Teleop.

Ông quay sang nhìn tôi:

– You talked about remote control and bad network in your interview. So, this is yours.

Tôi nhìn cái mũi tên trên bảng trắng. Tim đập nhanh tới mức tôi nghe được tiếng nó trong tai.

– Yes. I… I will do it.

– Take your time. First, research. Understand how the robot talks. Then build something small. Okay?

– Okay.

Ông Roger mỉm cười, đậy nắp bút:

– Good. I believe in you.

---

Cả tuần đó, tôi gần như không ngẩng đầu lên khỏi màn hình.

Tôi đào bới mọi thứ liên quan tới cách con robot giao tiếp. Robot chạy ROS 2, một nền tảng phần mềm mà các tiến trình nói chuyện với nhau bằng cách phát và nhận những gói tin gọi là *topic*. Có topic chứa góc của từng khớp. Có topic chứa dữ liệu IMU. Có topic chứa hình ảnh từ camera. Muốn điều khiển robot thì phải gửi lệnh vào đúng topic, đúng định dạng, đúng tần số. Và quan trọng nhất là phải đi qua lớp giám sát an toàn mà anh Huni đã dặn đi dặn lại.

Tôi đọc mã nguồn của các module cũ. Tôi đọc tài liệu của bộ SDK. Tôi đọc những bài viết trên diễn đàn quốc tế lúc mười một giờ đêm, vừa đọc vừa tra từ điển. Tôi thử dựng một môi trường mô phỏng trên máy mình để khỏi đụng vào con robot thật.

Khoa ngồi phía sau tôi, làm mô phỏng, nên tôi hỏi nó nhiều nhất. Nó giải thích nhiệt tình, kiểu giải thích của một đứa vừa học xong và còn nhớ rõ mình đã từng không hiểu chỗ nào.

– Anh hiểu nó như cái chợ vậy nè, – Khoa vẽ lên giấy. – Mỗi topic là một sạp hàng. Ai muốn bán thì bày hàng ra, ai muốn mua thì ghé sạp đó. Mà chợ này không có ông quản lý, ai đi chợ cũng tự kiếm sạp.

– Còn cái lớp an toàn?

– Là bà bảo vệ chợ. Ai mang hàng cấm vô là bà đuổi ra liền.

Tôi cười. Ví von hơi kỳ, nhưng tôi nhớ được.

Tới thứ Sáu tuần đó, tôi chưa làm ra được gì để khoe. Chỉ có một cuốn sổ chi chít ghi chú, một sơ đồ kiến trúc vẽ đi vẽ lại năm lần, và một danh sách những thứ cần thử.

Trong buổi họp, tôi báo cáo đúng như vậy. Tôi hơi lo, sợ người ta nghĩ mình chậm.

Ông Roger chỉ nói:

– Good. Research first, code later. Next week, show me something.

---

Tuần thứ tư là tuần Giáng sinh.

Sáng thứ Hai, trên bàn mỗi người có một cây kẹo gậy sọc đỏ trắng và một tấm thiệp nhỏ viết tay bằng tiếng Anh. Thiệp của tôi ghi: *Merry Christmas, Phong. Keep building. – Roger.* Chữ ông nghiêng nghiêng, hơi khó đọc, nhưng tôi đọc tới ba lần.

Trưa hôm đó, ông Roger đi một vòng khu AHN, khoe ảnh trên điện thoại. Vợ ông là người Việt, quê Cần Thơ. Hai cô con gái, một đứa chín tuổi, một đứa sáu tuổi, mặc váy công chúa màu hồng đứng hai bên cây thông Noel trong phòng khách. Ông gọi hai đứa là *my two princesses*, và lần nào nhắc tới, đuôi mắt ông cũng xếp thành hình rẻ quạt.

Tôi dán tấm thiệp lên cạnh màn hình rồi bắt tay vào việc.

Tôi bắt đầu với một phần mềm nhỏ, thật nhỏ. Chỉ cần kết nối được vào robot và đọc dữ liệu ra, chưa cần điều khiển gì cả. Một cửa sổ đơn giản, nền đen, chữ trắng, vài ô thông số.

Ngày đầu, nó không kết nối được. Lỗi mạng.

Ngày thứ hai, nó kết nối được nhưng không nhận được dữ liệu gì. Hóa ra tôi cấu hình sai miền mạng.

Ngày thứ ba, nó nhận được dữ liệu, nhưng toàn những con số vô nghĩa. Tôi giải mã sai định dạng tin nhắn.

Ngày thứ tư rơi vào thứ Năm, đúng ngày Giáng sinh. Văn phòng thưa người. Một nửa team xin nghỉ, chỉ còn tôi, Dân, Khoa và anh Huni ngồi gõ phím trong tiếng nhạc Giáng sinh văng vẳng từ khu Embedded bên cạnh.

Ba giờ chiều, tôi sửa xong dòng code cuối cùng, chạy lại chương trình.

Màn hình đen. Rồi từng dòng chữ hiện lên:

```
Robot name:   ARA-02
Robot ID:     HN-0207
Status:       CONNECTED
Battery:      78%

Torso pitch:   0.4°
Torso roll:   -0.2°

L_shoulder_pitch:   12.3°
L_shoulder_roll:     5.1°
L_elbow:            -30.7°
R_shoulder_pitch:   12.1°
...
```

Tôi nhìn trân trân vào màn hình, không dám thở.

– Dân ơi… Dân! – Tôi gọi, giọng lạc đi. – Nó lên rồi!

Dân chạy qua, nhìn màn hình, rồi nhìn tôi:

– Để em vô lab thử.

Dân đi vào phòng lab. Qua lớp kính, tôi thấy cậu ta bước tới con robot ARA-02 đang treo trên khung thép. Robot đang ở chế độ thả lỏng, khớp mềm, có thể cầm tay xoay được. Dân nắm lấy cánh tay trái của robot, nhẹ nhàng nâng lên.

Trên màn hình của tôi, dòng chữ `L_shoulder_pitch` bắt đầu nhảy số.

`12.3°… 18.6°… 27.4°… 41.0°…`

Dân hạ tay robot xuống. Con số lại chạy ngược về.

`35.2°… 22.8°… 13.0°…`

Dân nghiêng thân robot sang một bên. Dòng `Torso roll` nhảy lên `4.7°`.

Tôi ngồi đó nhìn những con số nhúc nhích trên màn hình. Không có hình ảnh, không có âm thanh, chỉ là những chữ số trắng trên nền đen. Vậy mà tôi có cảm giác như đang nghe nhịp tim của một sinh vật sống.

Khoa đứng sau lưng tôi từ lúc nào, ly trà sữa trên tay quên cả hút. Nó nhìn màn hình một lúc rồi khẽ nói:

– Nó đang thở kìa anh.

Tôi gật đầu. Tôi không nói được gì.

Anh Huni đi tới, đặt tay lên vai tôi, bóp nhẹ một cái:

– Ngon rồi em.

Chỉ ba chữ, vậy mà tôi muốn chạy ra ngoài bãi cỏ hét lên một tiếng.

---

Chiều thứ Sáu, họp báo cáo.

Tới lượt tôi, tôi kết nối laptop lên màn hình chiếu, mở phần mềm, kết nối vào ARA-02. Dân đứng sẵn trong lab, nhận tín hiệu tôi gật đầu là cử động tay robot. Những con số nhảy múa trên màn hình chiếu trước mặt cả phòng.

Tôi trình bày bằng tiếng Anh: phần mềm đọc được những gì, kiến trúc ra sao, tuần sau dự định làm gì. Vẫn sai ngữ pháp, vẫn lơ lớ, nhưng tôi không cần ai đỡ. Tờ giấy note Dân dúi vào tay tôi trước giờ họp chỉ có một chữ: *Chậm lại.* Tôi chậm lại.

Cả phòng im lặng lắng nghe. Không ai lướt điện thoại. Khoa còn ngồi thẳng lưng, chuyện hiếm có.

Tôi nói xong. Ông Roger không nói gì ngay. Ông nhìn màn hình chiếu thêm vài giây, những con số vẫn đang nhảy theo tay Dân, rồi gật gù, gật thêm lần nữa.

– Good job, Phong. Good job.

Hai chữ thôi. Hai chữ tiếng Anh ai cũng biết, đứa trẻ lớp hai cũng hiểu.

Tối đó tôi chạy xe máy về Bình Thạnh, kẹt xe ở ngã tư Hàng Xanh gần hai mươi phút, mà cứ ngồi trên yên cười một mình như thằng dở hơi. Đứng đèn đỏ, tôi lẩm bẩm hai chữ đó, *good job, good job*. Ông chú chạy xe ôm bên cạnh nhìn tôi rồi xích xe ra xa một chút.

Về tới phòng, tôi gọi cho mẹ.

– Mẹ ơi, con làm được rồi. Con đọc được số liệu từ con robot. Sếp khen con.

– Đọc số liệu là sao con?

– Là… là con biết được con robot nó đang làm gì, tay nó giơ lên bao nhiêu độ, người nó nghiêng bao nhiêu độ.

– À. – Mẹ ngừng một chút. – Giống như bắt mạch hả con?

Tôi khựng lại. Rồi tôi cười.

– Dạ. Giống bắt mạch đó mẹ.

– Vậy là giỏi rồi. Ăn cơm chưa?

– Dạ chưa.

– Ăn đi. Đừng có ăn mì hoài.

Tôi dạ, rồi cúp máy, rồi nấu mì.
