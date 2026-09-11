#### Tác giả chính: Hoàng Ngọc Hùng

## Giới thiệu
*Đây là một dư án về toán học được thực hiện bởi Hoàng Ngọc Hùng*
 ## ỨNG DỤNG CỦA HỆ PHƯƠNG TRÌNH ĐẠI SỐ TRONG GIẢI CÁC BÀI TOÁN THỰC TẾ
Trong toán học, hệ phương trình đại số là một công cụ quan trọng giúp mô tả
và làm rõ mối quan hệ giữa các đại lượng trong nhiều bài toán khác nhau. Việc
xây dựng và giải hệ phương trình không chỉ là một kĩ năng cơ bản của toán học
mà còn là phương tiện hữu hiệu để tiếp cận và giải quyết nhiều vấn đề trong
thực tiễn đời sống, khoa học và kĩ thuật.

Từ những bài toán đơn giản đến các mô hình phức tạp hơn, hệ phương trình
luôn giữ vai trò quan trọng trong việc biểu diễn các điều kiện ràng buộc giữa
các đại lượng. Thông qua việc chuyển đổi những tình huống thực tế thành các
mô hình toán học dưới dạng hệ phương trình, ta có thể phân tích, dự đoán và
tìm ra lời giải phù hợp cho bài toán đặt ra. Điều đó cho thấy tính ứng dụng rộng
rãi cũng như hiệu quả của tư duy toán học trong thực tế.

Nội dung đề tài này tập trung trình bày một số ứng dụng tiêu biểu của hệ
phương trình đại số thông qua các bài toán thực tiễn và mô hình toán học quen
thuộc. Qua đó, làm nổi bật vai trò của hệ phương trình trong việc ứng dụng toán
học vào đời sống, đồng thời thấy được giá trị và ý nghĩa thực tiễn mà chúng
mang lại.

## Lĩnh vực kinh tế
# Bài toán: Mô hình kinh tế đầu vào - đầu ra Leontief
# Mô tả bài toán:
  Mô hình kinh tế đầu vào - đầu ra Leontief phân tích mối quan hệ phụ thuộc lẫn nhau giữa các ngành trong một nền kinh tế. Nó sử dụng một ma trận đầu vào - đầu ra để thể hiện lượng đầu vào từ một ngành cần thiết cho việc sản xuất của các ngành khác. Mục tiêu là xác định mức sản lượng mà mỗi ngành phải tạo ra để đáp ứng cả nhu cầu nội bộ giữa các ngành và nhu cầu cuối cùng của xã hội, giúp lập kế hoạch và phân tích tác động kinh tế.

# Bài toán:
 Xét một hệ thống kinh tế đơn giản bao gồm ba ngành:
lúa gạo, dệt may và thép. Đầu ra của một đơn vị lúa gạo cần 0,4 đơn vị của
chính nó, 0,2 đơn vị dệt may và 0,1 đơn vị thép. Sản xuất một đơn vị dệt
may cần 0,1 đơn vị lúa gạo, 0,5 đơn vị của chính nó và 0,2 đơn vị thép.
Sản xuất một đơn vị thép cần 0,2 đơn vị lúa gạo, 0,1 đơn vị dệt may và
0,4 đơn vị của chính nó.

Giả sử hệ thống kinh tế có một nhu cầu cuối cùng đối với sản phẩm của
các ngành như sau:

    - Nhu cầu cuối cùng về lúa gạo: 120 đơn vị.
    - Nhu cầu cuối cùng về dệt may: 80 đơn vị.
    - Nhu cầu cuối cùng về thép: 100 đơn vị.

Yêu cầu: Tìm ma trận đầu vào - đầu ra cho hệ thống kinh tế này và tính
tổng sản lượng mà mỗi ngành phải sản xuất để đáp ứng đầy đủ cả nhu cầu
trung gian giữa các ngành và nhu cầu cuối cùng của hệ thống kinh tế.

# Lời giải

Gọi (x,y,z) lần lượt là tổng sản lượng mà các ngành lúa gạo, dệt may,
thép phải sản xuất. Và biểu diễn dưới dạng ma trận cột là

$$
X=
\begin{bmatrix}
x\\
y\\
z
\end{bmatrix}
$$

Ta thiết lập ma trận đầu vào - đầu ra của hệ thống kinh tế này là ma trận
(3x3) có các cột xếp theo thứ tự Lúa gạo - Dệt may - Thép thể hiện lượng
đầu vào của các ngành.

Ngành lúa gạo có 3 đầu vào là 0,4 từ lúa gạo, 0,2 từ dệt may và
0,1 từ thép. Nên cột của ngành Lúa gạo là

$$
\begin{bmatrix}
0,4\\
0,2\\
0,1
\end{bmatrix}
$$

Tương tự cho các ngành còn lại ta được ma trận đầu vào - đầu ra của hệ
thống kinh tế này và đặt tên là A

$$
A=
\begin{bmatrix}
0,4 & 0,1 & 0,2\\
0,2 & 0,5 & 0,1\\
0,1 & 0,2 & 0,4
\end{bmatrix}
$$

Nhu cầu cuối cùng của các ngành ta lập được thành ma trận cột

$$
B=
\begin{bmatrix}
120\\
80\\
100
\end{bmatrix}
$$

Tổng lượng sản phẩm của cả ba ngành phải sản xuất để đáp ứng đầy đủ cả
nhu cầu trung gian giữa các ngành và nhu cầu cuối cùng của hệ thống kinh tế
được biểu diễn dưới dạng

$$
X=AX+B \Leftrightarrow (A-I_3)X=-B
$$

$$
\Leftrightarrow
\begin{bmatrix}
-0,6 & 0,1 & 0,2\\
0,2 & -0,5 & 0,1\\
0,1 & 0,2 & -0,6
\end{bmatrix}
X=
\begin{bmatrix}
-120\\
-80\\
-100
\end{bmatrix}
$$

$$
\Leftrightarrow
X=
\begin{bmatrix}
-0,6 & 0,1 & 0,2\\
0,2 & -0,5 & 0,1\\
0,1 & 0,2 & -0,6
\end{bmatrix}^{-1}
\cdot
\begin{bmatrix}
-120\\
-80\\
-100
\end{bmatrix}
$$

(do $\det(A-I_3)\neq0$)

$$
\Leftrightarrow
X=
\begin{bmatrix}
\dfrac{52700}{137}\\
\dfrac{53400}{137}\\
\dfrac{49200}{137}
\end{bmatrix}
\approx
\begin{bmatrix}
384,67\\
389,78\\
359,12
\end{bmatrix}
$$

Vậy tổng sản lượng cần thiết mỗi ngành phải sản xuất là:

    - Lúa gạo khoảng 384,67 đơn vị.
    - Dệt may khoảng 389,78 đơn vị.
    - Thép khoảng 359,12 đơn vị.

## Mô hình cân bằng cục bộ cho các thị trường
# Mô tả bài toán:
Bài toán này nghiên cứu trạng thái cân bằng về giá và sản lượng của hai thị
trường riêng biệt nhưng có sự tác động qua lại lẫn nhau. Do mối liên hệ giữa
các yếu tố cung và cầu của hai thị trường, các đại lượng không còn độc lập mà
phụ thuộc lẫn nhau thông qua các điều kiện ràng buộc, từ đó hình thành một hệ
phương trình đại số phi tuyến.

Việc xây dựng và giải hệ phương trình này cho phép xác định mức giá và sản
lượng cân bằng của từng thị trường. Đây là trạng thái mà tại đó lượng cung và
lượng cầu ở cả hai thị trường đều bằng nhau, đồng thời phản ánh sự ổn định của
toàn bộ hệ thống kinh tế đang xét.

## Bài toán

Trong một nền kinh tế nhỏ có hai loại hàng hóa liên quan mật thiết với nhau là: **Sữa tươi (A)** và **bánh mì (B)**.

Với các thị trường (bao gồm giá (đơn vị: nghìn VNĐ), hàm cung, hàm cầu) và giả sử việc sản xuất sữa và bánh mì có mối quan hệ với nhau như sau:

### Thị trường Sữa tươi (A)

- Giá sữa tươi $(P_A)$: đơn vị nghìn đồng/lít.

- Hàm cầu sữa tươi:

$$
Q_A^D=200-P_A
$$

- Hàm cung sữa tươi:

$$
Q_A^S=20+2P_A-5P_B
$$

### Thị trường Bánh mì (B)

- Giá bánh mì $(P_B)$: đơn vị nghìn đồng/ổ.

- Hàm cầu bánh mì:

$$
Q_B^D=120-2P_B+0,5P_A
$$

- Hàm cung bánh mì:

$$
Q_B^S=30+P_B
$$

**Yêu cầu:** Tìm giá của sữa tươi và bánh mì để cả hai thị trường đạt trạng thái cân bằng (lượng cung bằng lượng cầu).

## Lời giải

Do giả thiết đã gọi tất cả các giá trị cần tìm nên ta không cần gọi lại lần nữa. Ta chỉ quan tâm đến các điều kiện là:

$$
P_A>0,\quad P_B>0
$$

Yêu cầu bài toán là cần xác định giá sữa tươi $(P_A)$ và giá bánh mì $(P_B)$ sao cho thị trường sữa tươi và bánh mì đạt trạng thái cân bằng, khi đó lượng cung và lượng cầu của chúng phải bằng nhau tức là:

$$
\begin{cases}
Q_A^S=Q_A^D\\
Q_B^S=Q_B^D
\end{cases}
$$

$$
\Leftrightarrow
\begin{cases}
20+2P_A-5P_B=200-P_A\\
30+P_B=120-2P_B+0,5P_A
\end{cases}
$$

$$
\Leftrightarrow
\begin{cases}
3P_A-5P_B=180\\
0,5P_A-3P_B=-90
\end{cases}
$$

Nhân phương trình thứ hai với $2$, ta được:

$$
\begin{cases}
3P_A-5P_B=180\\
P_A-6P_B=-180
\end{cases}
$$

Từ phương trình thứ hai:

$$
P_A=6P_B-180
$$

Thế vào phương trình thứ nhất:

$$
3(6P_B-180)-5P_B=180
$$

$$
18P_B-540-5P_B=180
$$

$$
13P_B=720
$$

$$
P_B=\frac{720}{13}\approx55,38
$$

Suy ra:

$$
P_A=6\cdot\frac{720}{13}-180
$$

$$
P_A=\frac{1980}{13}\approx152,31
$$

Vậy hai thị trường đạt cân bằng khi:

- **Giá sữa tươi:** khoảng $152,31$ nghìn đồng/lít.
- **Giá bánh mì:** khoảng $55,38$ nghìn đồng/ổ.
