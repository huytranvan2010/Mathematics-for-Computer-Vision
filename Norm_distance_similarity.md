**Norm of vector**
Cho vector $\mathbf{x}\in \mathbb{R}^{n}$. Làm sao để xác định vector $\mathbf{x}$ nằm xa vector $\mathbf{0}$. Hay vector "lớn", "nhỏ" có nghĩa là gì? Để trả lời câu hỏi đó chúng ta cùng tìm hiểu khái niệm **norm**.

**Norm** của vector $\mathbf{x}$ được kí hiệu là $\left\|\mathbf{x} \right\|$.

**Các tiên đề về norm:**
* Norm không âm: $\left\|\mathbf{x} \right\| \geqslant 0$, $\left\|\mathbf{x} \right\| = 0$ khi và chỉ khi $\mathbf{x} = \mathbf{0}$
* $\left\|\alpha \mathbf{x} \right\| = \left| \alpha \right| \left\| \mathbf{x} \right\|$, với $\alpha \in \mathbb{R}$
* Bất đăng thức tam giác: $\left\| \mathbf{x} + \mathbf{y} \right\| \leq \left\|\mathbf{x} \right\| + \left\|\mathbf{y} \right\|$

Có rất nhiều loại norm khác nhau, hay dùng nhất là norm $L1$ và norm $L2$.
**Manhattan norm**: cho vector $\mathbf{x}\in \mathbb{R}^{n}$
$$ \left\|\mathbf{x} \right\|_{1} = \sum_{i=1}^{n}\left| x_i \right| $$

**Euclidean norm**: cho vector $\mathbf{x}\in \mathbb{R}^{n}$
$$ \left\|\mathbf{x} \right\|_{2} = \left (\sum_{i=1}^{n}\left| x_i \right|^2  \right )^\frac{1}{2} $$

**Minkowski norm**: cho vector $\mathbf{x}\in \mathbb{R}^{n}$
$$ \left\|\mathbf{x} \right\|_{p} = \left (\sum_{i=1}^{n}\left| x_i \right|^p  \right )^\frac{1}{p}, p \geqslant 1 $$, 

**Chebyshev norm**: cho vector $\mathbf{x}\in \mathbb{R}^{n}$
$$ \left\|\mathbf{x} \right\|_{\infty}=\underset{1\leqslant i\leq n}{max}\left|x_{i} \right| $$

**Negative infinity norm:** cho vector $\mathbf{x}\in \mathbb{R}^{n}$
$$ \left\|\mathbf{x} \right\|_{-\infty}=\underset{1\leqslant i\leq n}{min}\left|x_{i} \right| $$

**Norm trong không gian của các hàm liên tục**
$C\left [a, b \right ]$ là tập hơp các hàm liên tục $x(t)$ trên đoạn $\left [a, b \right ]$. Đây là không gian vector tuyến tính.
https://www.coursera.org/learn/mathematics-for-computer-vision/lecture/ig1Mq/norm-of-vectors-distance-similarity

**Distance (dissimilarity)**
Khoảng cách giữa hai vector $\mathbf{x}, \mathbf{y} \in \mathbb{R}^{n}$ có thể được xác định như sau:
$$ d(\mathbf{x} , \mathbf{y}) = \left\|\mathbf{x} - \mathbf{y} \right\|  $$

**Các tiên đề về khoảng cách:**
* Khoảng cách không âm, $d(\mathbf{x} , \mathbf{y}) \geq 0$, dấu $=$ xảy ra khi và chỉ khi $\mathbf{x} = \mathbf{y}$
* Khoảng cách có tính đối xứng: $d(\mathbf{x} , \mathbf{y}) = d(\mathbf{y} , \mathbf{x})$ 
* Bất đẳn thưc tam giác: $d(\mathbf{x} , \mathbf{y}) \leq d(\mathbf{x} , \mathbf{z}) + d(\mathbf{z} , \mathbf{y})$

Các norm khác nhau tạo ta khoảng cách giữa các vector khác nhau.

Trong xử lý ảnh có thể biể diễn ảnh dưới dạng vector (được duỗi ra), sau đó chúng ta có thể đo lường độ tương đồng giữa các ảnh thông qua khoảng cách của các vector đó.

Có nhiều cách để chuyển khoảng cách $d(\mathbf{x} , \mathbf{y})$ giữa 2 vector $\mathbf{x}, \mathbf{y}$ sang độ tương đồng (similarity) giữa 2 vector đó. Một trong những cách chuyển đó là Gaussian:
$$sim(\mathbf{x}, \mathbf{y}) = exp\left ( \frac{-d^{2}(\mathbf{x},\mathbf{y})}{\sigma ^{2}} \right )$$
ở đây $\sigma$ là tham số tỉ lệ được chọn cho từng mục đích khác nhau, $0 \leq sim(\mathbf{x}, \mathbf{y}) \leq 1$





