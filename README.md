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


# Bài toán: Phân bổ nguồn lực trong sản xuất

## Mô tả bài toán

Bài toán phân bổ nguồn lực trong sản xuất là bài toán xác định số lượng sản phẩm cần sản xuất sao cho việc sử dụng các nguồn lực của doanh nghiệp đạt hiệu quả cao nhất. Trong thực tế, các nguồn lực như nguyên vật liệu, nhân công, thời gian lao động hay công suất máy móc đều có giới hạn nhất định, vì vậy doanh nghiệp cần xây dựng kế hoạch sản xuất phù hợp để tránh lãng phí và đảm bảo hiệu quả hoạt động.

Mỗi loại sản phẩm thường tiêu tốn một lượng tài nguyên khác nhau cho từng công đoạn sản xuất. Từ đó, các mối quan hệ giữa số lượng sản phẩm và lượng nguồn lực sử dụng có thể được mô hình hóa bằng các hệ phương trình hoặc bất phương trình đại số. Việc giải các hệ này giúp xác định phương án sản xuất phù hợp, đồng thời hỗ trợ doanh nghiệp trong việc tối ưu hóa lợi nhuận hoặc khai thác tối đa công suất hiện có.

## Bài toán
Trong một xưởng sản xuất có hai loại sản phẩm là **bàn học** và **ghế học sinh**.
Quá trình sản xuất cần trải qua hai công đoạn chính là cắt gỗ và sơn hoàn thiện.

- Để sản xuất một bàn học, cần: $3$ giờ ở công đoạn cắt gỗ và $2$ giờ ở công đoạn sơn hoàn thiện.

- Để sản xuất một ghế học sinh, cần: $2$ giờ ở công đoạn cắt gỗ và $3$ giờ ở công đoạn sơn hoàn thiện.

Do yêu cầu của kế hoạch sản xuất, mỗi ngày xưởng phải sử dụng hết đúng $180$ giờ công cho công đoạn cắt gỗ và đúng $210$ giờ công cho công đoạn sơn hoàn thiện.

**Yêu cầu:** Xác định số lượng sản phẩm mỗi loại trong một ngày mà xưởng phải sản xuất để sử dụng hết toàn bộ nguồn lực theo kế hoạch.

## Lời giải

- Gọi $x$ là số lượng bàn học cần sản xuất.
- Gọi $y$ là số lượng ghế học sinh cần sản xuất.

Điều kiện: $x,y$ là các số nguyên không âm, $x,y\in\mathbb{N}$.

Dựa trên yêu cầu phải sử dụng hết các nguồn lực, ta có hệ phương trình sau:

$$
\begin{cases}
3x+2y=180\\
2x+3y=210
\end{cases}
$$

$$
\Leftrightarrow
\begin{cases}
9x+6y=540\\
4x+6y=420
\end{cases}
$$

$$
\Leftrightarrow 5x=120
$$

$$
\Leftrightarrow x=24
$$

Thế $x=24$ vào phương trình:

$$
3x+2y=180
$$

ta được:

$$
3\cdot24+2y=180
$$

$$
72+2y=180
$$

$$
2y=108
$$

$$
y=54
$$

Vậy:

$$
\begin{cases}
x=24\\
y=54
\end{cases}
$$

Vậy để sử dụng hết chính xác các nguồn lực theo kế hoạch, xưởng cần sản xuất **24 bàn học và 54 ghế học sinh mỗi ngày**.

# Lĩnh vực khoa học tự nhiên

## Bài toán: Phân tích mạch điện với phần tử phi tuyến

### Mô tả bài toán

Bài toán này nghiên cứu một mạch điện cơ bản gồm nguồn điện áp, điện trở thuần và một phần tử điện có đặc tính phi tuyến. Khác với điện trở thông thường, điện áp trên phần tử đặc biệt này không tỉ lệ bậc nhất với cường độ dòng điện mà được biểu diễn thông qua một hàm bậc hai của dòng điện.

Do mối liên hệ phi tuyến giữa điện áp và cường độ dòng điện, việc phân tích mạch điện dẫn đến một hệ phương trình đại số phi tuyến tính. Thông qua việc xây dựng và giải hệ phương trình này, ta có thể xác định được cường độ dòng điện chạy trong mạch cũng như điện áp rơi trên phần tử phi tuyến.

Bài toán cho thấy vai trò của hệ phương trình đại số trong việc mô hình hóa các hiện tượng vật lí, đặc biệt là trong phân tích và thiết kế các hệ thống điện có chứa những phần tử với đặc tính hoạt động phức tạp.

## Bài toán

Một kỹ sư điện đang phân tích một mạch điện đơn giản mắc nối tiếp, gồm một nguồn điện áp một chiều (DC), một điện trở tuyến tính tiêu chuẩn và một phần tử điện trở phi tuyến đặc biệt.

- **Nguồn điện áp $(V_{\text{nguồn}})$:** Cung cấp $18$ Volt.

- **Điện trở tuyến tính $(R_1)$:** Có giá trị $3$ Ohm.

- **Phần tử phi tuyến:** Điện áp rơi trên nó $(V_{NL})$ và dòng điện chạy qua nó $(I)$ tuân theo phương trình:

$$
V_{NL}=I^2
$$

**Yêu cầu:** Tính dòng điện $(I)$ chạy trong mạch (theo chiều dương) và điện áp rơi $(V_{NL})$ trên phần tử phi tuyến.

## Lời giải
## Lời giải

Do dòng điện tính theo chiều dương nên:

$$
I>0
$$

Theo Định luật Kirchhoff về Điện áp (KVL - Kirchhoff’s Voltage Law):

Trong một vòng kín của mạch, tổng đại số các điện áp rơi trên các phần tử phải bằng điện áp của nguồn.

$$
V_{\text{nguồn}}-V_{R_1}-V_{NL}=0
$$

Điện áp rơi trên điện trở tuyến tính $(V_{R_1})$ tuân theo Định luật Ohm:

$$
V_{R_1}=I\cdot R_1
$$

Thay các giá trị vào ta được:

$$
18-I\cdot3-V_{NL}=0
$$

$$
\Leftrightarrow 3I+V_{NL}=18
$$

Kết hợp với phương trình của phần tử phi tuyến ở đề bài ta được hệ phương trình sau:

$$
\begin{cases}
3I+V_{NL}=18\\
V_{NL}=I^2
\end{cases}
$$

$$
\Leftrightarrow
\begin{cases}
I^2+3I-18=0\\
V_{NL}=I^2
\end{cases}
$$

Giải phương trình bậc hai:

$$
I^2+3I-18=0
$$

$$
\Delta=3^2-4\cdot1\cdot(-18)=81
$$

$$
\sqrt{\Delta}=9
$$

Do đó:

$$
I=\frac{-3\pm9}{2}
$$

$$
\Leftrightarrow
\begin{cases}
I=3\\
I=-6\quad(\text{loại})
\end{cases}
$$

Suy ra:

$$
I=3
$$

Thay vào:

$$
V_{NL}=I^2
$$

ta được:

$$
V_{NL}=3^2=9
$$

Vậy:

- Dòng điện chạy trong mạch là $3$ A.
- Điện áp rơi trên phần tử phi tuyến là $9$ V.

---

# Bài toán: Va chạm đàn hồi của hai vật thể

## Mô tả bài toán

Bài toán này mô tả một va chạm đàn hồi hoàn toàn giữa hai vật thể chuyển động trên cùng một đường thẳng. Với các thông số về khối lượng và vận tốc ban đầu của mỗi vật thể đã được cho trước, mục tiêu là xác định vận tốc cuối cùng của chúng sau khi va chạm. Việc này đòi hỏi phải áp dụng đồng thời hai nguyên lí vật lí cơ bản: định luật bảo toàn động lượng và định luật bảo toàn động năng, từ đó thiết lập một hệ phương trình đại số phi tuyến tính để giải tìm các vận tốc chưa biết.

## Bài toán

Hai vật thể đang chuyển động trên một đường thẳng và va chạm đàn hồi hoàn toàn.

- Vật thể 1 có khối lượng $m_1=2\text{ kg}$ và vận tốc ban đầu $v_{1_0}=5\text{ m/s}$.
- Vật thể 2 có khối lượng $m_2=3\text{ kg}$ và đang đứng yên $(v_{2_0}=0\text{ m/s})$.

**Yêu cầu:** Tính vận tốc cuối cùng của mỗi vật thể $(v_1$ và $v_2)$ sau va chạm.

**Lời giải.**

Trong va chạm đàn hồi, động lượng toàn phần và động năng toàn phần của hệ vật được bảo toàn:

- **Bảo toàn động lượng:**

$$
m_1v_{1_0}+m_2v_{2_0}=m_1v_1+m_2v_2
$$

Thay số và rút gọn ta được:

$$
10=2v_1+3v_2
$$

 **Bảo toàn động năng:**

$$
\frac{1}{2}m_1v_{1_0}^2+
\frac{1}{2}m_2v_{2_0}^2
=\frac{1}{2}m_1v_1^2+
\frac{1}{2}m_2v_2^2
$$

Thay số và rút gọn ta được:

$$
25=v_1^2+1,5v_2^2
$$

Khi đó ta có hệ phương trình:

$$
\begin{cases}
v_1^2+1,5v_2^2=25\\
2v_1+3v_2=10
\end{cases}
$$

$$
\Leftrightarrow
\begin{cases}
(10-3v_2)^2+6v_2^2=100\\
10-3v_2=2v_1
\end{cases}
$$

$$
\Leftrightarrow
\begin{cases}
v_2=4\\
v_2=0
\end{cases}
$$

và:

$$
2v_1=10-3v_2
$$

Nếu $v_2=0\Rightarrow v_1=5$ là trạng thái ban đầu của hệ vật nên ta không xét.

Nếu $v_2=4\Rightarrow v_1=-1$.

Vậy sau khi va chạm, vận tốc của hai vật thể lần lượt là:

$$
v_1=-1\text{ m/s},\qquad v_2=4\text{ m/s}
$$

---

# Bài toán: Cân bằng phương trình phản ứng Hóa học

## Mô tả bài toán

Khi cân bằng một phương trình phản ứng hóa học phức tạp, mục tiêu là tìm được các hệ số nguyên dương nhỏ nhất sao cho số nguyên tử của mỗi nguyên tố ở hai vế của phương trình phản ứng là bằng nhau. Đây chính là nguyên tắc bảo toàn nguyên tố trong hóa học.

Quá trình cân bằng phản ứng có thể được mô hình hóa bằng một hệ phương trình đại số tuyến tính. Trong đó, mỗi ẩn số biểu diễn hệ số của một chất trong phương trình hóa học, còn mỗi phương trình thể hiện điều kiện bảo toàn số nguyên tử của một nguyên tố cụ thể.

Thông qua việc thiết lập và giải hệ phương trình này, ta xác định được các hệ số thích hợp để hoàn chỉnh phương trình phản ứng. Bài toán cho thấy mối liên hệ chặt chẽ giữa toán học và hóa học, đồng thời thể hiện vai trò của hệ phương trình tuyến tính trong việc giải quyết các vấn đề thực tiễn của khoa học tự nhiên.

## Bài toán

Phản ứng oxi hóa -- khử giữa Đồng $(Cu)$, Axit nitric $(HNO_3)$ tạo ra Đồng(II) nitrat $(Cu(NO_3)_2)$, khí Nitơ đioxit $(NO_2)$ và Nước $(H_2O)$.

$$
Cu+HNO_3\rightarrow Cu(NO_3)_2+NO_2+H_2O
$$

**Yêu cầu:** Tìm các hệ số $a,b,c,d,e$ nhỏ nhất để cân bằng phương trình phản ứng:

$$
aCu+bHNO_3\rightarrow cCu(NO_3)_2+dNO_2+eH_2O
$$

## Lời giải

Áp dụng định luật bảo toàn nguyên tử ta có:

- **Nguyên tử Đồng $(Cu)$:**

$$
a=c
$$

- **Nguyên tử Hydro $(H)$:**

$$
b=2e
$$

- **Nguyên tử Nitơ $(N)$:**

$$
b=2c+d
$$

- **Nguyên tử Oxi $(O)$:**

$$
3b=6c+2d+e
$$

Khi đó ta có hệ phương trình:

$$
\begin{cases}
a-c=0\\
b-2e=0\\
b-2c-d=0\\
3b-6c-2d-e=0
\end{cases}
$$

Đây là hệ $4$ phương trình tuyến tính nhưng có $5$ ẩn nên hệ có vô số nghiệm phụ thuộc vào một ẩn tự do.

Giả sử $c$ là ẩn tự do và chọn:

$$
c=1
$$

Khi đó từ hệ ta suy ra:

$$
a=1
$$

$$
b=2+d
$$

$$
e=\frac{b}{2}
$$

Thế vào phương trình oxy:

$$
3b=6+2d+\frac{b}{2}
$$

Nhân cả hai vế với $2$:

$$
6b=12+4d+b
$$

$$
5b=12+4d
$$

Thay $b=2+d$:

$$
5(2+d)=12+4d
$$

$$
10+5d=12+4d
$$

$$
d=2
$$

Suy ra:

$$
b=4,\qquad e=2
$$

Vậy:

$$
a=1,\quad b=4,\quad c=1,\quad d=2,\quad e=2
$$

Do đó phương trình phản ứng cân bằng là:

$$
Cu+4HNO_3\rightarrow Cu(NO_3)_2+2NO_2+2H_2O
$$

---

# Bài toán: Tái cấu trúc hệ sinh thái

## Mô tả bài toán

Mô phỏng mối quan hệ giữa các loài sinh vật trong hệ sinh thái biển theo hướng tuyến tính. Mỗi loài vừa có khả năng sinh trưởng tự nhiên vừa chịu ảnh hưởng bởi các loài khác. Mục tiêu là tìm trạng thái cân bằng khi số lượng các loài không thay đổi theo thời gian.

## Bài toán

Một vùng biển có ba loài sinh vật chính:

- **Tảo biển:** phát triển tự nhiên và là nguồn thức ăn cho cá nhỏ.
- **Cá nhỏ:** ăn tảo biển và là thức ăn của cá mập.
- **Cá mập:** săn cá nhỏ để tồn tại.

Sau khi khảo sát thực địa, các nhà sinh học biển xác định được rằng:

- Mỗi $1000\text{ m}^2$ tảo biển phát triển thêm $200\text{ m}^2$ mỗi ngày.
- Mỗi con cá nhỏ tiêu thụ $400\text{ m}^2$ tảo biển mỗi ngày.
- Mỗi $1000\text{ m}^2$ tảo biển tạo điều kiện cho thêm $80$ con cá nhỏ mỗi ngày.
- Mỗi con cá nhỏ tự suy giảm $0,1$ con mỗi ngày và bị cá mập săn làm giảm $0,06$ con mỗi ngày.
- Mỗi con cá nhỏ cung cấp đủ năng lượng để duy trì $0,2$ con cá mập.
- Trung bình mỗi ngày số lượng cá mập suy giảm $0,4$ lần số lượng hiện có.

**Yêu cầu:** Hãy tìm tỉ lệ giữa diện tích tảo biển, số lượng cá nhỏ và số lượng cá mập khi hệ sinh thái biển ổn định.

## Lời giải

Gọi:

- $x$ là diện tích tảo biển (nghìn $\text{m}^2$).
- $y$ là số lượng cá nhỏ (con).
- $z$ là số lượng cá mập (con).

Khi hệ sinh thái ổn định thì lượng tăng và giảm của mỗi loài sau một ngày phải cân bằng.

### Đối với tảo biển

- Tảo biển phát triển thêm $0,2x$.
- Cá nhỏ tiêu thụ $0,4y$.

Do hệ ổn định nên:

$$
0,2x-0,4y=0
$$

$$
\Leftrightarrow x=2y
$$

### Đối với cá nhỏ

- Tăng thêm $0,08x$.
- Giảm tự nhiên $0,1y$.
- Bị cá mập săn mất $0,06z$.

Do hệ ổn định nên:

$$
0,08x-0,1y-0,06z=0
$$

### Đối với cá mập

- Tăng thêm $0,2y$.
- Giảm tự nhiên $0,4z$.

Do hệ ổn định nên:

$$
0,2y-0,4z=0
$$

$$
\Leftrightarrow z=0,5y
$$

Thế:

$$
x=2y,\qquad z=0,5y
$$

vào phương trình của cá nhỏ:

$$
0,08(2y)-0,1y-0,06(0,5y)=0
$$

$$
0,16y-0,1y-0,03y=0
$$

$$
0,03y=0,03y
$$

Phương trình luôn đúng nên hệ có vô số nghiệm tỉ lệ.

Suy ra:

$$
x:y:z=2y:y:0,5y
$$

Nhân cả ba số với $2$:

$$
x:y:z=4:2:1
$$

Vậy tỉ lệ cân bằng của hệ sinh thái biển là:

$$
4:2:1
$$

tức là cứ:

- $4000\text{ m}^2$ tảo biển,
- $2$ con cá nhỏ,
- $1$ con cá mập,

thì hệ sinh thái biển sẽ ổn định.

# Bài toán: Bài toán dân số

## Mô tả bài toán

Mô phỏng sự thay đổi dân số giữa các khu vực trong một thành phố. Dân số mỗi khu vực chịu ảnh hưởng bởi tốc độ sinh tự nhiên và sự di chuyển dân cư giữa các khu vực. Mục tiêu là tìm số dân của từng khu vực khi hệ thống đạt trạng thái cân bằng.

## Bài toán

Một thành phố gồm ba khu vực:

- **Khu A:** trung tâm thành phố.
- **Khu B:** khu dân cư ngoại ô.
- **Khu C:** khu công nghiệp.

Sau khi khảo sát, cơ quan thống kê xác định được rằng mỗi năm:

- Dân số khu A tăng thêm $10\%$ số dân hiện có và giảm $5\%$ do chuyển sang khu B.
- Dân số khu B nhận thêm dân từ khu A với lượng bằng $5\%$ dân số khu A, đồng thời giảm $8\%$ do chuyển sang khu C.
- Dân số khu C nhận thêm dân từ khu B với lượng bằng $8\%$ dân số khu B và giảm tự nhiên $4\%$.

Biết rằng khi hệ thống dân cư ổn định thì:

- Khu A tăng ròng $500$ người mỗi năm.
- Khu B không thay đổi dân số.
- Khu C không thay đổi dân số.

**Yêu cầu:** Tìm tỉ lệ dân số giữa ba khu vực khi hệ thống ổn định.

## Lời giải

Gọi:

- $x$ là dân số khu A.
- $y$ là dân số khu B.
- $z$ là dân số khu C.

### Đối với khu A

Khu A:

- Tăng $0,1x$.
- Giảm $0,05x$.

Do tăng ròng $500$ người nên:

$$
0,1x-0,05x=500
$$

$$
0,05x=500
$$

$$
x=10000
$$

### Đối với khu B

Khu B:

- Nhận thêm $0,05x$.
- Giảm $0,08y$.

Do dân số không đổi nên:

$$
0,05x-0,08y=0
$$

Thay $x=10000$:

$$
0,05\cdot10000-0,08y=0
$$

$$
500-0,08y=0
$$

$$
y=6250
$$

### Đối với khu C

Khu C:

- Nhận thêm $0,08y$.
- Giảm $0,04z$.

Do dân số không đổi nên:

$$
0,08y-0,04z=0
$$

Thay $y=6250$:

$$
0,08\cdot6250-0,04z=0
$$

$$
500-0,04z=0
$$

$$
z=12500
$$

Vậy dân số của ba khu vực lần lượt là:

$$
x=10000,\qquad y=6250,\qquad z=12500
$$

Do đó tỉ lệ dân số giữa ba khu vực là:

$$
10000:6250:12500
$$

Chia cả ba số cho $1250$, ta được:

$$
8:5:10
$$

Vậy tỉ lệ dân số ổn định giữa ba khu vực là:

$$
8:5:10
$$

tức là cứ:

- $8$ người ở khu A.
- $5$ người ở khu B.
- $10$ người ở khu C.

---

# Bài toán: Xác định đường cong dữ liệu

## Mô tả bài toán

Bài toán xác định đường cong dữ liệu là quá trình tìm một hàm toán học (thường là đa thức) mô tả tốt nhất mối quan hệ giữa các biến từ một tập hợp các điểm dữ liệu đã biết. Mục tiêu là tạo ra một mô hình toán học nhằm phân tích xu hướng, dự đoán giá trị hoặc đơn giản hóa việc biểu diễn dữ liệu thực nghiệm. Bằng cách thay thế các cặp giá trị dữ liệu vào dạng hàm giả định, bài toán sẽ dẫn đến một hệ phương trình đại số mà việc giải nó giúp xác định các hệ số của đường cong cần tìm.

## Bài toán

Tại một khu nghỉ dưỡng ven biển ở Nha Trang, ban quản lí muốn dự đoán nhiệt độ trong ngày để sắp xếp các hoạt động ngoài trời cho du khách như tắm biển, chèo thuyền và tham quan.

Qua quá trình quan sát, người ta nhận thấy nhiệt độ trong ngày biến thiên tuần hoàn và có thể được mô tả bởi một hàm lượng giác.

Người ta ghi nhận được rằng:

- Vào lúc 2 giờ sáng, nhiệt độ là $24^\circ C$.
- Vào lúc 8 giờ sáng, nhiệt độ là $30^\circ C$.
- Nhiệt độ cao nhất trong ngày đạt được vào lúc 14 giờ.

Người ta giả sử nhiệt độ thay đổi theo quy luật:

$$
T(t)=A\cos(\omega t+\omega_0)+b
$$

Trong đó:

- $t$ là thời gian tính theo giờ.
- $T(t)$ là nhiệt độ tính theo $^\circ C$.

**Yêu cầu:** Hãy dự đoán nhiệt độ tại khu nghỉ dưỡng này vào lúc 11 giờ và 14 giờ.

## Lời giải

Gọi $T(t)$ là nhiệt độ trung bình tại thời điểm $t$ (giờ), với:

$$
T(t)=A\cos(\omega t+\omega_0)+b
$$

Theo dữ liệu bài toán ta có:

$$
T(2)=24,\qquad T(8)=30 \qquad (1)
$$

Do nhiệt độ lớn nhất đạt được vào lúc $14$ giờ nên hàm số đạt giá trị lớn nhất tại $t=14$.

Mà hàm $\cos$ đạt giá trị lớn nhất khi:

$$
\omega t+\omega_0=2k\pi
$$

Để thuận tiện tính toán, ta chọn:

$$
14\omega+\omega_0=0
\Leftrightarrow
\omega_0=-14\omega
$$

Do đó:

$$
T(t)=A\cos(\omega(t-14))+b \qquad (2)
$$

Ngoài ra, nhiệt độ trong ngày có tính tuần hoàn theo chu kì $24$ giờ nên:

$$
T(0)=T(24)
$$

Mà hàm $\cos$ có chu kì $2\pi$ nên:

$$
24\omega=2\pi
$$

$$
\Leftrightarrow \omega=\frac{\pi}{12} \qquad (3)
$$

Từ (2) và (3), ta được:

$$
T(t)=A\cos\left(\frac{\pi}{12}(t-14)\right)+b
$$

Sử dụng dữ kiện trong (1), ta có hệ phương trình:

$$
\begin{cases}
A\cos\left(\dfrac{\pi}{12}(2-14)\right)+b=24\\
A\cos\left(\dfrac{\pi}{12}(8-14)\right)+b=30
\end{cases}
$$

$$
\Leftrightarrow
\begin{cases}
A\cos(-\pi)+b=24\\
A\cos\left(-\dfrac{\pi}{2}\right)+b=30
\end{cases}
$$

$$
\Leftrightarrow
\begin{cases}
-A+b=24\\
b=30
\end{cases}
$$

$$
\Leftrightarrow
\begin{cases}
A=6\\
b=30
\end{cases}
$$

Vậy nhiệt độ trung bình trong ngày được mô tả bởi hàm số:

$$
T(t)=6\cos\left(\frac{\pi}{12}(t-14)\right)+30
$$

Suy ra:

- **Vào lúc 11 giờ:**

$$
T(11)=6\cos\left(\frac{\pi}{12}(11-14)\right)+30
$$

$$
=6\cos\left(-\frac{\pi}{4}\right)+30
$$

$$
=6\cdot\frac{\sqrt{2}}{2}+30
$$

$$
=3\sqrt{2}+30\approx34,24^\circ C
$$

- **Vào lúc 14 giờ:**

$$
T(14)=6\cos(0)+30
$$

$$
=36^\circ C
$$

Vậy:

- Nhiệt độ lúc 11 giờ khoảng $34,24^\circ C$.
- Nhiệt độ lúc 14 giờ là $36^\circ C$.

---

# KẾT LUẬN

Qua quá trình tìm hiểu và thực hiện dự án, tôi đã có cơ hội ôn tập, củng cố và hệ thống lại các kiến thức liên quan đến hệ phương trình đại số, được tiếp cận với nhiều dạng hệ phương trình khác nhau cũng như những ứng dụng thực tế của chúng trong đời sống, khoa học và kĩ thuật. Điều này giúp tôi nhận ra rằng toán học nói chung và hệ phương trình nói riêng không chỉ mang ý nghĩa lí thuyết mà còn là công cụ quan trọng để mô hình hóa và giải quyết các bài toán thực tiễn.

Thông qua việc xây dựng các ví dụ minh họa và phân tích các bài toán ứng dụng, tôi đã bước đầu rèn luyện được khả năng tìm kiếm tài liệu, chọn lọc thông tin, trình bày vấn đề theo hướng logic và khoa học. Đây là những kĩ năng cần thiết cho quá trình học tập, nghiên cứu cũng như thực hiện các dự án lớn hơn trong tương lai.

Bên cạnh đó, quá trình thực hiện dự án cũng giúp tôi hiểu rõ hơn về phương pháp tự học, chủ động tìm tòi kiến thức ngoài phạm vi chương trình học trên lớp. Đây sẽ là nền tảng quan trọng giúp tôi tiếp tục nghiên cứu và thực hiện các dự án, khóa luận hoặc những công trình học thuật sau này.

Tôi xin bày tỏ lòng biết ơn sâu sắc tới Thầy giáo hướng dẫn TS.Nguyễn Đăng Minh Phúc đã tận tình hướng dẫn, góp ý và hỗ trợ tôi trong suốt quá trình thực hiện dự án.

Mặc dù đã rất cố gắng trong quá trình thực hiện, song do thời gian nghiên cứu và kiến thức bản thân còn hạn chế nên dự án khó tránh khỏi những thiếu sót nhất định. Tôi rất mong nhận được những ý kiến đóng góp và nhận xét từ quý thầy cô và các bạn để dự án được hoàn thiện hơn.

Xin chân thành cảm ơn!

# TÀI LIỆU THAM KHẢO

1. Linh, T. N. K. (Chủ biên), Đồng, P. Đ., Long, L. N., & Tuân, H. Đ. (2024). *Giáo trình đại số tuyến tính I*. Trường Đại học Sư phạm - Đại học Huế.

2. Khánh, N. P., & Khánh, H. Đ. (2017). *Bài tập phương trình và hệ phương trình có lời giải chi tiết*. Toanmath.com.

3. Hào, H. C. (2021). *Chuyên đề phương trình và hệ phương trình*. Sachhoc.com.

4. Em, N. C. (2019). *Chuyên đề phương trình và hệ phương trình*. Toanmath.com.

5. [Sách giáo khoa Toán 9 - Kết nối tri thức với cuộc sống](https://thcs.toanmath.com/2023/12/sach-giao-khoa-toan-9-tap-1-ket-noi-tri-thuc-voi-cuoc-song.html)

6. [Một số phương pháp giải phương trình, hệ phương trình](https://toanmath.com/2021/11/mot-so-phuong-phap-giai-phuong-trinh-he-phuong-trinh-tran-hoai-vu.html)
