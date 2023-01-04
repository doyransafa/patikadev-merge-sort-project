# patikadev-merge-sort-project
Patika.dev Veri Yapıları ve Algoritmalar Dersi - Merge Sort Projesi

[16,21,11,8,12,22] -> Merge Sort

Merge Sort işleminde tüm itemler tekil halde kalana kadar ayrıştırılır ve birleştirilerek sıralanır.

**1. adım:**
> [16,21,11] - [8,12,22]

**2. adım:**
> [16] - [21,11] - [8] - [12,22]

**3. adım:**
> [16] - [21] - [11] - [8] - [12] - [22]

**4. adım:** 
- 16 ve 21 kıyaslanır ve küçük sola, büyük sağa yazılır. Aynı işlem 11 ve 8 ve 12 ve 22 için de yapılır.
> [16,21] - [8,11] - [12,22]

**5. adım:** 
- İlk iki grubun ilk itemleri kıyaslanır ve küçük olan bir sonraki adımda ilk sıraya yazılır. 8 < 16
- 8 ilk sıraya yazıldıktan sonra soldaki grubun ilk sayısı ve sağdaki grubun kalan sayısı kıyaslanır ve küçük olan yazılır. 11 < 16
- Soldaki grubun tamamı kaldığı ve zaten sıralanmış olduğu için direkt olarak yazılır.
> [8,11,16,21] - [12,22]

**6. adım:** 
- İlk iki grubun ilk itemleri kıyaslanır ve küçük olan bir sonraki adımda ilk sıraya yazılır. 8 < 12
- 8 ilk sıraya yazıldıktan sonra soldaki grubun ikinci sayısı ve sağdaki grubun ilk sayısı kıyaslanır ve küçük olan yazılır. 11 < 12
- 11 ikinci sıraya yazıldıktan sonra soldaki grubun üçüncü sayısı ve sağdaki grubun ilk sayısı kıyaslanır ve küçük olan yazılır. 12 < 16
- 12 üçüncü sıraya yazıldıktan sonra soldaki grubun üçüncü sayısı ve sağdaki grubun ikinci sayısı kıyaslanır ve küçük olan yazılır. 16 < 22
- 16 dördüncü sıraya yazıldıktan sonra soldaki grubun dördüncü sayısı ve sağdaki grubun ikinci sayısı kıyaslanır ve küçük olan yazılır. 21 < 22
- 21 beşinci sıraya yazıldıktan kalan son sayı 22 altıncı sıraya yazılır.
> [8,11,12,16,21,22]

# Özet
> [16,21,11] - [8,12,22]

> [16] - [21,11] - [8] - [12,22]

> [16] - [21] - [11] - [8] - [12] - [22]

> [16,21] - [8,11] - [12,22]

> [8,11,16,21] - [12,22]

> [8,11,12,16,21,22]

# Big O Notation

O(n log n)
