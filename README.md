# SORU 1
# [7, 5, 1, 8, 3, 6, 0, 9, 4, 2] dizisinin Binary-Search-Tree aşamalarını yazınız.
# Örnek: root x'dir. root'un sağından y bulunur. Solunda z bulunur vb.

# ÇÖZÜM : 
İlk yapmamız gereken bir root (kök) belirlemek ve bu algoritma sisteminde ilk elemanız Root olacaktır.
Root belirlendikten sonra sırasıyla elemanlar önce root ile karşılaştırılarak işleme başlanır.
Root'un sol tarafına küçük sayılar, sağ tarafına ise büyük sayılar yazılır.
Ama her elemanın 2 den fazla eleman yazılamaz işlemler sırasında.

- Root 7'dir.
*   7
- 5 sayısı /'sayısından küçük olduğu için sola yazılır.
*    7
    /
   5
- 1 sayısı 7'den küçük, 5'ten küçük bu yüzden 5'in soluna yazılır
*     7
     /
    5
   /
  1
- 8 sayısı 7'den büyük bu yüzden sağına yazılır.
*      7
     /   \
    5     8
   /
  1
- 3 sayısı 7 ve 5'ten küçük, 1'den büyük olduğu için 1'in sağına yazılır.
*      7
     /   \
    5     8
   /
  1
   \
    3
- 6 sayısı 7'den küçük, 5'ten büyük olduğu için 5'in sağına yazılır.
*      7
     /   \
    5     8
   / \
  1   6
   \
    3
- 0 sayısı 7,5,1 den küçük olduğu için 1'in soluna yazılır.
*       7
      /   \
     5     8
    / \
   1   6
  / \
 0   3
- 9 sayısı 7 ve 8 'den büyük olduğu için 8'in sağına yazılır.
*       7
      /   \
     5     8
    / \     \
   1   6      9
  / \
 0   3
- 4 sayısı 7 ve 5'ten küçük, 1 ve 3'ten de büyük olduğu için sağa yazılır.
*         7
        /   \
       5     8
     /   \    \
    1       6   9
  /  \     
 0    3   
       \
        4
- 2 sayısı 7,5'ten küçük, 1'den büyük ama 3'ten küçük olduğu için 3'ün soluna yazılır.
*         7
        /   \
       5     8
     /   \    \
    1       6   9
  /  \     
 0    3   
     /  \
    2    4
                  
