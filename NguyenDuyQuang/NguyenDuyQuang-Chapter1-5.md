5
code1
a) Hàm cần trả về chỉ số cuối cùng của phần tử y nhưng vì không lấy giá trị đầu array nên nó bị thiếu
sửa thành for(int i = x.length() - 1; i >= 0; --i)
b) x=[1,2,3,4]; y = 4 đáp án là 3
c)  x = [0;1;2;3;4]; y = 1 đáp án 1 nó bỏ qua số 0 nên đáp án vẫn đúng
d)x = [0;1;2;3;4]; y = -1; Đáp án: -1. nó không tìm được y nên nó sẽ trả về -1
e) nó chỉ duyệt đến i=1 rồi dừng ko duyệt i-0 nên lỗi
code2
a) thay vì trả về giá trị cuối thì nó lại trả về giá trị đầu tiên của số 0
 sửa lại thành :for(int i = x.length()-1; i >= 0; i--)
b)trường hợp ko lỗi:[0,1,2,3,4] nó vẫn trả về 1 vì chỉ có 1 số 0
c)trường hợp gây ra lỗi : [0,1,0] nó trả về 0
d)x = [7,0,9,6] đáp án: 1.
e)nó tìm đến vị trí 0 đầu đã dừng nên ko tìm đc số 0 ở sau

code3
a hàm yêu cầu lấy số nguyên dương nhưng nó lại lấy cả 0 nên bị sai
sửa thành if (x[i] >0)
b trường hợp không gây lỗi [2,9,8] đáp án 3 

c trường hợp không gây lỗi [0,2,9,8] đáp án 4

e vì nó tính cả số 0 nên đáp ánh bị sai

code 4:
a hàm cần trả về số > 0 hoặc là chia 2 dư 1 nhưng nó lại không tính trường hợp số âm chua 2 dư 1 nên sai
sửa thanh thành "if (x[i]%2 == -1 || x[i] > 0)"
b x=[1,2,3],đáp án: 3
c x = [-3,0;4], đáp án: 2
e -3 chia 2 dư 1 nhưng không được đếm nên đáp án sai