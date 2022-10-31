# Insertion Sort Project
------------------------
[22,27,16,2,18,6]-> Insertion Sort

## 1. Yukarıda Verilen Dizinin Sort Türüne Göre Aşamalrını Yazınız
-------------------------
Insertion sort, dizinin üzerinde ilerleyerek bulunduğu haneyi ve bir öncekini karşılaştırır eğer bulunduğu hane bir öncekinden küçükse yer değiştirir ve bunu küçükten büyüğe bütün diziyi sıralayana kadar devam eder.

İlk sayı (22) sıralı olduğu için işlem yapılmaz.

[1.ADIM] [22,27,16,2,18,6]

(27) ve 22 karşılaştırılır. 22, 27'den küçük olduğu için değişiklik yapılmaz.

[2.ADIM] [22,27,16,2,18,6]

(16) ve 27 karşılaştırılır. 16, 27'den küçük olduğu için iki sayı yer değiştirir.Daha sonra 16 yeni konumunda 22 ile da karşılaştırılır ve 22'den de küçük olduğu için 22 ile de yer değiştirir.

[3.ADIM] [22,16,27,2,18,6]-> [16,22,27,2,18,6]

(2) ile bir önceki sayı (27) kıyaslar. 2, 27'den küçüktür. 2 ile 27 yer değiştirir. Daha sonra 2 ile 22'yi de kıyaslar. 2, 22'den küçüktür. 2 ile 22 yer değiştirir. Daha sonra tekrar 2 ile 16'yı kıyaslar. 2 16'dan küçüktür. 2 ile 16 da yer değiştirir.

[4.ADIM] [16,22,2,27,18,6]-> [16,2,22,27,18,6]-> [2,16,22,27,18,6]

(18) ile 27'yi kıyaslar. 18, 27'den küçüktür. 18 ile 27 yer değiştirir. Daha sonra tekrar 18 ile 22'yi kıyaslar. 18, 22'den küçüktür. 18 ile 22 yer değiştirir. Daha sonra tekrar 18 ile 16'yı kıyaslar. 18, 16'dan büyüktür. Değişiklik yapılmaz.

[5.ADIM] [2,16,22,18,27,6]->[2,16,18,22,27,6]

(6) ile 27'yi kıyaslar. 6, 27'den küçüktür. 6 ile 27 yer değiştirir. Daha sonra tekrar 6 ile 22'yi kıyaslar. 6, 22'den küçüktür. 6 ile 22 yer değiştirir. Daha sonra tekrar 6 ile 18'i kıyaslar. 6, 18'den küçüktür. 6 ile 18 yer değiştirir. Daha sonra tekrar 6 ile 16'yı kıyaslar. 6, 16'dan küçüktür. 6 ile 16 yer değiştirir. Daha sonra tekrar 6 ile 2'yi kıyaslar. 2, 6'dan küçüktür. Değişiklik yapılmaz.

[6.ADIM] [2,16,18,22,6,27]->[2,16,18,6,22,27]->[2,16,6,18,22,27]->[2,6,16,18,22,27]

## 2. Big - O Gösterimini yazınız
-----------------------------------

O(n^2)

## 3. Time Complexity
---------------------

* Worst Case: Aradığımız sayının sonda olması

  Tam ters verilmiş dizi, bu durumda dizinin her elemanı bir öncekinden küçük olacaktır. Bu yüzden 1. için döngü 0, 2. için geriye doğru 1, 3. için geriye doğru 2. Diğer elemanlar için 3,4,5,6 .....n kadar geriye doğru hareket yapacaktır.Yani 0+1+2+3....n-1 =[n*(n-1)/2]-> O n^2

* Average Case: Aradığımız sayının ortada olması

  n -> n/2 -> n/4  -> 2^x=n -> x=logn -> O (logn)

* Aradığımız sayının her durumda ilk sırada olması

  Tam sıralı dizi, n kadar sayının üzerinden birer defa geçer ve hiçbirini geriye doğru ilerletme gereği olmadığından tek geçişle kalır. -> O (n)

## 4. Dizi Sıralandıktan Sonra 18 Hangi Case Kapsamına Girer? Yazınız
-------------------------

Dizinin ortrasında olduğu için Average Case kapsamına girer.



## 2. [7,3,5,8,2,9,4,15,6] Dizisinin Insertion Sort'a göre İlk 4 Adımını Yazınız

[1.ADIM] [7,3,5,8,2,9,4,15,6]

[2.ADIM] [3,7,5,8,2,9,4,15,6]

[3.ADIM] [3,5,7,8,2,9,4,15,6]

[4.ADIM] [3,5,7,8,2,9,4,15,6]

[Patika.dev](https://www.patika.dev/tr)