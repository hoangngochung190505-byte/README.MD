#### Tác giả chính: Hoàng Ngọc Hùng

## Giới thiệu
*Đây là một dư án về toán học được thực hiện bởi Hoàng Ngọc Hùng*
 ## ỨNG DỤNG CỦA HỆ PHƯƠNG TRÌNH ĐẠI SỐ
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

Nội dung chương này tập trung trình bày một số ứng dụng tiêu biểu của hệ
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
