`[22, 27, 16, 2, 18, 6]` -> Insertion Sort

Yukarı verilen dizinin sort türüne göre aşamalarını yazınız.

Big-O gösterimini yazınız.

Time Complexity: Dizi sıralandıktan sonra 18 sayısı aşağıdaki case'lerden hangisinin kapsamına girer? Yazınız

- Average case: Aradığımız sayının ortada olması
- Worst case: Aradığımız sayının sonda olması
- Best case: Aradığımız sayının dizinin en başında olması.

`[7, 3, 5, 8, 2, 9, 4, 15, 6]` dizisinin Selection Sort'a göre ilk 4 adımını yazınız.

---
1. Baslangic elemani dizinin 2. elemani secilir. [22, **27**, 16, 2, 18, 6]
2. 27 ile 22 kiyas edilir. 27 > 22 oldugundan 3. elemana bakilir.
3. 16 < 27 ve 16 < 22 oldugundan en basa alinir. [16, 22, 27, 2, 18, 6]
4. 4'uncu elemana geldiginde bir oncekilerden kucuk oldugu icin en basa alinir. [2, 16, 22, 27, 18, 6]
5. Bakilacak indis 5'tir ve burada bulunan eleman 18 dir. 18 solundaki 2, 16, 22, 27 ile kontrol edilir ve olmasi gereken yere gelir. [2, 16, 18, 22, 27, 6]
6. Son adimda altinci indisdeki eleman diger elemanlarla kontrol edilir ve yerini alir. 
Dizinin son hali `[2, 6, 16, 18, 22, 27]` olur.

Big-O -> O( n<sup>2</sup> )

Dizi siralandiginda 18 sayisi ortaya yakin oldugundan Average case durumunda olur.

---

`[7, 3, 5, 8, 2, 9, 4, 15, 6]` -> Selection Sort
1. Birinci adim
    - Dizide ilk konum icin 8 indisi tamamiyla dolanir. 7'nin bulundugu konum en dusuk degere sahip olan 2 ile degistirilir. [**7**, 3, 5, 8, 2, 9, 4, 15, 6]
    - 2 ile 7'nin yerleri degistirilmis oldu. [**2**, 3, 5, 8, 7, 9, 4, 15, 6]
2. Ikinci adim
    - 3'u noldugu 1. indis dizinin geri kalanini sirali sekilde kontol eder. 3 digerlerinden kucuk oldugundan yeri degismez ve diger indise bakilir. [2, **3**, 5, 8, 7, 9, 4, 15, 6]
3. Ucuncu adim
    - 2'nci indiste bulunan 5 geri kalan indislerle karsilastirilir ve 6. indiste bulunan 4 ile yer degistirir. [2, 3, **4**, 8, 7, 9, **5**, 15, 6] 
4. Dorduncu adim
    - 8'in diger elemanlarla karsilastirmasi yapilir ve 6. indisteki 5 degeri ile yeri degisir. [2, 3, 4, **5**, 7, 9, **8**, 15, 6]
5. ...