# HỆ THỐNG BÁN VÉ TÀU HỎA

## GIỚI THIỆU TỔNG QUAN
Một hệ thống bán vé tàu sẽ ghi nhận lại thông tin của mỗi hành khách sau mỗi lần đặt vé tàu như sau:

Mỗi khi thực hiện đăng ký với hệ thống sẽ được cung cấp một tài khoản cá nhân với ID tài khoản là duy nhất, cùng với việc cung cấp những thông tin gồm: họ tên hành khách, tuổi, giới tính, thông tin liên lạc (số điện thoại, email). Với những lần đăng nhập tiếp theo, hành khách chỉ cần nhập mã ID để truy cập vào tài khoản. 

Mỗi hành khách sẽ được đặt nhiều vé và mỗi vé chỉ được sở hữu bởi một hành khách. Thông tin về vé bao gồm: mã vé, loại vé, giá vé, thời gian đi, trạm đón, trạm dừng và mã tàu mà vé có hiệu lực. Mỗi mã vé là duy nhất và chia thành 2 loại vé (phổ thông và vé VIP). Giá vé của từng loại vé sẽ khác nhau, cụ thể: với loại vé phổ thông sẽ đồng loạt có giá tiền là 100.000 VND và với loại vé VIP, giá tiền sẽ đắt hơn 50% so với giá vé phổ thông. 
Sau khi hoàn tất việc đăng ký, hành khách thực hiện thanh toán. Hành khách có thể lựa chọn thanh toán ngay lập tức hoặc thanh toán sau, tuy nhiên việc thanh toán sau phải tuân theo thời gian thanh toán quy định của hệ thống (thời gian thanh toán không được vượt quá 24 giờ kể từ thời gian đặt vé được ghi nhận). Sau khi ghi nhận đã thanh toán thành công, hành khách sẽ nhận được một phiếu đăng ký hoàn chỉnh nhằm nắm được thông tin về vé mình sở hữu, mã phiếu đăng ký của mỗi bản phiếu đăng ký là duy nhất và gồm các thông tin: họ tên hành khách, thời gian đặt vé, số lượng vé, mã hóa đơn của hóa đơn sau khi hành khách đã thực hiện thanh toán thành công, ID của tài khoản đặt vé và mã tàu mà hành khách sẽ di chuyển. Khách hàng có thể đặt vé nhiều lần trong ngày, khi đó, số lượng vé (số lượng vé một hành khách đặt không được quá 10 vé) và tổng số tiền đã thanh toán sẽ được ghi nhận và gửi cho hành khách tương ứng.

Trên mỗi vé tàu sẽ có đúng một mã tàu mà hành khách sẽ di chuyển, và mỗi tàu sẽ gồm nhiều vé tàu. Mã tàu là duy nhất đối với mỗi tàu, bên cạnh đó, hệ thống sẽ cung cấp thêm những thông tin liên quan đến tàu như sau: thời gian khởi hành, số ghế còn trống, tên trạm nơi tàu xuất phát và tên trạm tàu sẽ dừng lại. Vé tàu chỉ được chấp nhận khi trạm đón và trạm dừng trên vé mà hành khách đã đặt đúng với lộ trình mà tàu đó đi qua.
Mỗi tàu sẽ xuất phát từ một trạm, bên cạnh đó, mỗi trạm sẽ đóng vai trò vừa là trạm đón khách, vừa là trạm dừng để hoàn thành chuyến đi của hành khách, thông tin của trạm gồm: mã trạm và tên trạm, trong đó mã trạm là duy nhất.

Mỗi tàu sẽ được phụ trách bởi ba nhân viên (chỉ tính trong buồng lái tàu), trong đó gồm: một lái chính và hai phụ lái. Với mã nhân viên là duy nhất, những thông tin bổ sung gồm: họ tên nhân viên, tuổi, giới tính và mức lương. Lái chính sẽ đảm nhận trách nhiệm cầm lái trong suốt quá trình tàu di chuyển và cần phải cung cấp thêm thông tin về số năm kinh nghiệm bản thân và số năm kinh nghiệm tối thiểu đối với lái chính là 5 năm, tuy nhiên với những trường hợp bất khả kháng, nhiệm vụ này sẽ được giao lại cho một trong hai phụ lái, và khi đó cần phải đề cập rõ lý do vì sao cần đến sự thay thế.

Song song với việc thanh toán ngay lập tức, hệ thống cho phép hành khách thanh toán trực tuyến trong vòng 24 giờ tính từ thời gian đặt vé, sau khi thanh toán, hành khách sẽ nhận được hóa đơn, bao gồm mã hóa đơn là duy nhất và ghi nhận thêm những thông tin: họ tên hành khách, số tiền thanh toán, phương thức thanh toán (VNPay hoặc MoMo) và thời gian thanh toán. Sau khi hoàn thành xong bước thanh toán, hành khách sẽ được nhận một mã QR trên phiếu đăng ký với chức năng như vé để sử dụng khi lên tàu.

## MÔ TẢ DỮ LIỆU
![image](https://github.com/khanhhao1x/DATABASE/assets/166882051/76856a02-6d23-40b8-9bd0-55442f44a57d)
![image](https://github.com/khanhhao1x/DATABASE/assets/166882051/ef293a1d-dc15-4960-a39e-a4a8e6377fef)

## ERD
![image](https://github.com/khanhhao1x/DATABASE/assets/166882051/7c68db4e-1dff-47cc-b100-0538950a3769)

## MÔ TẢ DỮ LIỆU PHỤ THUỘC KHÓA CHÍNH, KHÓA NGOẠI
![image](https://github.com/khanhhao1x/DATABASE/assets/166882051/3c771a58-00ce-4fb2-8665-10eb427808d9)

