
# Proje 2 - Merge Sort
### [16,21,11,8,12,22]

### Yukarıdaki dizinin merge sort aşamaları;


***Bölme aşaması: Verilen dizi daha küçük parçalara bölünür. Bölünme, her dizi tek bir eleman kalana kadar tekrarlanır.***


- [16 21 11] [8 12 22]

- [16] , [21 11] [8 12] ,[ 22]

- [16] , [21] , [11] [8] , [12] , [22]   

- [11 16 21]   [8 12 22 ]

- [8 11 12 16 21 22]

---
***Big-O gösterimini yazınız.***

Big-O gösterimi O(n log n) olarak ifade edilir.

Bölme aşaması: Algoritma, giriş dizisini daha küçük parçalara böler. Her bir bölme işlemi, dizinin boyutunu yarıya indirir. Bu nedenle, bu bölme işlemi logaritmik zaman karmaşıklığına (log n) sahip olacaktır. Çünkü, genel olarak, bir şeyi sürekli olarak yarıya böldüğümüzde, bunu logaritmik sayıda kez yapabiliriz.

Birleştirme aşaması: Daha sonra, bu küçük parçalar, sıralanmış bir dizi oluşturmak üzere birleştirilir. Her bir birleştirme işlemi, en kötü durumda, her elemanın bir kez karşılaştırılmasını gerektirir, bu da birleştirme işleminin lineer zaman karmaşıklığına (n) sahip olacağı anlamına gelir.

Bu iki aşamanın birleşimi, Merge Sort'un O(n log n) zaman karmaşıklığına sahip olmasını sağlar. Çünkü her bölme adımında (log n), her eleman üzerinde bir işlem gerçekleştiriyoruz (n).