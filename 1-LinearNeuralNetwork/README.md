
## Table of Content. 
- [I. Các thành phần cơ bản của Linear Regression]()
	- 1. [Mô hình tuyến tính.]()
	- 2. [Hàm mất mát.]()
	- 3. [Nghiệm theo công thức.]()
	- 4. [Hạ Gradient.]()
	- 5. [Dự đoán bằng mô hình đã huấn luyện.]()
	- 6. [Vector hóa để tăng tốc độ tình toán.]()
- [II. Phân phối chuẩn và Hàm mất mát bình phương.]()
- [III. Từ Hồi quy tuyến tính tới mạng học sâu]

## I. Các thành phần cơ bản của Linear Regression

### 1. Mô hình tuyến tính.

Giả định tuyến tính trên cho thấy rằng mục tiêu (giá nhà) có thể được biểu diễn bởi tổng có trọng số của các đặc trưng (diện tích và tuổi đời):

$$ 
price = w_{diện_tích}.diện_tích + w_{tuổi_đời}.tuổi_đời + b 
$$

Ở đây,  $ w_{diện_tích} $ và $ w_{tuổi_đời} $ được gọi là các trọng số, và  b  được gọi là hệ số điều chỉnh (còn được gọi là độ dời).

$$
 \hat{y}=Xw+b.\
$$

### 2. Hàm mất mát.

$$
L(w, b) = \frac{1}{2}( \hat{y}^{(i)}-y^{(i)})^{2} 
$$

### 3. Nghiệm theo công thức

$$ 
w^{*}=(X^{T}X)^{−1}X^{T}y. 
$$

Tuy những bài toán đơn giản như hồi quy tuyến tính có thể có nghiệm theo công thức, bạn không nên làm quen với sự may mắn này. Mặc dù các nghiệm theo công thức giúp ta phân tích toán học một cách thuận tiện, các điều kiện để có được nghiệm này chặt chẽ đến nỗi không có phương pháp học sâu nào thoả mãn được.

### 4. Hạ Gradient.

$$
(w,b) \leftarrow (w,b)−\frac{\eta}{\|\beta\|}\sum_{i \in \beta}\partial_{(w,b)}l^{(i)}(w,b) 
$$


### 5. Dự đoán bằng mô hình đã huấn luyện.

Với mô hình hồi quy tuyến tính đã được huấn luyện $ \hat{w^{T}}x+\hat{b} $, ta có thể ước lượng giá của một căn nhà mới (ngoài bộ dữ liệu dùng để huấn luyện) với diện tích  x1 và tuổi đời x2 của nó. Việc ước lượng mục tiêu khi biết trước những đặc trưng thường được gọi là dự đoán hay suy luận (inference).

### 6. Vector hóa để tăng tốc độ tình toán.

Khi huấn luyện mô hình, chúng ta thường muốn xử lý đồng thời các mẫu dữ liệu trong minibatch. Để làm được điều này một cách hiệu quả, chúng ta phải vector hóa việc tính toán bằng cách sử dụng các thư viện đại số tuyến tính thay vì sử dụng các vòng lặp for trong Python.

## II. Phân phối Chuẩn và Hàm mất mát Bình phương

