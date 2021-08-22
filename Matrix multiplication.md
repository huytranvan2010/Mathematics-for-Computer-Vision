Ma trận $\textbf{A} \in \mathbb{R}^{m \times p} $, ma trận $\textbf{B} \in \mathbb{R}^{p \times m} $. $\textbf{C} \in \mathbb{R}^{n \times m}$ là tích của ma trận $\textbf{A}$ với ma trận $\textbf{B}$. Các phần tử của ma trận $\textbf{C}$ được xác định như sau:

$$c_{ij} = \sum_{k=1}^{p} a_{ik} b_{kj} $$

$c_{ij}$ sẽ là tích vô hướng của vector hàng $i$ của ma trận $\textbf{A}$ với cột $j$ của ma trận $\textbf{B}$ (nhớ chuyển về cùng hàng hoặc cột trước đã).

Một số tính chất $\textbf{A}, \textbf{E} \in \mathbb{R}^{m \times p} $, $\textbf{B} \in \mathbb{R}^{p \times m} $:

$$ (\textbf{A} + \textbf{E})\textbf{B} = \textbf{A} \textbf{B} + \textbf{E} \textbf{B} $$

$$ (\textbf{A} \textbf{B})^T = \textbf{B}^T \textbf{A}^T $$

> **Tip**: có ngoài cách ở trên có thể nhân ma trận đơn giản theo 2 cách nữa như sau:
    - Cột của ma trận $\textbf{C}$ là tích của ma trận $\textbf{A}$ và cột ma trận $\textbf{B}$ tương ứng. 
    - Hàng của ma trận $\textbf{C}$ là tích của hàng ma trận $\textbf{A}$ tương ứng và ma trận $\textbf{B}$. 
Hãy thử xem, điều trên là đúng đấy.

$\textbf{a} $ là vector hàng có chiều $1 \times n, \textbf{a} \in \mathbb{R}^{1 \times n}$
$\textbf{b} $ là vector hàng có chiều $n \times 1, \textbf{a} \in \mathbb{R}^{n \times 1}$

$\textbf{a} \cdot \textbf{b}$ là ma trận có chiều $1 \times 1$ (real number), $rank(\textbf{a} \cdot \textbf{b}) = 1$

$\textbf{b} \cdot \textbf{a}$ là ma trận có chiều $n \times n$ (real number), $rank(\textbf{a} \cdot \textbf{b}) = 1$ (điều này khá rõ ràng chỉ có 1 vector độc lập tuyến tính).





