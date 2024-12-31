# -pentesst
Quy trinh kiem tra danh gia
Quy trinh kỉm tra danh gia thong tin
B1:Thu nhap thong tin
	-	SOcial Enginer
	-Thu nhập thông tin kỹ thuật: IP,PORT,service,cve,cms,programing
	- Công cụ: Wapplayzer,Shodan,Censys,..
B2 :Rà quét lỗ hỗng:
	- Quét lỗ hổng hệ thống sử dụng công cụ:Acunetix,Nessus,Nuclei
B3:Khai thác lỗ hổng:
	- Từ kết quả bước1 và bước 2:thực hiện khai thác lỗ hổng
	- Top 10 OWAP:- Ịnection:(SQLI,XSS,CMD,OS,..)
		....
	-chức năng: Login,Register,Đăng bài bình luận
	-API:-Xét phương thức GET,POST,DELETE
	-Xác thực:API có lột lọt thông tin
	- Fuzzing API, xem cac API duoc phep truy cap
	-Input:có mã hoá dữ liệu không, nếu không thì tiến hành khai thác lỗ hỗng Ịnjection
	-Path:xem thử có thư mục nhạy cảm,File backup,data,csdl trên hệ thống ko
	-Payload:Thử qua lần lượt các payload; nếu đúng => trả về kết quả (áp dụng kỹ thuật fuzzing hoặc Intruder trên Burpsuite)
	-CVE:Xem CVE có POC chưa , sử dụng POC để khai thác
	-1 Day:những lỗ hổng chưa có mã khai thác
	-0Day:những lỗ hổng chưa được phát hiện ra
	-review Source: xem thử thông tin lộ lọt tren viewsrource ko , các phương thưc xác thực có phản hồi trên Source ko?
	- Authentication:Kiểm tra phân quyền giữa User / Admin thôgn qua các Prama,ID,URL,phương thức ,giá trị
B4 Tong hop bao cao:
1.Bao cao danh sach lo hong :mô tả chi tiết từng lổ hổng, mức độ nghiêm trọng, tác động và khuyến nghị cho từng lổ hổng
2.Báo cáo đnahs giá hệ thống:từ các kết quả lổ hổng => đánh giá chi tiết vè hệ thống, đưa ra khuyến nghị và khắc phục từng lổ hổng
