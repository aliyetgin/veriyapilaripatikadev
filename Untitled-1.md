[22,27,16,2,18,6] -> Insertion Sort
Algoritma dizideki herhangi bir sayının kendinden önceki sıralardaki sayılardan küçük mü diye kontrol eder. 

1- ilk adımda 27 > 22 dizide bir değişiklik olmaz
2- 16 hem 27 hem de 22'den küçük olduğu için yeni dizi [16,22,27,2,18,6] olur.
3- 2 de kendinden önceki tüm sayılardan küçüktür -> [2, 16, 22, 27, 18, 6]
4- 18 için önce 27 ye bakılır 18 < 27 olduğu için onla yer değiştirir, sonra 22 ile karşılaştırılır 18 < 22 olduğu için onla da yer değiştirir en son 18 > 16 olduğu için daha fazla yer değiştirmez yeni dizi ->  [2, 16, 18, 22, 27, 6]
5- 6 2'ye kadar olan sayılarla karşılaştırılır ve onlardan küçük olduğu için yer değiştirir ama 2 den küçük olduğu için onla yer değiştirmez ->  [2, 6, 16, 18, 22, 27]

Average Case -> O(n²) Bir dizi içerisinde n kadar arama yapabiliriz ve bunu n kere yaptığımız için n²;
Worst Case -> O(n²) 
Best Case -> O(n) Dizi sıralı olursa sadece 1 kere küçük mü diye bakarız, bu işlemi n kere yaptığımız için time complexity n olur.

Dizi sıralandıktan sonra 18 sayısı Average case kapsamına girer

[7,3,5,8,2,9,4,15,6] dizisinin Selection Sort'a göre ilk 4 adımı

1- Dizideki en küçük eleman 2 olduğu için 7 ile yer değiştiriyoruz [2,3,5,8,7,9,4,15,6]
2- İkinci en küçük 3 yerinde olduğu için yer değiştirme yok [2,3,5,8,7,9,4,15,6]
3- 4 ile 5 in yerini değiştiriyoruz [2,3,4,8,7,9,5,15,6]
4- 5 ile 8 yer değiştirir [2,3,4,5,7,9,8,15,6]