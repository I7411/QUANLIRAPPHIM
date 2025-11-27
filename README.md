# QUANLIRAPPHIM
BỘ CÔNG THƯƠNG
TRƯỜNG ĐẠI HỌC CÔNG THƯƠNG THÀNH PHỐ HỒ CHÍ MINH
KHOA CÔNG NGHỆ THÔNG TIN
--------------------------------
 


QUẢN LÝ RẠP CHIẾU PHIM

BÁO CÁO ĐỒ ÁN MÔN HỌC
HỆ QUẢN TRỊ CƠ SỞ DỮ LIỆU
SINH VIÊN THỰC HIỆN:
1.	2001230075, Võ Trí Cường, 14DHTH16
2.	2001230789, Huỳnh Thanh Minh Tâm, 14DHTH02
3.	2001230648, Huỳnh Minh Phát, 14DHTH02
4.	2001230636, Mai Hưng Phát, 14DHTH02
5.	2001230315, Phạm Thành Huy, 14DHTH16
GVHD: ThS. Hoàng Thị Liên Chi





TP. HỒ CHÍ MINH, tháng 12 năm 2025
 
 
BIÊN BẢN LÀM VIỆC
STT	MSSV	Họ tên	Nội dung phân công	Ghi chú
1	2001230075	Võ Trí Cường	Phân công nhiệm vụ + Rà soát dữ liệu + Chỉnh sửa lại CSDL + Ràng buộc default + Làm web app hoàn thiện	Nhóm trưởng
2	2001230789	Huỳnh Thanh Minh Tâm	Ràng buộc unique + Cursor + Lên lịch sao lưu tự động	
3	2001230648	Huỳnh Minh Phát	Ràng buộc check + Function + Giải pháp quản trị người dùng	
4	2001230636	Mai Hưng Phát	Chèn dữ liệu CSDL + Mô tả thuộc tính + Mô tả thuộc tính + Phân quyền người dùng	
5	2001230315	Phạm Thành Huy	Ràng buộc default  + Procedure	

ĐÁNH GIÁ THÀNH VIÊN
STT	MSSV	Họ tên	Tỉ lệ hoàn thành	Ghi chú
1	2001230075	Võ Trí Cường	100%	
2	2001230789	Huỳnh Thanh Minh Tâm	100%	
3	2001230648	Huỳnh Minh Phát	100%	
4	2001230636	Mai Hưng Phát	100%	
5	2001230315	Phạm Thành Huy	100%	

 
MỤC LỤC
MỞ ĐẦU	1
CHƯƠNG 1	XÂY DỰNG CƠ SỞ DỮ LIỆU	2
1.1	Giới thiệu cơ sở dữ liệu:	2
1.2	Các thành phần của cơ sở dữ liệu	2
1.2.1	Tạo bảng	2
1.2.2	Thành phần cơ sở dữ liệu	4
1.3	Thiết lập các ràng buộc	5
1.3.1	Ràng buộc duy nhất (Unique)	6
1.3.2	Ràng buộc kiểm tra (Check)	6
1.3.3	Ràng buộc giá trị mặc định (Default)	8
1.4	Lược đồ diagram	9
1.5	Mô tả chi tiết thuộc tính các bảng	10
1.6	Nhập dữ liệu mẫu	18
1.6.1	Bảng nhân viên	18
1.6.2	Bảng khách hàng	18
1.6.3	Bảng rạp	19
1.6.4	Bảng phim	19
1.6.5	Bảng quầy	20
1.6.6	Bảng phòng chiếu	20
1.6.7	Bảng suất chiếu	20
1.6.8	Bảng ghế	21
1.6.9	Bảng vé	21
1.6.10	Bảng hoá đơn	22
1.6.11	Bảng chi tiết hoá đơn	23
CHƯƠNG 2	CÀI ĐẶT YÊU CẦU XỬ LÝ	23
2.1	Tổng quan về xử lý hệ thống	23
2.2	Cài đặt Stored Procedure	23
2.3	Cài đặt Function	25
2.4	Cài đặt Trigger	26
2.5	Cài đặt Cursor	28
2.6	Cài đặt Transaction	30
CHƯƠNG 3	QUẢN TRỊ HỆ THỐNG	31
3.1	Giới thiệu	31
3.2	Giải pháp quản trị người dùng	31
3.2.1	Cơ chế xác thực	31
3.2.2	Các nhóm người dùng	32
3.3	Tạo Login, User và Role	33
3.3.1	Tạo Login	34
3.3.2	Tạo User	34
3.3.3	Tạo phân quyền (Role)	34
3.3.4	Thu hồi quyền truy cập	34
3.3.5	Cấp quyền thực thi (EXECUTE)	34
3.4	Lập lịch sao lưu định kỳ	34
3.4.1	Mô tả lịch trình sao lưu	34
3.4.2	Lệnh sao lưu cơ sở dữ liệu	35
3.5	Thiết lập sao lưu tự động	36
3.5.1	Tạo công việc sao lưu tự động Full Backup	36
3.5.2	Tạo công việc sao lưu tự động Differential	42
3.5.3	Tạo công việc sao lưu tự động Transaction log	42
3.6	Phục hồi cơ sở dữ liệu	42
3.7	Kết luận	42
CHƯƠNG 4	XÂY DỰNG ỨNG DỤNG	42
4.1	Mục tiêu	42
4.2	Cài đặt ứng dụng	42
4.3	Giao diện ứng dụng	42
4.4	Kết quả	45
4.5	Nhận xét	45
4.6	Tổng kết	45


DANH MỤC HÌNH ẢNH
Hình 1.1 Sơ đồ diagram hệ thống quản lý rạp chiếu phim	10

Hình 3.1 Sơ đồ lịch trình sao lưu cơ sở dữ liệu định kỳ	42

Hình 4.1 Giao diện đăng nhập người dùng	43
Hình 4.2 Giao diện đăng ký tài khoản	43
Hình 4.3 Giao diện Dashboard dành cho quản trị viên, nhân viên bán vé	44
Hình 4.4 Giao diện Dashboard dành cho khách	44


 
DANH MỤC BẢNG
Bảng 1.1 Bảng người dùng dùng cho phần đăng nhập hệ thống	10
Bảng 1.2 Nhân viên của rạp chiếu phim	11
Bảng 1.3 Khách hàng	12
Bảng 1.4 Phim	13
Bảng 1.5 Rạp	13
Bảng 1.6 Quầy bán vé	14
Bảng 1.7 Phòng chiếu	14
Bảng 1 8 Suất chiếu của rạp	15
Bảng 1.9 Ghế ở phòng chiếu phim	15
Bảng 1.10 Vé	16
Bảng 1.11 Hoá đơn của rạp chiếu phim	17
Bảng 1.12 Chi tiết hoá đơn	17

BẢNG DANH MỤC VIẾT TẮT
Tên viết tắt	Tên đầy đủ
SQL	Structured Query Language
T-SQL	Transact-Structured Query Language
CSDL	Cơ sở dữ liệu
	
	


 
 
MỞ ĐẦU
Trong bối cảnh xã hội hiện đại, ngành công nghiệp giải trí, đặc biệt là điện ảnh, đang phát triển mạnh mẽ. Các rạp chiếu phim ngày càng mở rộng quy mô và thu hút lượng lớn khách hàng đến xem phim mỗi ngày. Việc quản lý các hoạt động như đặt vé, quản lý suất chiếu, lập hóa đơn, theo dõi doanh thu và thông tin khách hàng bằng phương pháp thủ công đã trở nên kém hiệu quả dễ đến sai sót thông tin và tốn nhiều thời gian, chi phí.
Vì vậy, việc xây dựng ứng dụng quản lý rạp chiếu phim là hết sức cần thiết nhằm tự động hoá việc quản lý, nâng cao hiệu quả làm việc. Mục tiêu chính là thiết kế xây dựng hệ thống quản lý rạp chiếu phim có khả năng quản lý toàn bộ thông tin và hoạt động của rạp một cách khoa học và chính xác. Các hệ thống được hướng tới bao gồm:
-	Quản lý thông tin phim, rạp, phòng chiếu, suất chiếu.
-	Quản lý vé, khách hàng, nhân viên, quầy bán vé.
-	Hỗ trợ tự động lập hóa đơn, tính tổng tiền và quản lý chi tiết hóa đơn.
-	Cung cấp giao diện dễ sử dụng, giúp nhân viên và khách hàng tra cứu thông tin nhanh chóng.
-	Đảm bảo tính toàn vẹn dữ liệu, bảo mật người dùng và hạn chế trùng lặp thông tin.
Nhờ sự quan tâm, hướng dẫn của cô Hoàng Thị Liên Chi, nhóm em đã từng bước nghiên cứu, vận dụng các kiến thức đã được học nhằm đáp ứng những yêu cầu đã được đặt ra. Tuy nhiên, do kiến thức còn hạn chế nên chương trình vẫn không tránh khỏi những thiếu sót. Vì vậy nhóm chúng em mong nhận được sự đóng góp ý kiến của cô để từng bước xây dựng chương trình ngày càng hoàn thiện và hiệu quả hơn.



Nhóm trưởng nhóm 4
 
CHƯƠNG 1	XÂY DỰNG CƠ SỞ DỮ LIỆU
1.1	Giới thiệu cơ sở dữ liệu:
Hệ thống quản lý Rạp Chiếu Phim được ra đời nhằm đáp ứng những nhu cầu thực tế của khách hàng, nhà quản lý nhằm giải quyết những khó khăn gặp phải, giảm thiểu rủi ro, sai sót phục vụ cho việc lưu trữ, quản lý và xử lý thông tin liên quan đến hoạt động kinh doanh của một rạp chiếu phim hiện đại. 
Hệ thống quản lý Rạp Chiếu Phim được xây dựng trên nền tảng Microsoft SQL Server, sử dụng ngôn ngữ truy vấn T-SQL là một ngôn ngữ mở rộng của SQL hỗ trợ thao tác truy vấn, chèn dữ liệu, thao tác dữ liệu. Ngoài ra, hệ thống còn có chức năng xác thực danh tính dành cho người dùng đăng nhập lần đầu nhằm truy xuất hình ảnh khi cần thiết, tăng cường bảo vệ danh tính người dùng.
Hệ thống có các chức năng chính bao gồm: quản lý phim, quản lý phòng chiếu, quản lý vé, quản lý suất chiếu, quản lý thông tin khách hàng, quản lý nhân viên. Các chức năng này đảm bảo giao diện thân thiện với người dùng. Các chức năng được giới hạn khi phân quyền người dùng, admin có thể thực hiện đầy đủ các chức năng của hệ thống, người dùng chỉ thực hiện mua vé và nhân viên có chức năng quản lý khách hàng.

1.2	Các thành phần của cơ sở dữ liệu
1.2.1	Tạo bảng
CREATE TABLE NHANVIEN
(
    	ID INT IDENTITY(1,1),
    	MANV AS ('NV' + RIGHT('00000000' + CAST(ID AS VARCHAR(8)), 8)) PERSISTED,
TENNV NVARCHAR(80),
	NGAYSINH DATE,
	GIOITINH NVARCHAR(3),
	SDT VARCHAR(15),
	DIACHI NVARCHAR(120),
	EMAIL VARCHAR(50),
	LUONG MONEY,
	CONSTRAINT PK_NHANVIEN PRIMARY KEY (ID)
)

CREATE TABLE KHACHHANG
(
    	ID INT IDENTITY(1,1),
    	MAKH AS ('KH' + RIGHT('00000000' + CAST(ID AS VARCHAR(8)), 8)) PERSISTED,
	TENKH NVARCHAR(80),
	NGAYSINH DATE,
	GIOITINH NVARCHAR(3),
	SDT VARCHAR(15),
	CONSTRAINT PK_KHACHHANG PRIMARY KEY (ID)
)

CREATE TABLE PHIM 
(
	ID INT IDENTITY(1,1),
    	MAPHIM AS ('PH' + RIGHT('00000000' + CAST(ID AS VARCHAR(8)), 8)) PERSISTED,
	TENPHIM NVARCHAR(100),
	THELOAI NVARCHAR(50),
	THOILUONG NVARCHAR(15),
	DIENVIENCHINH NVARCHAR(50),
	KHOICHIEU DATE,
	NGONNGU NVARCHAR(40),
	XEPHANG VARCHAR(10),   -- Xếp hạng dựa trên độ tuổi theo kí hiệu hoặc số (P, 17+, 13+....)
	CONSTRAINT PK_PHIM PRIMARY KEY (ID)      
)

CREATE TABLE RAP 
(
	ID INT IDENTITY(1,1),
    	MARAP AS ('RAP' + RIGHT('0000000' + CAST(ID AS VARCHAR(7)), 7)) PERSISTED,
	TENRAP NVARCHAR(60),
	DIACHI NVARCHAR(100),
	CONSTRAINT PK_RAP PRIMARY KEY (ID)
)

CREATE TABLE QUAY
(
	ID INT IDENTITY(1,1),
    	MAQUAY AS ('QUAY' + RIGHT('000000' + CAST(ID AS VARCHAR(6)), 6)) PERSISTED,
    	TENQUAY NVARCHAR(50),
    	LOAIQUAY NVARCHAR(30),
    	RAP_ID INT NOT NULL,
    	CONSTRAINT PK_QUAY PRIMARY KEY (ID),
    	CONSTRAINT FK_QUAY_RAP FOREIGN KEY (RAP_ID) REFERENCES RAP(ID)
)

CREATE TABLE PHONGCHIEU
(
	ID INT IDENTITY(1,1),
    	MAPH AS ('P' + RIGHT('000000000' + CAST(ID AS VARCHAR(9)), 9)) PERSISTED,
	RAP_ID INT NOT NULL,
	TENPH NVARCHAR(20),
	SOCHO INT,
	CONSTRAINT PK_PHONGCHIEU PRIMARY KEY (ID),
   	CONSTRAINT FK_PHONGCHIEU_RAP FOREIGN KEY (RAP_ID) REFERENCES RAP(ID)
)

CREATE TABLE SUATCHIEU
(
	ID INT IDENTITY(1,1),
   	MASUAT AS ('SU' + RIGHT('00000000' + CAST(ID AS VARCHAR(8)), 8)) PERSISTED,
    	PHIM_ID INT NOT NULL,
	NGAYCHIEU DATE,
	GIOCHIEU TIME,
    	SOGHE VARCHAR (20),
	CONSTRAINT PK_SUATCHIEU PRIMARY KEY (ID),
	CONSTRAINT FK_SUATCHIEU_PHIM FOREIGN KEY (PHIM_ID) REFERENCES PHIM(ID)
)


CREATE TABLE GHE 
(
	ID INT IDENTITY(1,1),
    	MAGHE AS ('GHE' + RIGHT('000000' + CAST(ID AS VARCHAR(6)), 6)) PERSISTED,
	PHONGCHIEU_ID INT NOT NULL,
	RAP_ID INT NOT NULL,
	VITRI NVARCHAR(10),
	LOAIGHE NVARCHAR(10),
	CONSTRAINT PK_GHE PRIMARY KEY (ID, PHONGCHIEU_ID, RAP_ID),
	CONSTRAINT FK_GHE_PHONGCHIEU FOREIGN KEY (PHONGCHIEU_ID) REFERENCES PHONGCHIEU(ID)
)


CREATE TABLE VE
(
    	ID INT IDENTITY(1,1),
    	MAVE AS ('V' + RIGHT('000000' + CAST(ID AS VARCHAR(7)), 7)) PERSISTED,
    	KH_ID INT,
    	SUATCHIEU_ID INT,
    	GHE_ID INT,
	PHIM_ID INT,
	RAP_ID INT,
    	NGAYMUA DATE,
    	GIAVE MONEY,
    	CONSTRAINT PK_VE PRIMARY KEY (ID),
    	CONSTRAINT FK_VE_SUATCHIEU FOREIGN KEY (SUATCHIEU_ID) REFERENCES SUATCHIEU(ID),
    	CONSTRAINT FK_VE_KHACHHANG FOREIGN KEY (KH_ID) REFERENCES KHACHHANG(ID),
    	CONSTRAINT FK_VE_GHE FOREIGN KEY (GHE_ID, PHIM_ID, RAP_ID) REFERENCES GHE(ID, PHONGCHIEU_ID, RAP_ID)
)


CREATE TABLE HOADON
(
	ID INT IDENTITY(1,1),
    	MAHD AS ('HD' + RIGHT('00000000' + CAST(ID AS VARCHAR(8)), 8)) PERSISTED,
    	KH_ID INT,
    	NV_ID INT,
	NGAYLAP DATE,
	TONGTIEN MONEY,
    	CONSTRAINT PK_HOADON PRIMARY KEY (ID),
    	CONSTRAINT FK_HOADON_KHACHHANG FOREIGN KEY (KH_ID) REFERENCES KHACHHANG(ID),
    	CONSTRAINT FK_HOADON_NHANVIEN FOREIGN KEY (NV_ID) REFERENCES NHANVIEN(ID)
)

CREATE TABLE CHITIETHOADON
(
	HOADON_ID INT NOT NULL,
    	VE_ID INT NOT NULL,
    	CONSTRAINT PK_CHITIETHOADON PRIMARY KEY (HOADON_ID, VE_ID),
    	CONSTRAINT FK_CTHD_HOADON FOREIGN KEY (HOADON_ID) REFERENCES HOADON(ID),
    	CONSTRAINT FK_CTHD_VE FOREIGN KEY (VE_ID) REFERENCES VE(ID)
)

1.2.2	Thành phần cơ sở dữ liệu
Cơ sở dữ liệu của hệ thống ứng dụng quản lý rạp chiếu phim được xây dựng nhằm lưu trữ, quản lý và liên kết chặt chẽ các thông tin liên quan đến hoạt động của rạp, bao gồm phim, suất chiếu, vé, khách hàng, nhân viên, hóa đơn, cùng các đối tượng liên quan khác. Mỗi bảng trong cơ sở dữ liệu đóng vai trò quan trọng trong việc đảm bảo hệ thống vận hành hiệu quả, dữ liệu được quản lý nhất quán và có thể truy xuất nhanh chóng khi cần thiết.
Bảng PHIM lưu trữ thông tin chi tiết về các bộ phim đang hoặc sắp được chiếu như mã phim, tên phim, thể loại, thời lượng, diễn viên chính, ngày khởi chiếu, ngôn ngữ và xếp hạng độ tuổi. Bảng này là nền tảng để xác định các suất chiếu và bán vé.
Bảng SUATCHIEU mô tả các suất chiếu cụ thể của từng bộ phim, bao gồm mã suất, mã phim, ngày chiếu, giờ chiếu và thông tin số ghế, giúp hệ thống phân biệt các thời điểm chiếu khác nhau cho cùng một bộ phim.
Bảng RAP và PHONGCHIEU quản lý thông tin về các rạp và phòng chiếu. Bảng RAP lưu thông tin tên rạp, địa chỉ, còn PHONGCHIEU chứa thông tin về các phòng chiếu trong từng rạp như mã phòng, số chỗ ngồi, và mối liên hệ với bảng RAP.
Bảng GHE lưu danh sách ghế trong từng phòng, bao gồm vị trí và loại ghế, giúp quản lý việc đặt vé theo vị trí cụ thể.
Bảng VE quản lý thông tin vé bán ra, liên kết trực tiếp với khách hàng, suất chiếu và ghế. Mỗi vé bao gồm mã vé, mã khách hàng, mã suất chiếu, mã ghế, ngày mua và giá vé.
Bảng KHACHHANG lưu trữ thông tin của khách hàng như mã khách hàng, họ tên, ngày sinh, giới tính, và số điện thoại – là dữ liệu quan trọng cho việc tra cứu, chăm sóc khách hàng và thống kê doanh thu.
Bảng NHANVIEN lưu thông tin nhân sự làm việc tại rạp, bao gồm mã nhân viên, họ tên, ngày sinh, giới tính, số điện thoại, địa chỉ, email và mức lương, phục vụ cho công tác quản lý và phân công nhiệm vụ.
Bảng HOADON ghi nhận thông tin về các hóa đơn thanh toán khi khách hàng mua vé hoặc dịch vụ tại quầy, bao gồm mã hóa đơn, mã khách hàng, mã nhân viên, ngày lập và tổng tiền.
Cuối cùng, bảng CHITIETHOADON thể hiện mối quan hệ giữa hóa đơn và vé, giúp chi tiết hóa các giao dịch đã phát sinh.

1.3	Thiết lập các ràng buộc
Trong cơ sở dữ liệu Hệ thống Quản lý Rạp Chiếu Phim, việc thiết lập các ràng buộc nhằm đảm bảo tính toàn vẹn và chính xác của dữ liệu. Các ràng buộc được sử dụng bao gồm: ràng buộc duy nhất , ràng buộc kiểm tra và ràng buộc mặc định.
1.3.1	Ràng buộc duy nhất (Unique)
-- Bảng RAP
-- Ràng buộc tên rạp duy nhất
ALTER TABLE RAP
ADD CONSTRAINT UQ_RAP_TENRAP UNIQUE (TENRAP)

-- Bảng NHANVIEN
--Ràng buộc địa chỉ email nhân viên duy nhất
ALTER TABLE NHANVIEN
ADD CONSTRAINT UQ_NHANVIEN_EMAIL UNIQUE (EMAIL)

-- Bảng KHACHHANG
--Ràng buộc số điện thoại của khách hàng là duy nhất
ALTER TABLE KHACHHANG
ADD CONSTRAINT UQ_KHACHHANG_SDT UNIQUE (SDT)

-- Bảng PHIM
--Ràng buộc số điện thoại của khách hàng là duy nhất
ALTER TABLE PHIM
ADD CONSTRAINT UQ_PHIM_TENPHIM UNIQUE (TENPHIM)

--Bảng SUATCHIEU
--Ràng buộc một suất chiếu duy nhất tại cùng ngày chiếu và giờ chiếu
ALTER TABLE SUATCHIEU
ADD CONSTRAINT UQ_SUATCHIEU UNIQUE (MASUAT, NGAYCHIEU, GIOCHIEU)

--Bảng QUAY
--Ràng buộc tên quầy là duy nhất
ALTER TABLE QUAY
ADD CONSTRAINT UQ_QUAY_TENRAP UNIQUE (TENQUAY, MARAP)

1.3.2	Ràng buộc kiểm tra (Check)

-- Bảng NHÂN VIÊN
ALTER TABLE NHANVIEN
ADD 
    CONSTRAINT CK_NHANVIEN_GIOITINH CHECK (GIOITINH IN (N'Nam', N'Nữ')), -- Giới tính “nam” hoặc “nữ”
    CONSTRAINT CK_NHANVIEN_NGAYSINH CHECK (NGAYSINH <= GETDATE()), -- Ngày sinh không được lớn hơn ngày hiện tại
    CONSTRAINT CK_NHANVIEN_TUOI CHECK (DATEDIFF(YEAR, NGAYSINH, GETDATE()) >= 18),
    CONSTRAINT CK_NHANVIEN_LUONG CHECK (LUONG >= 1000000), --Lương nhân viên tối thiểu 1 triệu
    CONSTRAINT CK_NHANVIEN_EMAIL_FORMAT CHECK (EMAIL LIKE '%@%.%'); -- Email phải có định dạng @

-- Bảng KHÁCH HÀNG
ALTER TABLE KHACHHANG
ADD 
    CONSTRAINT CK_KHACHHANG_GIOITINH CHECK (GIOITINH IN (N'Nam', N'Nữ')), -- Khách hàng có giới tính “nam” hoặc “nữ”
    CONSTRAINT CK_KHACHHANG_NGAYSINH CHECK (NGAYSINH <= GETDATE()), -- Ngày sinh của khách hàng không được lớn hơn ngày hiện tại
    CONSTRAINT CK_KHACHHANG_TUOI CHECK (DATEDIFF(YEAR, NGAYSINH, GETDATE()) >= 10); -- Kiểm tra khách hàng phải tối thiểu 10 tuổi

-- Bảng PHIM
ALTER TABLE PHIM
ADD 
    CONSTRAINT CK_PHIM_KHOICHIEU CHECK (KHOICHIEU <= GETDATE()),
    CONSTRAINT CK_PHIM_THOILUONG_FORMAT CHECK (ISNUMERIC(THOILUONG) = 1 AND CAST(THOILUONG AS INT) > 0),
    CONSTRAINT CK_PHIM_XEPHANG CHECK (XEPHANG IN ('P', '13+', '16+', '18+')); -- Kiểm tra xếp hạng phim

-- Bảng PHÒNG CHIẾU
ALTER TABLE PHONGCHIEU
ADD CONSTRAINT CK_PHONGCHIEU_SOGHE CHECK (SOGHE > 0); -- Số ghế không được bằng 0 hoặc số âm

-- Bảng SUẤT CHIẾU
ALTER TABLE SUATCHIEU
ADD 
    CONSTRAINT CK_SUATCHIEU_NGAYCHIEU CHECK (NGAYCHIEU <= GETDATE() + 365), 
    CONSTRAINT CK_SUATCHIEU_GIOCHIEU CHECK (GIOCHIEU >= '08:00' AND GIOCHIEU <= '23:00'); -- Giờ chiếu trong khoảng 8:00 đến 23:00

-- Bảng GHẾ
ALTER TABLE GHE
ADD CONSTRAINT CK_GHE_LOAIGHE CHECK (LOAIGHE IN (N'Thường', N'VIP'));

-- Bảng VÉ
ALTER TABLE VE
ADD 
    CONSTRAINT CK_VE_GIAVE CHECK (GIAVE >= 0),
    CONSTRAINT CK_VE_NGAYMUA CHECK (NGAYMUA <= GETDATE());

-- Bảng HÓA ĐƠN
ALTER TABLE HOADON
ADD 
    CONSTRAINT CK_HOADON_NGAYLAP CHECK (NGAYLAP <= GETDATE()), -- Ngày lập không được lớn hơn ngày hiện tại
    CONSTRAINT CK_HOADON_TONGTIEN CHECK (TONGTIEN >= 0)  -- hoá đơn không được tổng tiền là số âm

1.3.3	Ràng buộc giá trị mặc định (Default)
-- BẢNG NHÂN VIÊN

-- Lương nhân viên mặc định là 5 triệu đồng
ALTER TABLE NHANVIEN
ADD CONSTRAINT DF_NHANVIEN_LUONG DEFAULT 5000000 FOR LUONG

-- BẢNG PHIM

--Ngày khởi chiếu mặc định là ngày hiện tại
ALTER TABLE PHIM
ADD CONSTRAINT DF_PHIM_KHOICHIEU DEFAULT (GETDATE()) FOR KHOICHIEU

--Ngôn ngữ mặc định của phim là Tiếng Việt
ALTER TABLE PHIM
ADD CONSTRAINT DF_PHIM_NGONNGU DEFAULT N'Tiếng Việt' FOR NGONNGU

-- Xếp hạng độ tuổi của phim mặc định là 'P'
ALTER TABLE PHIM
ADD CONSTRAINT DF_PHIM_XEPHANG DEFAULT 'P' FOR XEPHANG

-- BẢNG QUẦY
ALTER TABLE QUAY
ADD CONSTRAINT DF_QUAY_LOAI DEFAULT N'Bán vé' FOR LOAIQUAY;

-- BẢNG PHÒNG CHIẾU
--Số ghế ngồi ở phòng chiếu mặc định 100 chỗ ngồi
ALTER TABLE PHONGCHIEU
ADD CONSTRAINT DF_PHONGCHIEU_SOGHE DEFAULT 100 FOR SOGHE

-- BẢNG SUẤT CHIẾU
--Ngày chiếu mặc định là ngày hiện tại trong hệ thống
ALTER TABLE SUATCHIEU
ADD CONSTRAINT DF_SUATCHIEU_NGAY DEFAULT (GETDATE()) FOR NGAYCHIEU

--Giờ chiếu mặc định 18:00
ALTER TABLE SUATCHIEU
ADD CONSTRAINT DF_SUATCHIEU_GIO DEFAULT '18:00' FOR GIOCHIEU

-- BẢNG GHẾ
--Loại ghế mặc định là loại ghế thường
ALTER TABLE GHE
ADD CONSTRAINT DF_GHE_LOAIGHE DEFAULT N'Thường' FOR LOAIGHE;

-- 8. BẢNG VÉ
--Ngày mua vé là ngày hiện tại
ALTER TABLE VE
ADD CONSTRAINT DF_VE_NGAYMUA DEFAULT (GETDATE()) FOR NGAYMUA

--Giá vé mặc định 50000 đồng
ALTER TABLE VE
ADD CONSTRAINT DF_VE_GIAVE DEFAULT 50000 FOR GIAVE;

-- BẢNG HÓA ĐƠN

--Lập hoá đơn có ngày lập là ngày hiện tại
ALTER TABLE HOADON
ADD CONSTRAINT DF_HOADON_NGAYLAP DEFAULT (GETDATE()) FOR NGAYLAP

--Tổng tiền mặc định là 0
ALTER TABLE HOADON
ADD CONSTRAINT DF_HOADON_TONGTIEN DEFAULT 0 FOR TONGTIEN

1.4	Lược đồ diagram
Lược đồ cơ sở dữ liệu (Database Diagram) thể hiện mối quan hệ giữa các bảng dữ liệu trong hệ thống, giúp người thiết kế và người sử dụng dễ dàng hình dung được cấu trúc tổng thể cũng như liên kết logic giữa các thực thể.Lược đồ diagram tổng cộng có 11 bảng chính bao gồm: KHACHHANG, NHANVIEN, PHIM, VE, SUATCHIEU, QUAY, RAP, PHONGCHIEU, GHE, HOADON và CHITIETHOADON.
 
Hình 1.1 Sơ đồ diagram hệ thống quản lý rạp chiếu phim

1.5	Mô tả chi tiết thuộc tính các bảng
Các bảng trong hệ thống Rạp chiếu phim bao gồm 12 bảng được mô tả chi tiết như sau:
Bảng NGUOIDUNG (USERNAME, PASSWORD, ROLE, FACEPICTURE, CREATEAT, VERIFIED)
Tên cột	Diễn giải	Kiểu dữ liệu	Ràng buộc
USERNAME	Tên người dùng	VARCHAR (100)	Khoá chính, Not null
PASSWORD	Mật khẩu	VARCHAR (100)	
ROLE	Vai trò	NVARCHAR (15)	
FACEPICTURE	Hình khuôn mặt	VARBINARY(MAX)	
CREATEAT	Thời điểm tạo	DATETIME	
VERIFIED	Đã xác minh	BIT	
Bảng 1.1 Bảng người dùng dùng cho phần đăng nhập hệ thống
Mô tả:  Bảng NGUOIDUNG lưu trữ thông tin về thông tin người dùng đăng nhập. Thuộc tính bao gồm:
-	USERNAME: là tên người dùng duy nhất có kiểu VARCHAR (100)
-	PASSWORD: là mật khẩu của người dùng, kiểu VARCHAR(100).
-	ROLE: ghi nhận ngày sinh của nhân viên, kiểu DATE.
-	FACEPICTURE: Lưu trữ hình ảnh danh tính người dùng, kiểu VARBINARY(MAX).
-	CREATEAT: là thời điểm tạo tài khoản, kiểu DATETIME.
-	VERIFIED: đã xác minh hay chưa, kiểu BIT.

Bảng NHANVIEN (MANV, TENNV, NGAYSINH, GIOITINH, SDT, DIACHI, EMAIL, LUONG)
Tên cột	Diễn giải	Kiểu dữ liệu	Ràng buộc
MANV	Mã nhân viên	CHAR(10)	Khóa chính, Not null
TENNV	Tên nhân viên	NVARCHAR(80)	
NGAYSINH	Ngày sinh	DATE	
GIOITINH	Giới tính	NVARCHAR(3)	
SDT	Số điện thoại	VARCHAR(15)	
DIACHI	Địa chỉ	NVARCHAR(120)	
EMAIL	Email liên hệ	VARCHAR(50)	
LUONG	Lương nhân viên	MONEY	
Bảng 1.2 Nhân viên của rạp chiếu phim
Mô tả: Bảng NHANVIEN lưu trữ thông tin về nhân viên đang làm việc tại rạp chiếu phim.
-	MANV: là mã định danh duy nhất của nhân viên, kiểu CHAR(10), khóa chính và không được để trống.
-	TENNV: là họ và tên đầy đủ của nhân viên, kiểu NVARCHAR(80).
-	NGAYSINH: ghi nhận ngày sinh của nhân viên, kiểu DATE.
-	GIOITINH: cho biết giới tính của nhân viên (Nam/Nữ), kiểu NVARCHAR(3).
-	SDT: là số điện thoại liên hệ của nhân viên, kiểu VARCHAR(15).
-	DIACHI: lưu địa chỉ nơi ở của nhân viên, kiểu NVARCHAR(120).
-	EMAIL: là địa chỉ thư điện tử để liên hệ, kiểu VARCHAR(50).
-	LUONG: thể hiện mức lương hiện tại của nhân viên, kiểu MONEY.

Bảng KHACHHANG (MAKH, TENKH, NGAYSINH, GIOITINH, SDT)
Tên cột	Diễn giải	Kiểu dữ liệu	Ràng buộc
MAKH	Mã khách hàng	CHAR(10)	Khóa chính, Not null
TENKH	Tên khách hàng	NVARCHAR(80)	
NGAYSINH	Ngày sinh	DATE	
GIOITINH	Giới tính	NVARCHAR(3)	
SDT	Số điện thoại	VARCHAR(15)	
Bảng 1.3 Khách hàng
Mô tả: Bảng KHACHHANG quản lý thông tin của khách hàng đến rạp.
-	MAKH: là mã khách hàng, khóa chính kiểu CHAR(10) và không được để trống.
-	TENKH: là họ tên của khách hàng, kiểu NVARCHAR(80).
-	NGAYSINH: lưu ngày sinh của khách hàng, kiểu DATE.
-	GIOITINH: xác định giới tính của khách hàng, kiểu NVARCHAR(3).
-	SDT: là số điện thoại để liên hệ hoặc đặt vé, kiểu VARCHAR(15).

Bảng PHIM (MAPHIM, TENPHIM, THELOAI, THOILUONG, DIENVIENCHINH, KHOICHIEU, NGONNGU, XEPHANG)
Tên cột	Diễn giải	Kiểu dữ liệu	Ràng buộc
MAPHIM	Mã phim	CHAR(10)	Khóa chính, Not null
TENPHIM	Tên phim	NVARCHAR(100)	
THELOAI	Thể loại	NVARCHAR(50)	
THOILUONG	Thời lượng chiếu	NVARCHAR(15)	
DIENVIENCHINH	Diễn viên chính	NVARCHAR(50)	
KHOICHIEU	Ngày khởi chiếu	DATE	
NGONNGU	Ngôn ngữ	NVARCHAR(40)	
XEPHANG	Xếp hạng độ tuổi (P, 13+, 17+...)	VARCHAR(10)	
Bảng 1.4 Phim
Mô tả: Bảng PHIM chứa thông tin về các bộ phim được chiếu tại rạp.
-	MAPHIM: là mã định danh duy nhất cho từng bộ phim, kiểu CHAR(10), khóa chính.
-	TENPHIM: tên của bộ phim, kiểu NVARCHAR(100).
-	THELOAI: thể loại của phim (hành động, hài, kinh dị...), kiểu NVARCHAR(50).
-	THOILUONG: thời lượng chiếu phim, kiểu NVARCHAR(15) (ví dụ: “120 phút”).
-	DIENVIENCHINH: liệt kê diễn viên chính trong phim, kiểu NVARCHAR(50).
-	KHOICHIEU: là ngày bắt đầu khởi chiếu phim, kiểu DATE.
-	NGONNGU: ngôn ngữ trình chiếu của phim, kiểu NVARCHAR(40).
-	XEPHANG: xếp hạng độ tuổi (như P, 13+, 17+), kiểu VARCHAR(10).

Bảng RAP (MARAP, TENRAP, DIACHI)
Tên cột	Diễn giải	Kiểu dữ liệu	Ràng buộc
MARAP	Mã rạp	CHAR(10)	Khóa chính, Not null
TENRAP	Tên rạp	NVARCHAR(60)	
DIACHI	Địa chỉ rạp	NVARCHAR(100)	
Bảng 1.5 Rạp
Mô tả: Bảng RAP lưu thông tin về các rạp chiếu phim trong hệ thống.
-	MARAP: là mã rạp, kiểu CHAR(10), khóa chính, không được trống.
-	TENRAP: là tên của rạp chiếu phim, kiểu NVARCHAR(60).
-	DIACHI: là địa chỉ cụ thể của rạp, kiểu NVARCHAR(100).

Bảng QUAY (MAQUAY, TENQUAY, LOAIQUAY, MARAP)
Tên cột	Diễn giải	Kiểu dữ liệu	Ràng buộc
MAQUAY	Mã quầy	CHAR(10)	Khóa chính, Not null
TENQUAY	Tên quầy	NVARCHAR(50)	
LOAIQUAY	Loại quầy (bán vé, bắp nước...)	NVARCHAR(30)	
MARAP	Mã rạp	CHAR(10)	Khóa ngoại RAP(MARAP)
Bảng 1.6 Quầy bán vé
Mô tả:
Bảng QUAY lưu trữ thông tin liên quan đến quay trong hệ thống quản lý rạp chiếu phim.

Bảng PHONGCHIEU (MAPH, MARAP, TENPH, SOGHE)
Tên cột	Diễn giải	Kiểu dữ liệu	Ràng buộc
MAPH	Mã phòng chiếu	CHAR(10)	Khóa chính, Not null
MARAP	Mã rạp	CHAR(10)	Khóa ngoại RAP(MARAP)
TENPH	Tên phòng chiếu	NVARCHAR(20)	
SOCHO	Số lượng chỗ ngồi  trong phòng	INT	
Bảng 1.7 Phòng chiếu
Mô tả: Bảng PHONGCHIEU quản lý thông tin các phòng chiếu trong mỗi rạp.
-	MAPH: mã phòng chiếu, kiểu CHAR(10), khóa chính.
-	MARAP: mã rạp chứa phòng chiếu, khóa ngoại tham chiếu RAP(MARAP).
-	TENPH: tên hoặc ký hiệu của phòng chiếu, kiểu NVARCHAR(20).
-	SOCHO: số lượng ghế ngồi có trong phòng chiếu, kiểu INT.

Bảng SUATCHIEU (MASUAT, MAPHIM, NGAYCHIEU, GIOCHIEU, SOGHE)
Tên cột	Diễn giải	Kiểu dữ liệu	Ràng buộc
MASUAT	Mã suất chiếu	CHAR(10)	Khóa chính, Not null
MAPHIM	Mã phim	CHAR(10)	Khóa ngoại PHIM(MAPHIM)
NGAYCHIEU	Ngày chiếu	DATE	
GIOCHIEU	Giờ chiếu	TIME	
SOGHE	Mã số ghế	VARCHAR(20)	
Bảng 1 8 Suất chiếu của rạp
Mô tả: Bảng SUATCHIEU lưu trữ thông tin về từng suất chiếu của phim.
-	MASUAT: mã suất chiếu, kiểu CHAR(10), khóa chính.
-	MAPHIM: mã phim được chiếu, khóa ngoại PHIM(MAPHIM).
-	NGAYCHIEU: ngày chiếu phim, kiểu DATE.
-	GIOCHIEU: giờ bắt đầu chiếu, kiểu TIME.
-	SOGHE: mã số ghế được sử dụng trong suất chiếu, kiểu VARCHAR(20).

Bảng GHE (MAGHE, MAPH, MARAP, VITRI, LOAIGHE)
Tên cột	Diễn giải	Kiểu dữ liệu	Ràng buộc
MAGHE	Mã ghế	CHAR(10)	Khóa chính, Not null
MAPH	Mã phòng chiếu	CHAR(10)	Khóa ngoại PHONGCHIEU (MAPH)
MARAP	Mã rạp	CHAR(10)	Khóa ngoại RAP (MARAP)
VITRI	Vị trí ghế	NVARCHAR(10)	
LOAIGHE	Loại ghế (VIP, thường...)	NVARCHAR(10)	
Bảng 1.9 Ghế ở phòng chiếu phim
Mô tả: Bảng GHE mô tả vị trí và loại ghế trong từng phòng chiếu.
-	MAGHE: mã ghế, kiểu CHAR(10), khóa chính.
-	MAPH: mã phòng chiếu chứa ghế, khóa ngoại PHONGCHIEU(MAPH).
-	MARAP: mã rạp tương ứng, khóa ngoại RAP(MARAP).
-	VITRI: vị trí ghế trong phòng (ví dụ: A1, B5...), kiểu NVARCHAR(10).
-	LOAIGHE: loại ghế (VIP, Thường...), kiểu NVARCHAR(10).

Bảng VE (MAVE, MAKH, MASUAT, MAGHE , MAPH, MARAP, NGAYMUA, GIAVE)
Tên cột	Diễn giải	Kiểu dữ liệu	Ràng buộc
MAVE	Mã vé	CHAR(10)	Khóa chính, Not null
MAKH	Mã khách hàng	CHAR(10)	Khóa ngoại KHACHHANG(MAKH)
MASUAT	Mã suất chiếu	CHAR(10)	Khóa ngoại SUATCHIEU (MASUAT)
MAGHE	Mã ghế	CHAR(10)	Khóa ngoại GHE (MAGHE)
MAPH	Mã phòng chiếu	CHAR(10)	
MARAP	Mã rạp	CHAR(10)	
NGAYMUA	Ngày mua vé	DATE	
GIAVE	Giá vé	MONEY	
Bảng 1.10 Vé
Mô tả: Bảng VE lưu trữ thông tin về vé mà khách hàng đặt hoặc mua.
-	MAVE: mã vé, kiểu CHAR(10), khóa chính.
-	MAKH: mã khách hàng, khóa ngoại KHACHHANG(MAKH).
-	MASUAT: mã suất chiếu, khóa ngoại SUATCHIEU(MASUAT).
-	MAGHE: mã ghế được chọn, khóa ngoại GHE(MAGHE).
-	MAPH: mã phòng chiếu, kiểu CHAR(10).
-	MARAP: mã rạp, kiểu CHAR(10).
-	NGAYMUA: ngày khách mua vé, kiểu DATE.
-	GIAVE: giá tiền của vé, kiểu MONEY.

Bảng HOADON (MAHD, MAKH, MANV, NGAYLAP, TONGTIEN)
Tên cột	Diễn giải	Kiểu dữ liệu	Ràng buộc
MAHD	Mã hóa đơn	CHAR(10)	Khóa chính, Not null
MAKH	Mã khách hàng	CHAR(10)	Khóa ngoại KHACHHANG (MAKH)
MANV	Mã nhân viên	CHAR(10)	Khóa ngoại NHANVIEN (MANV)
NGAYLAP	Ngày lập hóa đơn	DATE	
TONGTIEN	Tổng tiền hóa đơn	MONEY	
Bảng 1.11 Hoá đơn của rạp chiếu phim
Mô tả: Bảng HOADON quản lý thông tin các hóa đơn thanh toán của khách hàng.
-	MAHD: mã hóa đơn, kiểu CHAR(10), khóa chính.
-	MAKH: mã khách hàng, khóa ngoại KHACHHANG(MAKH).
-	MANV: mã nhân viên lập hóa đơn, khóa ngoại NHANVIEN(MANV).
-	NGAYLAP: ngày lập hóa đơn, kiểu DATE.
-	TONGTIEN: tổng số tiền thanh toán của hóa đơn, kiểu MONEY.

Bảng CHITIETHOADON (MAHD, MAVE)
Tên cột	Diễn giải	Kiểu dữ liệu	Ràng buộc
MAHD	Mã hóa đơn	CHAR(10)	Khóa chính, Khóa ngoại HOADON(MAHD)
MAVE	Mã vé	CHAR(10)	Khóa chính, Khóa ngoại VE (MAVE)
Bảng 1.12 Chi tiết hoá đơn
Mô tả: Bảng CHITIETHOADON lưu các chi tiết vé thuộc về một hóa đơn cụ thể.
-	MAHD: mã hóa đơn, là khóa chính đồng thời khóa ngoại HOADON(MAHD).
-	MAVE: mã vé, là khóa chính đồng thời khóa ngoại VE(MAVE).

1.6	Nhập dữ liệu mẫu
1.6.1	Bảng nhân viên
INSERT INTO NHANVIEN (TENNV, NGAYSINH, GIOITINH, SDT, DIACHI, EMAIL, LUONG)
VALUES
(N'Nguyễn Văn Anh','2005-05-12',N'Nam','0901234567',N'123 Lê Lợi, Ba Đình, Hà Nội','anhnv@cgv.com.vn',15000000.00),
(N'Trần Thị Bích','2002-11-03',N'Nữ','0912345678',N'45 Trần Phú, Quận Đống Đa, Hà Nội','bichtt@cgv.com.vn',12000000.00),
(N'Lê Văn Cường','2000-02-20',N'Nam','0987654321',N'78 Nguyễn Trãi, Quận 1, TP.HCM','cuonglv@cgv.com.vn',18000000.00),
(N'Phạm Thị Diệp','2006-07-15',N'Nữ','0977123456',N'91 Lý Thường Kiệt, P.Vườn Lài, TP.HCM','dieppt@cgv.com.vn',11000000.00),
(N'Hoàng Văn Em','2001-12-01',N'Nam','0933123456',N'55A Lê Duẩn, Quận 1, TP.HCM','emhv@cgv.com.vn',14000000.00),
(N'Huỳnh Ngọc Bích','2001-12-01',N'Nữ','0933123456',N'321 Văn Cao, P.Phú Thọ Hoà, TP.HCM','bichhn@cgv.com.vn',10000000.00),
(N'Nguyễn Thị Hoa','1999-03-08',N'Nữ','0904567890',N'22 Nguyễn Văn Cừ, Quận 5, TP.HCM','hoant@cgv.com.vn',13000000.00),
(N'Lý Quốc Hùng','2003-04-17',N'Nam','0918787878',N'12 Trần Hưng Đạo, Quận 3, TP.HCM','hunglq@cgv.com.vn',12500000.00),
(N'Đỗ Minh Tuấn','2002-09-22',N'Nam','0909988776',N'59 Bùi Viện, Quận 1, TP.HCM','tuandm@cgv.com.vn',14500000.00),
(N'Nguyễn Thanh Trúc','2004-01-14',N'Nữ','0934567890',N'11 Hai Bà Trưng, Quận 3, TP.HCM','trucnt@cgv.com.vn',11500000.00),
(N'Võ Thị Mai','1998-08-10',N'Nữ','0912789654',N'72 Pasteur, Quận 1, TP.HCM','maivt@cgv.com.vn',15500000.00),
(N'Trần Quốc Khánh','2000-07-05',N'Nam','0981122334',N'99 Nguyễn Văn Linh, Đà Nẵng','khanhtq@cgv.com.vn',16000000.00),
(N'Bùi Thanh Nam','2001-02-18',N'Nam','0978345678',N'35A Nguyễn Huệ, Quận 1, TP.HCM','nambt@cgv.com.vn',13500000.00),
(N'Lâm Hồng Phúc','2003-05-09',N'Nam','0912789543',N'28 Võ Văn Ngân, Thủ Đức, TP.HCM','phuclh@cgv.com.vn',13800000.00),
(N'Nguyễn Hồng Đào','2004-09-23',N'Nữ','0938234567',N'48 Điện Biên Phủ, Quận Bình Thạnh, TP.HCM','daonh@cgv.com.vn',10800000.00),
(N'Trương Minh Hòa','1999-11-19',N'Nam','0977223344',N'61 Nguyễn Thông, Quận 3, TP.HCM','hoatm@cgv.com.vn',16500000.00),
(N'Phan Ngọc Yến','2002-12-03',N'Nữ','0912334455',N'17 Võ Thị Sáu, Quận 3, TP.HCM','yenpn@cgv.com.vn',11200000.00),
(N'Đặng Thanh Huy','2001-06-15',N'Nam','0908789654',N'81 Cách Mạng Tháng 8, Quận 10, TP.HCM','huydt@cgv.com.vn',14200000.00),
(N'Ngô Thị Tâm','2005-03-30',N'Nữ','0937766554',N'102 Lê Văn Sỹ, Quận Phú Nhuận, TP.HCM','tamnt@cgv.com.vn',10000000.00),
(N'Lê Quang Vũ','2007-01-02',N'Nam','0983456789',N'29 Nguyễn Kiệm, Quận Gò Vấp, TP.HCM','vulq@cgv.com.vn',17500000.00);

1.6.2	Bảng khách hàng 
INSERT INTO KHACHHANG (TENKH, NGAYSINH, GIOITINH, SDT)
VALUES
(N'Nguyễn Văn Khanh', '1995-01-10', N'Nam', '0909988776'),
(N'Trần Thị Loan', '1993-04-22', N'Nữ', '0911223344'),
(N'Lê Thị M', '1988-09-30', N'Nữ', '0977665544'),
(N'Phạm Văn Nam', '2000-06-05', N'Nam', '0988776655'),
(N'Đỗ Thị Tâm', '1997-03-14', N'Nữ', '0904455667'),
(N'Vũ Văn Phúc', '1984-12-25', N'Nam', '0915566778'),
(N'Bùi Thị Quyên', '1991-08-08', N'Nữ', '0923344556'),
(N'Nguyễn Thị Nga', '1999-02-02', N'Nữ', '0932233445'),
(N'Trần Văn Sang', '1982-10-11', N'Nam', '0945566778'),
(N'Hồ Thị Thu', '1996-07-07', N'Nữ', '0956677889'),
(N'Lê Văn Hậu', '1990-09-12', N'Nam', '0903344556'),
(N'Ngô Thị Mai', '1998-11-23', N'Nữ', '0917788990'),
(N'Phan Văn Toàn', '1985-05-30', N'Nam', '0926677889'),
(N'Đặng Thị Duyên', '1999-01-18', N'Nữ', '0935566778'),
(N'Trương Văn Long', '1987-03-10', N'Nam', '0944455667'),
(N'Hoàng Thị Kim', '1994-12-05', N'Nữ', '0953344556'),
(N'Nguyễn Văn Tài', '1992-06-25', N'Nam', '0962233445'),
(N'Lý Thị Thuỷ', '2001-04-08', N'Nữ', '0971122334'),
(N'Tạ Văn Quang', '1983-02-27', N'Nam', '0980011223'),
(N'Đoàn Thị Hồng', '1997-08-19', N'Nữ', '0998899001')

1.6.3	Bảng rạp
INSERT INTO RAP (TENRAP, DIACHI)
VALUES
(N'CGV Vincom Center Thủ Đức', N'Vincom Center, 216 Võ Văn Ngân, P.Thủ Đức, TP.HCM'),
(N'Galaxy Cinema - Vincom', N'Vincom Mega Mall Smart City, KĐT Vinhomes Smart City, P. Đại Mỗ, Hà Nội'),
(N'Lotte Cinema - AEON Mall', N'AEON Mall Bình Tân, 1 Đường Số 17A, P.An Lạc, TP. Hồ Chí Minh'),
(N'CGV Aeon Tân Phú', N'Aeon Mall Tân Phú , 30 Tân Thắng, P.Tân Sơn Nhì, TP.HCM'),
(N'CGV Hoàng Văn Thụ', N' 415 Hoàng Văn Thụ, Phường Tân Sơn Hoà, TP.Hồ Chí Minh'),
(N'CGV Thảo Điền Pearl', N'Tầng 2, Thảo Điền Mall, 12 Quốc Hương, P. Thảo Điền, Q.2, Tp. Hồ Chí Minh'),
(N'CGV Liberty Citypoint', N'Tầng M – 1, Liberty Center Saigon Citypoint, 59 – 61 Pasteur, Q.1, Tp. Hồ Chí Minh'),
(N'CGV Vivo City', N'Lầu 5, TTTM SC VivoCity, 1058 Nguyễn Văn Linh, Q.7, Tp. Hồ Chí Minh'),
(N'CGV Pearl Plaza', N'Tầng 5, Pearl Plaza, 561A Điện Biên Phủ, P.25, Q. Bình Thạnh, Tp. Hồ Chí Minh'),
(N'CGV Vincom Landmark 81', N'B1, Vincom Center Landmark 81, 722 Điện Biên Phủ, P. 22, Q. Bình Thạnh, Tp. Hồ Chí Minh')

1.6.4	Bảng phim
INSERT INTO PHIM (TENPHIM, THELOAI, THOILUONG, DIENVIENCHINH, KHOICHIEU, NGONNGU, XEPHANG)
VALUES
(N'Colorful Stage! Một Miku không thể hát', N'Hoạt hình', N'105 phút', 'Saki Fujita', '2025-06-13', N'Tiếng Nhật', 'PG'),
(N'Mưa đỏ', N'Lịch sử/Chiến tranh', N'124 phut', N'Đỗ Nhật Hoàng', '2025-08-22', N'Tiếng Việt', 'T13'),
(N'Một bộ phim Minecraft', N'Hài/Phiêu lưu','101 phut','Jack Black', '2025-04-04', N'Tiếng Anh', 'PG'),
(N'Địa đạo: Mặt trời trong bóng tối', N'Lịch sử/Chiến tranh','125 phút', N'Thái Hoà','2025-04-04', N'Tiếng Việt', NULL),
(N'TRẬN CHIẾN SAU TRẬN CHIẾN', N'Hành Động, Hồi hộp, Tâm Lý','162 phút', 'Leonardo DiCaprio','2025-09-26', N'Tiếng Anh – phụ đề Tiếng Việt', 'T18'),
(N'LÀM GIÀU VỚI MA 2: CUỘC CHIẾN HỘT XOÀN', N'Hài, Hành Động','125 phút', 'Trung Lùn','2025-08-29', N'Tiếng Anh – phụ đề Tiếng Việt', 'T16')


1.6.5	Bảng quầy
INSERT INTO QUAY (TENQUAY, LOAIQUAY, RAP_ID)
VALUES
(N'Quầy số 1', N'Bán vé', 1),
(N'Quầy số 2', N'Bán vé', 1),
(N'Quầy số 3', N'Bán vé', 2),
(N'Quầy số 4', N'Bán vé', 2),
(N'Quầy số 5', N'Bán vé', 3),
(N'Quầy số 6', N'Bán vé', 3),
(N'Quầy số 7', N'Bán vé', 1),
(N'Quầy số 8', N'Bán vé', 2),
(N'Quầy số 9', N'Bán vé', 3),
(N'Quầy số 10', N'Bán vé', 1),
(N'Quầy đồ ăn 1', N'Bán đồ ăn và giải khát', 1),
(N'Quầy đồ ăn 2', N'Bán đồ ăn và giải khát', 2),
(N'Quầy đồ ăn 3', N'Bán đồ ăn và giải khát', 3),
(N'Quầy đồ ăn 4', N'Bán đồ ăn và giải khát', 1),
(N'Quầy đồ ăn 5', N'Bán đồ ăn và giải khát', 2)

1.6.6	Bảng phòng chiếu
-- Rạp 1: ID = 1
INSERT INTO PHONGCHIEU (TENPH, SOCHO, RAP_ID)
VALUES
(N'Phòng 1', 150, 1),
(N'Phòng 2', 160, 1),
(N'Phòng 3', 170, 1),
(N'Phòng 4', 180, 1),
(N'Phòng 5', 190, 1),

-- Rạp 2: ID = 2
(N'Phòng 1', 140, 2),
(N'Phòng 2', 150, 2),
(N'Phòng 3', 160, 2),
(N'Phòng 4', 170, 2),
(N'Phòng 5', 180, 2),

-- Rạp 3: ID = 3
(N'Phòng 1', 140, 3),
(N'Phòng 2', 150, 3),
(N'Phòng 3', 160, 3),
(N'Phòng 4', 170, 3),
(N'Phòng 5', 180, 3)

1.6.7	Bảng suất chiếu
INSERT INTO SUATCHIEU (PHIM_ID, NGAYCHIEU, GIOCHIEU)
VALUES
(1, '2025-09-25', '18:00'),
(2, '2025-09-25', '20:00'),
(3, '2025-09-26', '16:00'),
(4, '2025-09-26', '19:30'),
(5, '2025-09-27', '14:00'),
(6, '2025-09-27', '17:00'),
(1, '2025-09-28', '13:30'),
(2, '2025-09-28', '15:30'),
(3, '2025-09-28', '18:00'),
(4, '2025-09-28', '20:30'),
(5, '2025-09-29', '10:00'),
(6, '2025-09-29', '12:30'),
(1, '2025-09-29', '15:00'),
(2, '2025-09-29', '18:00'),
(3, '2025-09-29', '20:30'),
(4, '2025-09-30', '09:00'),
(5, '2025-09-30', '11:00'),
(6, '2025-09-30', '13:30'),
(1, '2025-09-30', '16:00'),
(2, '2025-09-30', '19:30')

1.6.8	Bảng ghế
INSERT INTO GHE (MAGHE, MAPH, MARAP, VITRI, LOAIGHE)
VALUES
('GHE001', 'P001', 'RAP001', 'A1', N'Thường'),
('GHE002', 'P001', 'RAP001', 'A2', N'Thường'),
('GHE003', 'P001', 'RAP001', 'B1', 'VIP'),
('GHE004', 'P001', 'RAP001', 'B2','VIP'),
('GHE005', 'P002', 'RAP001', 'C1', N'Thường'),
('GHE006', 'P002', 'RAP001', 'C2', N'Thường'),
('GHE007', 'P003', 'RAP002', 'A1', N'Thường'),
('GHE008', 'P003', 'RAP002', 'A2', 'VIP'),
('GHE009', 'P003', 'RAP002', 'B1', N'Thường'),
('GHE010', 'P004', 'RAP002', 'B2', 'VIP');


1.6.9	Bảng vé
INSERT INTO VE (MAVE, MAKH, MASUAT, NGAYMUA, GIAVE)
VALUES
('V001', 'KH001', 'SU001', '2025-09-25', 120000),
('V002', 'KH002', 'SU002', '2025-09-25', 150000),
('V003', 'KH003', 'SU003', '2025-09-26', 100000),
('V004', 'KH004', 'SU004', '2025-09-26', 130000),
('V005', 'KH005', 'SU005', '2025-09-27', 140000),
('V006', 'KH006', 'SU006', '2025-09-27', 160000)

1.6.10	Bảng hoá đơn
INSERT INTO HOADON (MAHD, MAKH, MANV, NGAYLAP, TONGTIEN)
VALUES
('HD001', 'KH001', 'NV001', '2025-09-25', NULL),
('HD002', 'KH002', 'NV002', '2025-09-25', NULL),
('HD003', 'KH003', 'NV003', '2025-09-26', NULL),
('HD004', 'KH004', 'NV004', '2025-09-26', NULL),
('HD005', 'KH005', 'NV005', '2025-09-27', NULL),
('HD006', 'KH006', 'NV006', '2025-09-27', NULL),
('HD007', 'KH007', 'NV001', '2025-09-27', NULL),
('HD008', 'KH008', 'NV002', '2025-09-27', NULL),
('HD009', 'KH009', 'NV003', '2025-09-28', NULL),
('HD010', 'KH010', 'NV004', '2025-09-28', NULL),
('HD011', 'KH001', 'NV005', '2025-09-28', NULL),
('HD012', 'KH002', 'NV006', '2025-09-28', NULL),
('HD013', 'KH003', 'NV001', '2025-09-29', NULL),
('HD014', 'KH004', 'NV002', '2025-09-29', NULL),
('HD015', 'KH005', 'NV003', '2025-09-29', NULL),
('HD016', 'KH006', 'NV004', '2025-09-29', NULL),
('HD017', 'KH007', 'NV005', '2025-09-30', NULL),
('HD018', 'KH008', 'NV006', '2025-09-30', NULL),
('HD019', 'KH009', 'NV001', '2025-09-30', NULL),
('HD020', 'KH010', 'NV002', '2025-09-30', NULL),
('HD021', 'KH001', 'NV003', '2025-09-30', NULL),
('HD022', 'KH002', 'NV004', '2025-09-30', NULL),
('HD023', 'KH003', 'NV005', '2025-09-30', NULL),
('HD024', 'KH004', 'NV006', '2025-09-30', NULL),
('HD025', 'KH005', 'NV001', '2025-09-30', NULL),
('HD026', 'KH006', 'NV002', '2025-09-30', NULL),
('HD027', 'KH007', 'NV003', '2025-09-30', NULL),
('HD028', 'KH008', 'NV004', '2025-09-30', NULL),
('HD029', 'KH009', 'NV005', '2025-09-30', NULL),
('HD030', 'KH010', 'NV006', '2025-09-30', NULL)

1.6.11	Bảng chi tiết hoá đơn
    INSERT INTO CHITIETHOADON (HOADON_ID, VE_ID)
    VALUES
    (1, 1),
    (2, 2),
    (3, 3),
    (4, 4),
    (5, 5)

CHƯƠNG 2	CÀI ĐẶT YÊU CẦU XỬ LÝ
2.1	Tổng quan về xử lý hệ thống
Xử lý cơ sở dữ liệu nhằm giúp hệ thống đảm bảo vận hành một cách tự động chính xác, trơn tru nhất. Các xử lý dữ liệu được cài đặt đảm bảo được tính toàn vẹn dữ liệu trong quá trình thêm, xoá, sửa, tránh tình trạng không được trùng dữ liệu cũng như thay đổi vượt quá yêu cầu đưa ra.
Các yêu cầu xử lý được đưa bao gồm: Stored Procedure, Function, Trigger, Cursor và Transaction.

2.2	Cài đặt Stored Procedure
--Thêm khách hàng mới
CREATE PROCEDURE sp_ThemKhachHang
  @TENKH NVARCHAR(100), @NGAYSINH DATE, @GIOITINH NVARCHAR(10), @SDT VARCHAR(10)
AS
BEGIN
  IF EXISTS (SELECT 1 FROM KHACHHANG WHERE SDT = @SDT)
  BEGIN
    RAISERROR (N'Số điện thoại đã tồn tại.', 16, 1); RETURN;
  END
  INSERT INTO KHACHHANG (TENKH, NGAYSINH, GIOITINH, SDT)
  VALUES (@TENKH, @NGAYSINH, @GIOITINH, @SDT);
END
GO

--Cập nhật lương nhân viên
CREATE PROCEDURE sp_CapNhatLuongNhanVien
  @MANV CHAR(10), @LUONGMOI MONEY
AS
BEGIN
  DECLARE @NhanVienID INT = (SELECT ID FROM NHANVIEN WHERE MANV = @MANV);
  IF @NhanVienID IS NULL
  BEGIN
    RAISERROR (N'Không tìm thấy nhân viên.', 16, 1); RETURN;
  END
  UPDATE NHANVIEN SET LUONG = @LUONGMOI WHERE ID = @NhanVienID;
END
GO

--Tính doanh thu ngày
CREATE PROCEDURE sp_TinhDoanhThuNgay
  @NGAY DATE
AS
BEGIN
  DECLARE @DOANHTHU MONEY;
  SELECT @DOANHTHU = SUM(TONGTIEN)
  FROM HOADON
  WHERE CONVERT(DATE, NGAYLAP) = @NGAY;
  SET @DOANHTHU = ISNULL(@DOANHTHU, 0);
  PRINT N'Tổng doanh thu ngày ' + CONVERT(NVARCHAR(20), @NGAY, 103) + N' là: ' + CAST(@DOANHTHU AS NVARCHAR(30)) + N' đồng.';
  SELECT @DOANHTHU AS DOANHTHU;
END
GO

--Liệt kê vé theo khách hàng
CREATE PROCEDURE sp_LietKeVeTheoKhachHang
  @MAKH CHAR(10)
AS
BEGIN
  DECLARE @KhachHangID INT = (SELECT ID FROM KHACHHANG WHERE MAKH = @MAKH);
  SELECT V.MAVE, SC.MASUAT, V.NGAYMUA, V.GIAVE, P.TENPHIM
  FROM VE V
  JOIN SUATCHIEU SC ON V.SUATCHIEU_ID = SC.ID
  JOIN PHIM P ON SC.PHIM_ID = P.ID
  WHERE V.KH_ID = @KhachHangID;
END
GO

--Thêm một bộ phim mới
CREATE PROCEDURE sp_ThemPhim
  @TENPHIM NVARCHAR(100), @THELOAI NVARCHAR(50), @THOILUONG NVARCHAR(20),
  @DIENVIENCHINH NVARCHAR(100), @KHOICHIEU DATE,
  @NGONNGU NVARCHAR(50) = N'Tiếng Việt', @XEPHANG NVARCHAR(10) = NULL
AS
BEGIN
  IF EXISTS (SELECT 1 FROM PHIM WHERE TENPHIM = @TENPHIM)
  BEGIN
    RAISERROR (N'Tên phim đã tồn tại.', 16, 1); RETURN;
  END
  INSERT INTO PHIM (TENPHIM, THELOAI, THOILUONG, DIENVIENCHINH, KHOICHIEU, NGONNGU, XEPHANG, HINH)
  VALUES (@TENPHIM, @THELOAI, @THOILUONG, @DIENVIENCHINH, @KHOICHIEU, @NGONNGU, @XEPHANG, NULL);
END
GO

2.3	Cài đặt Function
--Thêm khách hàng mới
CREATE PROCEDURE sp_ThemKhachHang
  @TENKH NVARCHAR(100), @NGAYSINH DATE, @GIOITINH NVARCHAR(10), @SDT VARCHAR(10)
AS
BEGIN
  IF EXISTS (SELECT 1 FROM KHACHHANG WHERE SDT = @SDT)
  BEGIN
    RAISERROR (N'Số điện thoại đã tồn tại.', 16, 1); RETURN;
  END
  INSERT INTO KHACHHANG (TENKH, NGAYSINH, GIOITINH, SDT)
  VALUES (@TENKH, @NGAYSINH, @GIOITINH, @SDT);
END
GO

--Cập nhật lương nhân viên
CREATE PROCEDURE sp_CapNhatLuongNhanVien
  @MANV CHAR(10), @LUONGMOI MONEY
AS
BEGIN
  DECLARE @NhanVienID INT = (SELECT ID FROM NHANVIEN WHERE MANV = @MANV);
  IF @NhanVienID IS NULL
  BEGIN
    RAISERROR (N'Không tìm thấy nhân viên.', 16, 1); RETURN;
  END
  UPDATE NHANVIEN SET LUONG = @LUONGMOI WHERE ID = @NhanVienID;
END
GO

--Tính doanh thu ngày
CREATE PROCEDURE sp_TinhDoanhThuNgay
  @NGAY DATE
AS
BEGIN
  DECLARE @DOANHTHU MONEY;
  SELECT @DOANHTHU = SUM(TONGTIEN)
  FROM HOADON
  WHERE CONVERT(DATE, NGAYLAP) = @NGAY;
  SET @DOANHTHU = ISNULL(@DOANHTHU, 0);
  PRINT N'Tổng doanh thu ngày ' + CONVERT(NVARCHAR(20), @NGAY, 103) + N' là: ' + CAST(@DOANHTHU AS NVARCHAR(30)) + N' đồng.';
  SELECT @DOANHTHU AS DOANHTHU;
END
GO

--Liệt kê vé theo khách hàng
CREATE PROCEDURE sp_LietKeVeTheoKhachHang
  @MAKH CHAR(10)
AS
BEGIN
  DECLARE @KhachHangID INT = (SELECT ID FROM KHACHHANG WHERE MAKH = @MAKH);
  SELECT V.MAVE, SC.MASUAT, V.NGAYMUA, V.GIAVE, P.TENPHIM
  FROM VE V
  JOIN SUATCHIEU SC ON V.SUATCHIEU_ID = SC.ID
  JOIN PHIM P ON SC.PHIM_ID = P.ID
  WHERE V.KH_ID = @KhachHangID;
END
GO

--Thêm một bộ phim mới
CREATE PROCEDURE sp_ThemPhim
  @TENPHIM NVARCHAR(100), @THELOAI NVARCHAR(50), @THOILUONG NVARCHAR(20),
  @DIENVIENCHINH NVARCHAR(100), @KHOICHIEU DATE,
  @NGONNGU NVARCHAR(50) = N'Tiếng Việt', @XEPHANG NVARCHAR(10) = NULL
AS
BEGIN
  IF EXISTS (SELECT 1 FROM PHIM WHERE TENPHIM = @TENPHIM)
  BEGIN
    RAISERROR (N'Tên phim đã tồn tại.', 16, 1); RETURN;
  END
  INSERT INTO PHIM (TENPHIM, THELOAI, THOILUONG, DIENVIENCHINH, KHOICHIEU, NGONNGU, XEPHANG, HINH)
  VALUES (@TENPHIM, @THELOAI, @THOILUONG, @DIENVIENCHINH, @KHOICHIEU, @NGONNGU, @XEPHANG, NULL);
END
GO

2.4	Cài đặt Trigger
CREATE TRIGGER TRG_NHANVIEN_MASTER_UPDATE
ON NHANVIEN
AFTER UPDATE
AS
BEGIN
    SET NOCOUNT ON;
    -- 1. Kiểm tra giảm lương
    IF UPDATE(LUONG) AND EXISTS (SELECT 1 FROM inserted i JOIN deleted d ON i.ID = d.ID WHERE i.LUONG < (d.LUONG * 0.5))
    BEGIN
        RAISERROR(N'Không được giảm lương nhân viên quá 50%%.', 16, 1)
        ROLLBACK TRANSACTION; RETURN;
    END
    -- 2. Kiểm tra trùng SDT
    IF UPDATE(SDT) AND EXISTS (SELECT 1 FROM NHANVIEN n JOIN inserted i ON n.SDT = i.SDT WHERE n.ID <> i.ID)
    BEGIN
        RAISERROR(N'Lỗi: SĐT đã tồn tại cho nhân viên khác.', 16, 1)
        ROLLBACK TRANSACTION; RETURN;
    END;
    -- 3. Ghi Log
    IF UPDATE(LUONG)
        INSERT INTO LOG_NHANVIEN(NHANVIEN_ID, TENNV, HANHDONG) SELECT ID, TENNV, 'UPDATE_LUONG' FROM inserted
    IF UPDATE(DIACHI)
        INSERT INTO LOG_NHANVIEN(NHANVIEN_ID, TENNV, HANHDONG) SELECT ID, TENNV, 'UPDATE_DIACHI' FROM inserted
    IF (UPDATE(TENNV) OR UPDATE(EMAIL))
        INSERT INTO LOG_NHANVIEN(NHANVIEN_ID, TENNV, HANHDONG) SELECT ID, TENNV, 'UPDATE_OTHER' FROM inserted
END
GO

-- Trigger trên PHIM (Kiểm tra trùng tên)
CREATE TRIGGER TRG_PHIM_KET_HOP
ON PHIM
AFTER INSERT, UPDATE
AS
BEGIN
    SET NOCOUNT ON;
    IF EXISTS (SELECT 1 FROM INSERTED i WHERE EXISTS (SELECT 1 FROM PHIM p WHERE p.TENPHIM = i.TENPHIM AND p.ID <> i.ID))
    BEGIN
        RAISERROR(N'Lỗi: Tên phim đã tồn tại!', 16, 1);
        ROLLBACK TRANSACTION; RETURN;
    END;
END;
GO

-- Trigger trên KHACHHANG (Kiểm tra SDT 10 số)
CREATE TRIGGER TRG_KHACHHANG_SDT
ON KHACHHANG
AFTER INSERT, UPDATE
AS
BEGIN
    -- (SỬA: Bỏ kiểm tra LIKE '%[^0-9]%' vì SDT của bạn có 0909988776)
    IF EXISTS (SELECT 1 FROM INSERTED WHERE LEN(SDT) <> 10)
    BEGIN
        RAISERROR(N'Số điện thoại phải đúng 10 chữ số!', 16, 1);
        ROLLBACK TRANSACTION;
    END
END
GO

-- Trigger trên CHITIETHOADON (Để tự động tính TONGTIEN cho HOADON)
CREATE TRIGGER TRG_CHITIETHOADON_TinhTongTien
ON CHITIETHOADON
AFTER INSERT, UPDATE, DELETE
AS
BEGIN
    SET NOCOUNT ON;
    DECLARE @AffectedHoadonIDs TABLE (ID INT PRIMARY KEY);
    INSERT INTO @AffectedHoadonIDs (ID) SELECT HOADON_ID FROM inserted;
    INSERT INTO @AffectedHoadonIDs (ID) SELECT HOADON_ID FROM deleted;

    UPDATE HOADON
    SET TONGTIEN = (
        SELECT ISNULL(SUM(v.GIAVE), 0)
        FROM CHITIETHOADON cthd
        JOIN VE v ON cthd.VE_ID = v.ID
        WHERE cthd.HOADON_ID = HOADON.ID
    )
    WHERE HOADON.ID IN (SELECT ID FROM @AffectedHoadonIDs);
END
GO

-- Trigger trên VE (Chặn đặt vé cũ)
CREATE TRIGGER trg_Insert_VE
ON VE
INSTEAD OF INSERT
AS
BEGIN
    IF EXISTS (
        SELECT 1 FROM SUATCHIEU sc JOIN inserted i ON sc.ID = i.SUATCHIEU_ID
        WHERE (sc.NGAYCHIEU < CAST(GETDATE() AS DATE)) OR 
              (sc.NGAYCHIEU = CAST(GETDATE() AS DATE) AND sc.GIOCHIEU < CAST(GETDATE() AS TIME))
    )
    BEGIN
        RAISERROR(N'Suất chiếu đã qua, không thể đặt vé.', 16, 1); RETURN
    END
    INSERT INTO VE (KH_ID, SUATCHIEU_ID, GHE_ID, NGAYMUA, GIAVE)
    SELECT KH_ID, SUATCHIEU_ID, GHE_ID, NGAYMUA, GIAVE FROM inserted
END
GO


2.5	Cài đặt Cursor
-- In danh sách suất chiếu 7 ngày tới (SỬA: Dùng ID)
PRINT N'Running Cursor 1: In danh sách suất chiếu 7 ngày tới...';
GO
DECLARE @Suat_ID INT, @Phim_ID INT,
        @TenPhim NVARCHAR(100), @NgayChieu DATE, @GioChieu TIME;

DECLARE cur_Suat CURSOR FAST_FORWARD FOR
SELECT ID, PHIM_ID, NGAYCHIEU, GIOCHIEU
FROM SUATCHIEU
WHERE NGAYCHIEU BETWEEN CAST(GETDATE() AS DATE) AND DATEADD(DAY, 7, CAST(GETDATE() AS DATE))
ORDER BY NGAYCHIEU, GIOCHIEU;

OPEN cur_Suat;
FETCH NEXT FROM cur_Suat INTO @Suat_ID, @Phim_ID, @NgayChieu, @GioChieu;

WHILE @@FETCH_STATUS = 0
BEGIN
    SELECT @TenPhim = TENPHIM FROM PHIM WHERE ID = @Phim_ID;
    PRINT N'ID Suất: ' + CAST(@Suat_ID AS NVARCHAR(10))
        + N' | Phim: ' + ISNULL(@TenPhim, N'(Không tìm thấy phim)')
        + N' | Ngày: ' + CONVERT(NVARCHAR(10), @NgayChieu, 103)
        + N' | Giờ: ' + CONVERT(NVARCHAR(8), @GioChieu, 108)
    FETCH NEXT FROM cur_Suat INTO @Suat_ID, @Phim_ID, @NgayChieu, @GioChieu
END
CLOSE cur_Suat
DEALLOCATE cur_Suat
GO

-- Tăng giá 10% cho vé của phim "Mưa đỏ" (SỬA: Dùng ID)
PRINT N'Running Cursor 2: Tăng giá 10% cho vé của phim "Mưa đỏ"...'
GO
DECLARE @Suat_ID INT
DECLARE cur_Suat CURSOR LOCAL FOR
SELECT S.ID
FROM SUATCHIEU S
INNER JOIN PHIM P ON S.PHIM_ID = P.ID
WHERE P.TENPHIM = N'Mưa đỏ'

OPEN cur_Suat;
FETCH NEXT FROM cur_Suat INTO @Suat_ID

WHILE @@FETCH_STATUS = 0
BEGIN
    UPDATE VE
    SET GIAVE = ROUND(GIAVE * 1.10, 0)
    WHERE SUATCHIEU_ID = @Suat_ID
    FETCH NEXT FROM cur_Suat INTO @Suat_ID
END;
CLOSE cur_Suat
DEALLOCATE cur_Suat
GO

--  Tính tổng tiền cho từng hóa đơn (SỬA: Dùng ID)
PRINT N'Running Cursor 3: Tính tổng tiền cho từng hóa đơn...'
GO
DECLARE @HOADON_ID INT
DECLARE @Total MONEY
DECLARE cur_HD CURSOR LOCAL FOR
SELECT DISTINCT HOADON_ID FROM CHITIETHOADON

OPEN cur_HD
FETCH NEXT FROM cur_HD INTO @HOADON_ID

WHILE @@FETCH_STATUS = 0
BEGIN
    SELECT @Total = SUM(V.GIAVE)
    FROM CHITIETHOADON C
    JOIN VE V ON C.VE_ID = V.ID
    WHERE C.HOADON_ID = @HOADON_ID
    SET @Total = ISNULL(@Total, 0)
    UPDATE HOADON SET TONGTIEN = @Total WHERE ID = @HOADON_ID
    FETCH NEXT FROM cur_HD INTO @HOADON_ID
END;
CLOSE cur_HD
DEALLOCATE cur_HD
GO

-- Xóa vé cũ (cũ hơn 1 năm)
PRINT N'Running Cursor 4: Xóa vé cũ (cũ hơn 1 năm)...'
GO
DECLARE @VE_ID INT
DECLARE cur_OldVe CURSOR FOR
SELECT ID FROM VE WHERE NGAYMUA < DATEADD(YEAR, -1, CAST(GETDATE() AS DATE))

OPEN cur_OldVe;
FETCH NEXT FROM cur_OldVe INTO @VE_ID
WHILE @@FETCH_STATUS = 0
BEGIN
    BEGIN TRY
        BEGIN TRANSACTION;
        DELETE FROM CHITIETHOADON WHERE VE_ID = @VE_ID
        DELETE FROM VE WHERE ID = @VE_ID
        COMMIT TRANSACTION
    END TRY
    BEGIN CATCH
        ROLLBACK TRANSACTION;
        PRINT N'Lỗi khi xóa vé ID = ' + CAST(@VE_ID AS NVARCHAR(10)) + N' - ' + ERROR_MESSAGE()
    END CATCH
    FETCH NEXT FROM cur_OldVe INTO @VE_ID
END
CLOSE cur_OldVe
DEALLOCATE cur_OldVe
GO

--Tính điểm thưởng
PRINT N'Running Cursor 5: Tính điểm thưởng...';
GO
DECLARE @KetQua TABLE (KH_ID INT, TongChi MONEY, DiemThuong INT)
DECLARE @KH_ID INT
DECLARE @TongChi MONEY
DECLARE @DiemMoi INT
DECLARE cur_KH CURSOR LOCAL FOR SELECT ID FROM KHACHHANG

OPEN cur_KH;
FETCH NEXT FROM cur_KH INTO @KH_ID
WHILE @@FETCH_STATUS = 0
BEGIN
    SELECT @TongChi = SUM(TONGTIEN) FROM HOADON WHERE KH_ID = @KH_ID
    SET @TongChi = ISNULL(@TongChi, 0)
    SET @DiemMoi = FLOOR(@TongChi / 100000)
    INSERT INTO @KetQua VALUES (@KH_ID, @TongChi, @DiemMoi)
    FETCH NEXT FROM cur_KH INTO @KH_ID
END
CLOSE cur_KH
DEALLOCATE cur_KH
-- Hiển thị kết quả điểm thưởng
SELECT KH.MAKH, KH.TENKH, KQ.TongChi, KQ.DiemThuong
FROM @KetQua KQ
JOIN KHACHHANG KH ON KQ.KH_ID = KH.ID
GO

2.6	Cài đặt Transaction
BEGIN TRANSACTION
BEGIN TRY
    -- 1️ NHÂN VIÊN
    INSERT INTO NHANVIEN (TENNV, NGAYSINH, GIOITINH, SDT, DIACHI, EMAIL, LUONG)
    VALUES (N'Nguyễn Văn A (Test)', '1990-01-01', N'Nam', '0909123458', N'Hà Nội', 'nva@test.com', 15000000);
    DECLARE @NV_ID INT = SCOPE_IDENTITY()

    -- 2️ KHÁCH HÀNG
    INSERT INTO KHACHHANG (TENKH, NGAYSINH, GIOITINH, SDT)
    VALUES (N'Trần Thị B (Test)', '1995-03-12', N'Nữ', '0987654322')
    DECLARE @KH_ID INT = SCOPE_IDENTITY()

    -- 3️ PHIM
    INSERT INTO PHIM (TENPHIM, THELOAI, THOILUONG, DIENVIENCHINH, KHOICHIEU, NGONNGU, XEPHANG, HINH)
    VALUES (N'Avengers: Endgame', N'Hành động', N'180 phút', N'Robert Downey Jr.', '2025-04-26', N'Tiếng Anh', 'T13', '/Images/Phim/avengers.jpg');
    DECLARE @PHIM_ID INT = SCOPE_IDENTITY()

    -- 4️ RẠP
    INSERT INTO RAP (TENRAP, DIACHI)
    VALUES (N'CGV Vincom Nguyễn Trãi', N'72 Nguyễn Trãi, Hà Nội')
    DECLARE @RAP_ID INT = SCOPE_IDENTITY()

    -- 5️ PHÒNG CHIẾU
    INSERT INTO PHONGCHIEU (TENPH, SOCHO, RAP_ID)
    VALUES (N'Phòng Test', 50, @RAP_ID)
    DECLARE @PHONG_ID INT = SCOPE_IDENTITY()

    -- 6️ SUẤT CHIẾU
    INSERT INTO SUATCHIEU (PHIM_ID, NGAYCHIEU, GIOCHIEU)
    VALUES (@PHIM_ID, '2025-10-15', '19:00')
    DECLARE @SUAT_ID INT = SCOPE_IDENTITY()

    -- 7️ GHẾ
    INSERT INTO GHE (PHONGCHIEU_ID, RAP_ID, VITRI, LOAIGHE)
    VALUES (@PHONG_ID, @RAP_ID, 'A1 (Test)', N'Thường')
    DECLARE @GHE_ID INT = SCOPE_IDENTITY()

    -- 8️ VÉ
    INSERT INTO VE (KH_ID, SUATCHIEU_ID, GHE_ID, NGAYMUA, GIAVE)
    VALUES (@KH_ID, @SUAT_ID, @GHE_ID, GETDATE(), 90000)
    DECLARE @VE_ID INT = SCOPE_IDENTITY()

    -- 9️ HÓA ĐƠN
    INSERT INTO HOADON (KH_ID, NV_ID, NGAYLAP, TONGTIEN)
    VALUES (@KH_ID, @NV_ID, GETDATE(), 0)
    DECLARE @HD_ID INT = SCOPE_IDENTITY()

    -- 10 CHI TIẾT HÓA ĐƠN (Sẽ kích hoạt Trigger TRG_CHITIETHOADON_TinhTongTien)
    INSERT INTO CHITIETHOADON (HOADON_ID, VE_ID)
    VALUES (@HD_ID, @VE_ID)

    COMMIT TRANSACTION;
    PRINT N'>>> TRANSACTION (Thêm dữ liệu) thành công.'
END TRY
BEGIN CATCH
    ROLLBACK TRANSACTION;
    PRINT N'>>> LỖI TRANSACTION (Thêm dữ liệu): ' + ERROR_MESSAGE()
END CATCH
GO

CHƯƠNG 3	QUẢN TRỊ HỆ THỐNG
3.1	Giới thiệu 


3.2	Giải pháp quản trị người dùng
Trong hệ quản trị cơ sở dữ liệu, quản trị người dùng là một nội dung quan trọng giúp đảm bảo tính bảo mật, toàn vẹn và kiểm soát truy cập dữ liệu. Mỗi người dùng cần được xác định danh tính rõ ràng, cấp quyền phù hợp với nhiệm vụ và được tổ chức theo nhóm hoặc vai trò cụ thể. Giải pháp quản trị người dùng thường bao gồm hai thành phần chính: cơ chế xác thực người dùng và tổ chức các nhóm người dùng.
3.2.1	Cơ chế xác thực
Cơ chế xác thực (Authentication Mechanism) là quá trình xác minh danh tính của người dùng trước khi họ được phép truy cập vào hệ thống cơ sở dữ liệu. Đây là bước đầu tiên và quan trọng nhất trong việc bảo đảm an toàn cho hệ thống, ngăn chặn các hành vi truy cập trái phép và kiểm soát quyền hạn của từng người dùng.
 	Mục tiêu của cơ chế của xác thực là đảm bảo chỉ người dùng hợp lệ mới có quyền truy cập hệ thống. Bảo vệ cơ sở dữ liệu khỏi các rủi ro an ninh như tấn công xâm nhập, đánh cắp dữ liệu hoặc phá hoại thông tin. Ngoài ra, ghi nhận và theo dõi lịch sử truy cập, phục vụ công tác kiểm tra và đánh giá bảo mật.
	Các phương thức xác thực chính bao gồm:
-	Xác thực bằng tài khoản hệ điều hành (Windows Authentication):  Cơ chế này sử dụng chính tài khoản người dùng trong môi trường hệ điều hành Windows để kiểm tra quyền truy cập. Khi người dùng đăng nhập vào máy tính thuộc miền mạng, hệ thống sẽ tự động xác nhận thông tin đăng nhập mà không yêu cầu nhập lại. Ngoài ra, đảm bảo tính bảo mật cao, vì toàn bộ thông tin đăng nhập được quản lý tập trung trong hệ thống mạng của tổ chức và giảm thiểu tình trạng trùng lặp tài khoản và tiết kiệm thời gian cho người dùng. Hạn chế của cơ chế này là chỉ áp dụng hiệu quả trong môi trường nội bộ có máy chủ quản lý miền (Domain Controller).
-	Xác thực nội bộ của hệ quản trị cơ sở dữ liệu (Database Authentication): Là cơ chế mà người dùng đăng nhập trực tiếp bằng tài khoản do hệ quản trị cơ sở dữ liệu cung cấp.
-	Xác thực kết hợp (Mixed Mode Authentication): Là sự kết hợp giữa hai phương thức trên: người dùng có thể đăng nhập bằng tài khoản hệ điều hành hoặc tài khoản nội bộ của hệ quản trị. Cách này mang lại tính linh hoạt, phù hợp với những tổ chức có nhiều đối tượng người dùng khác nhau. Ví dụ: nhân viên nội bộ và khách hàng bên ngoài.
-	Xác thực đa yếu tố (Multi-Factor Authentication - MFA): Là cơ chế xác thực sử dụng từ hai yếu tố trở lên. Phương thức này giúp tăng cường đáng kể mức độ an toàn, đặc biệt trong môi trường cơ sở dữ liệu có thông tin. Ví dụ: Thẻ bảo mật hoặc thiết bị di động, Sinh trắc học, Mật khẩu,…. 
-	Xác thực một lần (Single Sign-On - SSO): Cho phép người dùng chỉ cần đăng nhập một lần duy nhất để truy cập vào nhiều hệ thống hoặc ứng dụng có liên quan. Phù hợp với môi trường doanh nghiệp lớn có nhiều hệ thống tích hợp. Giúp giảm thiểu việc phải nhớ nhiều mật khẩu, đồng thời nâng cao trải nghiệm người dùng.

3.2.2	Các nhóm người dùng
Bên cạnh cơ chế xác thực, việc phân loại và tổ chức người dùng thành nhóm hoặc vai trò (Role) là bước tiếp theo trong quá trình quản trị người dùng. Cách làm này giúp người quản trị dễ dàng cấp quyền, kiểm soát hoạt động và duy trì tính nhất quán trong toàn bộ hệ thống cơ sở dữ liệu. Mục tiêu của việc này đơn giản hoá cấp và thu hồi quyền truy cập, quản lý người dùng theo chức năng, phòng ban hoặc nhiệm vụ công việc, bảo mật về an toàn và minh bạch trong quá trình thao tác dữ liệu và giúp quản trị viên mở rộng, điều chỉnh quyền một cách nhanh chóng khi có thay đổi về nhân sự hoặc cơ cấu tổ chức.
Các nhóm người dùng phổ biến như:
-	Nhóm quản trị (Administrators): Có quyền cao nhất trong hệ thống, chịu trách nhiệm cấu hình, giám sát và bảo trì cơ sở dữ liệu. Được phép tạo, xóa người dùng; cấp quyền truy cập và chỉnh sửa cấu trúc dữ liệu. Nhóm này đóng vai trò trung tâm trong việc đảm bảo tính ổn định và an toàn của hệ thống.
-	Nhóm chủ sở hữu cơ sở dữ liệu (Database Owners): Có quyền quản lý toàn bộ các đối tượng trong một cơ sở dữ liệu cụ thể như bảng, thủ tục, chỉ mục, và quan hệ giữa chúng. Chịu trách nhiệm kiểm soát dữ liệu trong phạm vi một dự án hoặc bộ phận nhất định.
-	Nhóm người dùng thông thường (Standard Users): Là những người trực tiếp thao tác với dữ liệu hằng ngày. Thường chỉ có quyền thực hiện một số chức năng cơ bản như xem, thêm, sửa hoặc xóa dữ liệu trong phạm vi được phép. Việc hạn chế quyền này giúp tránh sai sót hoặc thay đổi ngoài ý muốn đối với cấu trúc dữ liệu.
-	Nhóm khách (Guest Users): Có quyền truy cập tạm thời, thường dùng cho các đối tác hoặc người dùng cần tham khảo dữ liệu trong thời gian ngắn. Mọi quyền truy cập đều bị giới hạn nghiêm ngặt nhằm đảm bảo an toàn cho hệ thống.
-	Nhóm người dùng đặc thù (Custom Roles): Được thiết kế riêng theo nhu cầu của tổ chức, chẳng hạn như nhóm kế toán, nhóm nhân sự, nhóm kỹ thuật,… Giúp phản ánh rõ mô hình hoạt động thực tế của doanh nghiệp trong hệ thống cơ sở dữ liệu.

3.3	Tạo Login, User và Role
Login (Đăng nhập), User (Người dùng) và Role (Vai trò) là khái niệm chính trong quản trị cơ sở dữ liệu, với Login là bước đăng nhập để User thao tác với cơ sở dữ liệu dựa trên role đã có.


3.3.1	Tạo Login


3.3.2	Tạo User


3.3.3	Tạo phân quyền (Role)


3.3.4	Thu hồi quyền truy cập


3.3.5	Cấp quyền thực thi (EXECUTE)



3.4	Lập lịch sao lưu định kỳ
3.4.1	Mô tả lịch trình sao lưu
Kế hoạch sao lưu cơ sở dữ liệu được diễn ra 6 ngày/ tuần, đảm bảo an toàn tránh gặp sự cố. Mô hình phục hồi được sử dụng trong cơ sở dữ liệu quản lý rạp chiếu phim là đầy đủ (Full). Có ba loại sao lưu được thực hiện:
-	Sao lưu đầy đủ (Full Backup): Sao lưu toàn bộ cơ sở dữ liệu, thực hiện đơn giản giảm thao tác thực hiện. Tuy nhiên, thời gian sao lưu sẽ tốn nhiều thời gian hơn trong các phương pháp khác do có kích thước lớn.
-	Sao lưu một phần (Differential Backup): Được sử dụng để sao lưu một phần từ bản Full Backup đã thực hiện sao lưu trước đó, do đó thời gian thực hiện sẽ nhanh hơn và dung lượng file sẽ giảm đi đáng kể. Tuy nhiên, việc thực hiện nhiều lần thì kích thước của file sẽ tăng lên dần, gây tốn bộ nhớ hơn.
-	Sao lưu tập tin log (Transaction log backup): Tập tin transaction log có nhiệm vụ ghi lại tất cả những thay đổi trong cơ sở dữ liệu để giảm khả năng mất dữ liệu xuống mức thấp nhất, cần sao lưu lại định kỳ để khôi phục lại thao tác nếu cơ sở dữ liệu gặp sự cố.
Lịch trình sao lưu của cơ sở dữ liệu quản lý rạp chiếu phim được minh họa sơ đồ ở hình 3.1:

 
Hình 3.1 Sơ đồ lịch trình sao lưu cơ sở dữ liệu định kỳ
Ở sơ đồ hình 3.1 lịch trình được mô tả lịch trình chi tiết như sau:
-	Thứ hai: Cơ sở dữ liệu được sao lưu được thực hiện sao lưu đầy đủ (Full Backup) vào lúc 22 giờ 00 phút.
-	Thứ ba: Sau khi có bản sao lưu Full Backup gần nhất vào thứ hai hôm qua, thực hiện sao lưu một phần vào lúc 11 giờ trưa. Vào buổi chiều tiến hành sao lưu tập tin log vào lúc 22 giờ 00 phút.
-	Thứ tư: Thực hiện sao lưu Differential Backup vào lúc 11 giờ trưa, buổi chiều sao lưu log backup vào lúc 22 giờ 00 phút.
-	Thứ năm: Thực hiện tương tự như lịch trình của thứ tư.
-	Thứ sáu: Thực hiện sao lưu full backup vào lúc 22 giờ 00 phút.
-	Thứ bảy: Sau khi có bản sao lưu full backup vào thứ sáu, sao lưu được thực hiện tương tự ở lịch trình thứ tư và thứ năm.

3.4.2	Lệnh sao lưu cơ sở dữ liệu
-	Trước khi sao lưu cơ sở dữ liệu cần phải đặt mô hình phục hồi là FULL:
-- Đặt mô hình phục hồi là FULL
ALTER DATABASE DB_QLRAPCHIEUPHIM
SET RECOVERY FULL

-	Lệnh sao lưu đầy đủ:
--Sao lưu định kỳ Full Backup
DECLARE @FileName NVARCHAR(200)
SET @FileName = 'D:\Document\QTCSDL\DB_QLRAPCHIEUPHIM_Full' -- Đường dẫn có thể thay đổi được
    + CONVERT(VARCHAR(8), GETDATE(), 112) + '.bak'
BACKUP DATABASE DB_QLRAPCHIEUPHIM
TO DISK = @FileName
WITH INIT, -- Ghi đề bản sao lưu cũ trước đó
     NAME = 'Full Backup DB_QLRAPCHIEUPHIM',
     DESCRIPTION = 'Sao lưu toàn bộ dữ liệu định kỳ (Full Backup)',
     STATS = 10

-	Lệnh sao lưu một phần:
--Sao lưu định kỳ Differential Backup
DECLARE @FileName NVARCHAR(200)
SET @FileName = 'D:\Document\QTCSDL\DB_QLRAPCHIEUPHIM_Diff' 
    + CONVERT(VARCHAR(8), GETDATE(), 112) + '.bak'
BACKUP DATABASE DB_QLRAPCHIEUPHIM
TO DISK = @FileName
WITH DIFFERENTIAL,
     NAME = 'Differential Backup DB_QLRAPCHIEUPHIM',
     DESCRIPTION = 'Sao lưu phần thay đổi từ bản full gần nhất',
     STATS = 10

-	Lệnh sao lưu tập tin log:
--Sao lưu định kỳ Transaction Log Backup
DECLARE @FileName NVARCHAR(200)
SET @FileName = 'D:\Document\QTCSDL\DB_QLRAPCHIEUPHIM_Log' 
    + REPLACE(CONVERT(VARCHAR(19), GETDATE(), 120), ':', '') + '.trn'
BACKUP LOG DB_QLRAPCHIEUPHIM
TO DISK = @FileName
WITH INIT,
     NAME = 'Transaction Log Backup DB_QLRAPCHIEUPHIM',
     DESCRIPTION = 'Sao lưu log giao dịch định kỳ để khôi phục đến thời điểm cụ thể',
     STATS = 10

3.5	Thiết lập sao lưu tự động
3.5.1	Tạo công việc sao lưu tự động Full Backup
-	Sao lưu toàn bộ cơ sở dữ liệu vào cuối tuần hoặc theo chu kỳ nhất định (ví dụ: thứ Hai và thứ Sáu).
-	Các bước thực hiện:
-	Mở SQL Server Management Studio (SSMS) → Mở SQL Server Agent → chuột phải Jobs → chọn New Job...
-	Đặt tên cho công việc, ví dụ: Backup_Full_RapChieuPhim.
 

Trong tab Steps, nhấn New... → nhập:
•	Step name: FullBackup
•	Type: Transact-SQL script (T-SQL)
•	Database: DB_QLRAPCHIEUPHIM
•	Command:
DECLARE @FileName NVARCHAR(200)
SET @FileName = 'D:\Document\QTCSDL\DB_QLRAPCHIEUPHIM_Full' 
    + CONVERT(VARCHAR(8), GETDATE(), 112) + '.bak'
BACKUP DATABASE DB_QLRAPCHIEUPHIM
TO DISK = @FileName
WITH INIT, 
     NAME = 'Full Backup DB_QLRAPCHIEUPHIM',
     DESCRIPTION = 'Sao lưu toàn bộ dữ liệu định kỳ (Full Backup)',
     STATS = 10
 

Trong tab Schedules, nhấn New... → đặt lịch:
•	Name: Full_Backup_Schedule
•	Frequency: Weekly → chọn Thứ Hai, Thứ Sáu
•	Time: 22:00
 
Nhấn OK dể lưu lại
 
Sau khi lưu lại xong
 
Bắt đầu sao lưu: Tên Jobs  Start Job at Step …
 
Sau lưu sao lưu tự động thành công sẽ hiện trong tập tin đã lưu ở ổ đĩa đã dẫn đến nơi ở ổ đĩa D.
 
 
Tự động sao lưu đúng thời gian đặt lên lịch như Hình 3.1:
 

3.5.2	Tạo công việc sao lưu tự động Differential
Tương tự như Hình 3.1 được thực hiện theo lịch trình sao lưu tự động Diferential:

 

 

 
Lịch trình sao lưu tự động được thực hiện vào thứ ba, thứ tư, thứ năm và thứ bảy vào lúc 11 giờ sáng.
 

 

  

 


3.5.3	Tạo công việc sao lưu tự động Transaction log
Thực hiện sao lưu Transation log theo lịch trình như Hình 3.1:
 

 
Lịch trình sao lưu tự động được lên lịch thứ ba, thứ tư, thứ năm và thứ bảy vào lúc 22 giờ.
 

 

 

3.6	Phục hồi cơ sở dữ liệu
Trong quá trình vận hành hệ thống quản lý rạp chiếu phim, việc sao lưu (backup) và phục hồi (restore) cơ sở dữ liệu là hết sức quan trọng nhằm đảm bảo dữ liệu không bị mất do lỗi hệ thống, lỗi phần cứng hoặc thao tác nhầm lẫn từ người dùng.
Mục đích phục hồi lại cơ sở dữ liệu nhằm khôi phục lại dữ liệu khi gặp sự cố xảy ra, cho phép quay lại trạng thái dữ liệu ở một thời điểm cụ thể, tạo ra môi trường an toàn cho việc triển nâng cấp, triển khai một ứng dụng hoặc website.
Lệnh phục hồi cơ sở dữ liệu được thực hiện theo thứ tự sau: Full Backup, Differential Backup và Transaction Log Backup.
-	Lệnh phục hồi Full Backup:
RESTORE DATABASE DB_QLRAPCHIEUPHIM
FROM DISK = 'D:\Document\QTCSDL\DB_QLRAPCHIEUPHIM_Full_20251123.bak'
WITH NORECOVERY
-	Lệnh phục hồi Differential Backup:
RESTORE DATABASE DB_QLRAPCHIEUPHIM
FROM DISK = 'D:\Document\QTCSDL\DB_QLRAPCHIEUPHIM_Diff_20251123.bak'
WITH NORECOVERY
-	Lệnh phục hồi Transaction Log Backup:
RESTORE LOG DB_QLRAPCHIEUPHIM
FROM DISK = 'D:\Document\QTCSDL\DB_QLRAPCHIEUPHIM_Log_20251123.trn'
WITH RECOVERY
Kết luận: Việc thực hiện đúng quy trình giúp đảm bảo cơ sở dữ liệu được khôi phục đầy đủ, an toàn và không xảy ra lỗi tính nhất quán.

3.7	Kết luận
Trong chương này, nhóm đã tiến hành các bước quan trọng trong quá trình xây dựng và quản trị cơ sở dữ liệu cho hệ thống quản lý rạp chiếu phim. Từ việc thiết kế mô hình dữ liệu, định nghĩa bảng và ràng buộc, cho đến cấu hình Login – User – Role, các thao tác được thực hiện đã đảm bảo tính toàn vẹn, bảo mật và ổn định của cơ sở dữ liệu.
Bên cạnh đó, việc thiết lập cơ chế phân quyền chi tiết giúp kiểm soát tốt quyền truy cập của từng nhóm người dùng, tránh các thao tác không mong muốn và đảm bảo dữ liệu được bảo vệ an toàn. Đây là yếu tố then chốt đối với các hệ thống thực tế, nơi an ninh dữ liệu có vai trò quan trọng.
Ngoài ra, nhóm cũng đã triển khai quy trình sao lưu và phục hồi cơ sở dữ liệu theo các bước Full Backup, Differential Backup và Transaction Log Backup. Quy trình này giúp hệ thống có khả năng khôi phục dữ liệu ở bất kỳ thời điểm nào và đảm bảo hoạt động liên tục ngay cả khi xảy ra sự cố.
Nhờ các bước thực hiện trong chương này, cơ sở dữ liệu của hệ thống đã được cấu hình một cách đầy đủ, có khả năng vận hành lâu dài, phục vụ tốt cho các chức năng nghiệp vụ ở những chương tiếp theo như đặt vé, quản lý phòng chiếu, quản lý khách hàng và thanh toán.


CHƯƠNG 4	XÂY DỰNG ỨNG DỤNG
4.1	Mục tiêu


4.2	Cài đặt ứng dụng
-	Ngôn ngữ lập trình: C# (ASP.NET cùng với mô hình MVC 5).
-	Nền tảng đám mây: Azure, Azure hosting web.
-	Tên miền: https://doannhom4qtcsdl.azurewebsites.net/.
-	Máy chủ: SQL Server 2022, Azure SQL Database.
-	Phần mềm: Visual Studio 2022, SQL Server Management 20 / 21.

4.3	Giao diện ứng dụng
-	Giao diện đăng nhập hệ thống:
 
Hình 4.1 Giao diện đăng nhập người dùng
-	Giao diện đăng ký:
 
Hình 4.2 Giao diện đăng ký tài khoản
-	Giao diện Dashboard:
    
Hình 4.3 Giao diện Dashboard dành cho quản trị viên, nhân viên bán vé
 
Hình 4.4 Giao diện Dashboard dành cho khách

-	Có các ràng buộc đã thiết lập:
Dữ liệu được cho là ngày sinh không thoả 18 tuổi:
 

 



-	Thực hiện chức năng CRUD:
 

 



4.4	Kết quả


4.5	Nhận xét


4.6	Tổng kết



TÀI LIỆU THAM KHẢO
[1]	Studocu: https://www.studocu.vn/vn/document/truong-dai-hoc-su-pham-thanh-pho-ho-chi-minh/ly-thuyet-do-thi-va-ung-dung/cosodulieu-quan-ly-rap-chieu-phim/21365076 < Available: 09-10-2025>
[2]	Scribd: https://www.scribd.com/document/615235193/H%E1%BB%87-th%E1%BB%91ng-qu%E1%BA%A3n-l%C3%BD-r%E1%BA%A1p-chi%E1%BA%BFu-phim-phan-tich-thi%E1%BA%BFt-k%E1%BA%BF-h%E1%BB%87-th%E1%BB%91ng-thong-tin-CTU < Available: 12-10-2025>
[3]	Giáo trình Hệ Quản trị Cơ sở dữ liệu, Trường Đại học Công Thương TP.HCM, 2025.
[4]	Bài giảng Lập trình Web, Trường Đại học Công Thương TP.HCM, 2025.




