Verilen diziyi ([7, 5, 1, 8, 3, 6, 0, 9, 4, 2]) sırasıyla ele alarak bir Binary Search Tree (BST) oluşturalım. İlk elemanı kök (root) olarak alarak ağacı inşa etmeye başlıyoruz ve her bir sayıyı yerleştirirken sağa veya sola yerleştiriyoruz.

1. Adım: Root'u Belirleme
İlk eleman her zaman ağacın kökü olur.
Root = 7
2. Adım: Diğer Elemanları Ekleyerek Ağaç Oluşturma
5: 5, kök olan 7’den küçük. Bu yüzden 5’i root’un soluna ekliyoruz.

Root'un solu: 5
1: 1, hem 7’den hem de 5’ten küçük. Bu nedenle, 5’in soluna ekliyoruz.

5’in solu: 1
8: 8, kök olan 7’den büyük. Bu yüzden, 8’i root’un sağına ekliyoruz.

Root'un sağı: 8
3: 3, 7’den ve 5’ten küçük, ancak 1’den büyük. Bu nedenle, 1’in sağına ekliyoruz.

1'in sağı: 3
6: 6, 7’den küçük, ancak 5’ten büyük. Bu yüzden, 5’in sağına ekliyoruz.

5'in sağı: 6
0: 0, hem 7’den, 5’ten ve 1’den küçük. Bu nedenle, 1’in soluna ekliyoruz.

1'in solu: 0
9: 9, 7’den ve 8’den büyük. Bu nedenle, 8’in sağına ekliyoruz.

8'in sağı: 9
4: 4, 7’den ve 5’ten küçük, ancak 1 ve 3’ten büyük. Bu yüzden, 3’ün sağına ekliyoruz.

3'ün sağı: 4
2: 2, 7’den, 5’ten ve 3’ten küçük, ancak 1’den büyük. Bu yüzden, 3’ün soluna ekliyoruz.

3'ün solu: 2
Sonuç Olarak Oluşan Binary Search Tree:
Ağaç yapımız şu şekilde oluşur:

markdown
Kodu kopyala
         7
       /   \
      5     8
     / \     \
    1   6     9
   / \
  0   3
     / \
    2   4