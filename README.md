- 👋 Hi, I’m @taylorlona
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
taylorlona/taylorlona is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
Sắp xếp chọn hay selection sort sẽ là thuật toán thứ hai mà mình giới thiệu đến các bạn, ý tưởng của thuật toán này như sau:
void Swap(int &a, int &b){
    int temp = a;
    a = b;
    b = temp;
}

void InterchangeSort(int a[], int n){	
    for (int i = 0; i < n - 1; i++)
        for (int j = i + 1; j < n; j++)
	        if(a[i] > a[j])  //nếu có nghịch thế thì đổi chỗ
		        Swap(a[i], a[j]);
}
