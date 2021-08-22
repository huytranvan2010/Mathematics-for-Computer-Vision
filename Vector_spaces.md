

# Vectors and vector spaces
## Multidimensional vector spaces
Có thể hiểu đơn giản **vector là một mảng các giá trị số**. Mỗi số trong mảng được coi như tọa độ của vector hay thành phần của vector. Chiều của vector chính là số thành phần (hay số tọa độ của nó)
Ví dụ  $(1, 2, 3.3)$ là vector có 3 chiều

**Sparse vector** - vector mà các thành phần của nó chủ ýếu là 0, ví dụ $(0, 1, 0, 0, 0, 0, 0.1)$ - sparse vector có chiều là 7

Định nghĩa chính thức của sparse vector: vector n chiều được coi là sparse nếu số thành phần của nó bị giới hạn bởi $\alpha n$, ở đây $\alpha \ll 1$.

**Không gian vector** - không gian các vector có cùng chiều. Đây là không gian tuyến tính (linear space) vì trong này xác định 2 phép tính (operations):
* Nhân với số vô hướng (scalar): mỗi thành phần của vector được nhân với số vô hướng
* Phép cộng hai vector được vector mới. Thành phần (tọa độ) của vector mới bằng tổng 2 thành phần tương ứng các các vector ban đầu.

Tổng quát hơn chúng ta đi tìm hiểu về một số tiên đề của không gian vector.
**Real vector space** - tập hợp $V$ với 2 phép tính:
* Nhân vô hướng: cho vector $\textbf{x}\in V$ và số thực $c$, tích của $\textbf{x}$ và $c$ là vector $c\textbf{x}$ cũng thuộc $V$
* Cộng: cho vectors $\textbf{x}, \textbf{y} \in V$, tổng của $\textbf{x}$ và $\textbf{y}$ là một vector thuộc $V$ 

**Tiên đề cho phép cộng vector**:
* Phép cộng có tính giao hoán (coomutative): $\textbf{x}+\textbf{y} = \textbf{y}+\textbf{x}$
* Phép cộng có tính kết hợp: $(\textbf{x}+\textbf{y})+\textbf{z}=\textbf{x}+(\textbf{y}+\textbf{z})$
* Phần tử 0. Tồn tại phần tử 0 sao cho $\textbf{x}+0=0+\textbf{x}=\textbf{x}$
* Phần tử nghich đảo. Cho mỗi phần tử $\textbf{x}$ tồn tại $(-\textbf{x})$ sao cho $\textbf{x}+(-\textbf{x})=(-\textbf{x})+\textbf{x}=0$

**Tiên đề cho phép nhân vô hướng**:
* Cho vector $\textbf{x} \in V$ và các số nguyên $c, d$ ta có: $0*\textbf{x}=0$, $1*\textbf{x}=\textbf{x}$, $(cd)\textbf{x}=c(d\textbf{x})$
* Tính phân phối: Cho vectors $\textbf{x}, \textbf{y} \in V$ và các số nguyên $c, d$:
    * $c(\textbf{x}+\textbf{y})=c\textbf{x}+c\textbf{y}$
    * $(c+d)\textbf{x}=c\textbf{x}+d\textbf{x}$

**Một số kí hiệu toán học**
$\mathbb{R}$ - tập hợp các số thực
Vector, mảng các số thực có thể được biểu theo hàng hoặc theo cột.
$\mathbb{R}^{1\times n}$ - không gian vector hàng có chiều n
$\mathbb{R}^{n\times 1}$ - không gian vector cột có chiều n
$\mathbb{R}^{n}$ - không gian vector n chiều

Vector hàng có thể được biểu diễn như sau $\textbf{x}=(x_1, x_2,...,x_n)$, ở đây $x_i$ là tọa tọa $i^{th}$ của vector $\textbf{x}$.
*Linear combination* của 2 vector $\textbf{x}, \textbf{y}$:

$$\alpha \textbf{x} + \beta \textbf{y} =\alpha(x_1, x_2,...,x_n)+\beta(y_1, y_2,...,y_n)=(\alpha x_1 + \beta y_1, \alpha x_2 + \beta y_2,...,\alpha x_n + \beta y_n)$$

Vector cột có thể được biểu diễn như sau $\textbf{x}=\begin{bmatrix}
 x_1\\
 x_2\\
 ...\\
 x_n\\
\end{bmatrix}$

*Linear combination* của 2 vector cột được biểu diễn như sau: 
$$\alpha \textbf{x} + \beta \textbf{y} = \begin{bmatrix}
 \alpha x_1\\
 \alpha x_2\\
 ...\\
 \alpha x_n\\
\end{bmatrix} + \begin{bmatrix}
 \beta y_1\\
 \beta y_2\\
 ...\\
 \beta x_n\\
\end{bmatrix} = \begin{bmatrix}
 \alpha x_1 + \beta y_1\\
 \alpha x_2 + \beta y_2\\
 ...\\
 \alpha x_n + \beta y_n\\
\end{bmatrix}$$

Vector hàng có thể chuyển thành vector cột và ngược lại bằng chuyển vị, chuyển vị của $\textbf{x}$ là $\textbf{x}^T$.
Ví dụ $\textbf{x}=(1, 2, 3, 4)$,  $\textbf{x}^T=\begin{bmatrix}
 1\\
 2\\
 3\\
 4\\
\end{bmatrix}$. Ở đây đối với vector hàng có thể dùng ngoặc vuông cũng được không sao cả.