# 90DegreeMatrix

Để giải quyết câu hỏi mà không có bất kỳ khoảng trống nào, hãy xoay mảng dưới dạng hình vuông, chia ma trận thành hình vuông hoặc chu kỳ. Ví dụ, 
ma trận A 4 X 4 sẽ có 2 chu kỳ. Chu kỳ đầu tiên được hình thành bởi hàng đầu tiên, cột cuối cùng, hàng cuối cùng và cột đầu tiên của nó. Chu kỳ thứ hai được hình thành bởi hàng thứ 2, cột thứ hai cuối cùng, hàng thứ hai cuối cùng và cột thứ 2. Ý tưởng là đối với mỗi chu kỳ vuông, hoán đổi các phần tử có liên quan đến ô tương ứng trong ma trận theo hướng ngược chiều kim đồng hồ, tức là từ trên sang trái, từ trái sang dưới, từ dưới sang phải và từ phải lên trên cùng một lúc mà không sử dụng gì khác ngoài một biến tạm thời để đạt được điều này.

Đặt kích thước của hàng và cột là 3. 
Trong lần lặp đầu tiên - 
a [i] [j] = Phần tử ở chỉ mục đầu tiên (phần trên cùng góc bên trái) = 1.
a [j] [n-1-i] = Phần tử ở đầu góc ngoài cùng bên phải Phần tử = 3.
a [n-1-i] [n-1-j] = Phần tử ở góc ngoài cùng bên phải = 9.
a [n-1-j] [i] = Phần tử ở góc ngoài cùng bên trái = 7.
Di chuyển các phần tử này theo chiều kim đồng hồ phương hướng. 
Trong lần lặp thứ hai - 
a [i] [j] = 2.
a [j] [n-1-i] = 6.
a [n-1-i] [n-1-j] = 8.
a [n- 1-j] [i] = 4. 
Tương tự, di chuyển các phần tử này theo chiều kim đồng hồ. 
