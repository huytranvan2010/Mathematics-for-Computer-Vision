**Orthogonal system** of vectors (hệ vector trực giao). Giả sử $E$ là không gian Euclid. Bộ các vector $ \mathbf{u}_1, \mathbf{u}_2 ... \mathbf{u}_n $ được gọi là hệ trực giao nếu các vector đôi một trực giao với nhau:

$$ \left< \mathbf{u}_i, \mathbf{u}_j \right> = 0, for i\neq j, i,j=1,2...n  $$

Hệ vector trực giao luôn độc lập tuyến tính. Một cơ sở là hệ trực giao thì gọi là cơ sở trực giao.

$ V \subset \mathbb{R}^n $. Bộ các vector $ \mathbf{u}_1, \mathbf{u}_2 ... \mathbf{u}_n $ được gọi là cơ sở trực giao của $V$ nếu:
* $ \mathbf{u}_1, \mathbf{u}_2 ... \mathbf{u}_m $ là hệ trực giao
* $span(\mathbf{u}_1, \mathbf{u}_2 ... \mathbf{u}_m) = V$ (có thể tạo ra các vector thuộc $V$ từ bộ các vector đó)

**Orthomormal system** (hệ trực chuẩn) 
Hệ trực giao $ \mathbf{x}_1, \mathbf{x}_2 ... \mathbf{x}_n $ được gọi là trực chuẩn nếu :
$$ \left< \mathbf{u}_i, \mathbf{u}_i \right> = 1 $$

Đối với hệ trực chuẩn ta có: $\left\| \mathbf{u}_i \right\| = 1$

Làm sao để chuyển hệ trực giao thành trực chuẩn?
Gram-Schmidt algorithm: chuyển hệ vector $ \mathbf{x}_1, \mathbf{x}_2 ... \mathbf{x}_k $ thành hệ trực chuẩn $ \mathbf{u}_1, \mathbf{u}_2 ... \mathbf{u}_m $ để mà:

$$ span( \mathbf{x}_1, \mathbf{x}_2 ... \mathbf{x}_k ) = span( \mathbf{u}_1, \mathbf{u}_2 ... \mathbf{u}_m )$$

Trong trường hợp này $dim(span( \mathbf{x}_1, \mathbf{x}_2 ... \mathbf{x}_k )) = m$

Nếu $ \mathbf{u}_1, \mathbf{u}_2 ... \mathbf{u}_m $ là cơ sở trực chuẩn của không gian con $V$ khi đó với mọi $\mathbf{u} \in V$ ta có:

$$ \mathbf{u} = \left< \mathbf{u}, \mathbf{u}_1 \right> \mathbf{u}_1 + \left< \mathbf{u}, \mathbf{u}_2 \right> \mathbf{u}_2 + ... + \left< \mathbf{u}, \mathbf{u}_m \right> \mathbf{u}_m   $$


Áp dụng tính trực giao trong không gian Euclid chúng ta có thể xác định được projection (hình chiếu). 

#### Tài liệu tham khảo
1. https://www.coursera.org/learn/mathematics-for-computer-vision/lecture/o7tHD/orthogonal-basis-projection


