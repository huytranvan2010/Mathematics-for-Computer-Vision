
Cho ma trận vuông $\textbf{A} \in \mathbb{R}^{n \times n}$. Ma trận nghịch đảo (inverse matrix) của ma trận A kí hiệu là $\textbf{A}^{-1}$ cũng là ma trận vuông thỏa mãn:

$$\textbf{A} \cdot \textbf{A}^{-1} = \textbf{A}^{-1} \cdot \textbf{A} = \textbf{I}_n  $$

Đối với ma trận đơn vị : $$\textbf{I}_n^{-1} = \textbf{I}_n  $$

Đối với ma trận đường chéo $\textbf{D} = diag(d_1, d_2, \dots, d_n) $ thì : 

$$ \textbf{D}^{-1} =  diag(1/d_1, 1/d_2, \dots, 1/d_n)$$

Đối với ma trận trực giao $\textbf{A}$ thì:

$$\textbf{A}^{-1} = \textbf{A}^T$$

cái này do tính chất của ma trận trực giao.

Ngoài ta chúng ta có $(\textbf{A}^T)^{-1} = (\textbf{A}^{-1})^T$

**Định thức ma trận (matrix determinant**)

Một số tính chất:
- $det(diag(d_1, d_2, \dots, d_n)) = d_1 d_2 \dots d_n$
- $det(\textbf{A}^T) = det(\textbf{A})$
- $det(\textbf{A} \cdot \textbf{B}) = det(\textbf{B} \cdot \textbf{A})$
- Cho ma trận trực giao $\textbf{A}$: $det(\textbf{A}) = 1$
- Nếu $\textbf{A}$ là ma trận đường chéo trên thì $det(\textbf{A})$ bằng tích tất cả các phần tử trên đường chéo của nó

**Công thức cho ma trận nghịc đảo**

Cho $\textbf{A} \in \mathbb{R}^{n \times n}$, ma trận nghịch đảo của $\textbf{A}$ tồn tại nếu $det(\textbf{A}) \neq 0$

$$\textbf{A}^{-1} = \frac{1}{det(\textbf{A})} (\textbf{A}_{cof})^T$$

trong đó $\textbf{A}_{cof}$ là matrix of cofactors, $\textbf{A}_{cof} = (\textbf{A}_{ij})$

$\textbf{A}_{ij} = (-1)^{i+j} det(\textbf{M}_{ij})$

trong đó $\textbf{M}_{ij}$ là ma trận có được từ ma trận $\textbf{A}$ bằng cachs loại bỏ hàng $i$ và cột $j$.

**Ma trận full rank**

Cho $\textbf{A} \in \mathbb{R}^{n \times n}$:

$$Rank(\textbf{A}) = n$$ khi vào chỉ khi $det(\textbf{A}) \neq 0$.


