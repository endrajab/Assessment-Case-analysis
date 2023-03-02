# Assessment-Case-analysis

## Requirement:
Tim QA sedang menguji sebuah aplikasi untuk sebuah mesin kopi. Mesin tersebut dapat membuat berbagai jenis kopi 

berdasarkan ukuran kopi, susu, gula dan sirup. Kriteria sebagai berikut:

1. Suhu kopi harus sama dengan 78 Derajat
2. Ukuran kopi (Kecil,Sedang,Besar)
3. Gula (tanpa gula, 1 sendok, 2 sendok, 3 sendok, 4 sendok)
4. Susu (Pakai atau Tidak Pakai)
5. Sirup (tidak pakai sirup, Karamel, Hazelnut, Vanila)
6. Sirup tidak bisa ditambahkan jika gula yang dimasukan lebih dari 3 sendok

## Task:
Berdasarkan Requirement di atas, strategi Black box Testing yang bisa digunakan adalah adalah **Decision Testing Table**.

Dikarenakan kriteria input yang banyak sehingga akan menimbulkan kombinasi input yang banyak juga sehingga dengan menggunakan decision testing table, kita bisa melihat dengan jelas semua kemungkinan kombinasi input yang bisa dilakukan pengetesan.
Kombinasi input yang bisa dihasilkan adalah 3x5x2x4 = 120
- 3 jenis kopi
- 5 kombinasi input gula
- 2 kombinasi susu
- 4 kombinasi sirup

Berikut table decision yang dapat dibuat dengan requirement diatas

|Condition |1|2|3|4|5|6|7|8|9|10|11|12|
|----------|-|-|-|-|-|-|-|-|-|-|-|-|
|Kopi|Kecil|Sedang|Besar|Kecil|Sedang|Besar|Kecil|Sedang|Besar|Kecil|Sedang|Besar|
|Gula|No Gula|No Gula|No Gula|No Gula|No Gula|No Gula|No Gula|No Gula|No Gula|No Gula|No Gula|No Gula|
|Susu|No|No|No|No|No|No|No|No|No|No|No|No|
|Sirup|No|No|No|Karamel|Karamel|Karamel|Hazelnut|Hazelnut|Hazelnut|Vanila|Vanila|Vanila|

|Condition |13|14|15|16|17|18|19|20|21|22|23|24|
|----------|-|-|-|-|-|-|-|-|-|-|-|-|
|Kopi|Kecil|Sedang|Besar|Kecil|Sedang|Besar|Kecil|Sedang|Besar|Kecil|Sedang|Besar|
|Gula|No Gula|No Gula|No Gula|No Gula|No Gula|No Gula|No Gula|No Gula|No Gula|No Gula|No Gula|No Gula|
|Susu|Yes|Yes|Yes|Yes|Yes|Yes|Yes|Yes|Yes|Yes|Yes|Yes|
|Sirup|No|No|No|Karamel|Karamel|Karamel|Hazelnut|Hazelnut|Hazelnut|Vanila|Vanila|Vanila|

|Condition |25|26|27|28|29|30|31|32|33|34|36|36|
|----------|-|-|-|-|-|-|-|-|-|-|-|-|
|Kopi|Kecil|Sedang|Besar|Kecil|Sedang|Besar|Kecil|Sedang|Besar|Kecil|Sedang|Besar|
|Gula|1 sendok|1 sendok|1 sendok|1 sendok|1 sendok|1 sendok|1 sendok|1 sendok|1 sendok|1 sendok|1 sendok|1 sendok|
|Susu|Yes|Yes|Yes|Yes|Yes|Yes|Yes|Yes|Yes|Yes|Yes|Yes|
|Sirup|No|No|No|Karamel|Karamel|Karamel|Hazelnut|Hazelnut|Hazelnut|Vanila|Vanila|Vanila|

|Condition |37|38|39|40|41|42|43|44|45|46|47|48|
|----------|-|-|-|-|-|-|-|-|-|-|-|-|
|Kopi|Kecil|Sedang|Besar|Kecil|Sedang|Besar|Kecil|Sedang|Besar|Kecil|Sedang|Besar|
|Gula|2 sendok|2 sendok|2 sendok|2 sendok|2 sendok|2 sendok|2 sendok|2 sendok|2 sendok|2 sendok|2 sendok|2 sendok|
|Susu|Yes|Yes|Yes|Yes|Yes|Yes|Yes|Yes|Yes|Yes|Yes|Yes|
|Sirup|No|No|No|Karamel|Karamel|Karamel|Hazelnut|Hazelnut|Hazelnut|Vanila|Vanila|Vanila|

|Condition |49|50|51|52|53|54|55|56|57|58|59|60|
|----------|-|-|-|-|-|-|-|-|-|-|-|-|
|Kopi|Kecil|Sedang|Besar|Kecil|Sedang|Besar|Kecil|Sedang|Besar|Kecil|Sedang|Besar|
|Gula|3 sendok|3 sendok|3 sendok|3 sendok|3 sendok|3 sendok|3 sendok|3 sendok|3 sendok|3 sendok|3 sendok|3 sendok|
|Susu|Yes|Yes|Yes|Yes|Yes|Yes|Yes|Yes|Yes|Yes|Yes|Yes|
|Sirup|No|No|No|Karamel|Karamel|Karamel|Hazelnut|Hazelnut|Hazelnut|Vanila|Vanila|Vanila|

|Condition |61|62|63|64|65|66|67|68|69|70|71|72|
|----------|-|-|-|-|-|-|-|-|-|-|-|-|
|Kopi|Kecil|Sedang|Besar|Kecil|Sedang|Besar|Kecil|Sedang|Besar|Kecil|Sedang|Besar|
|Gula|4 sendok|4 sendok|4 sendok|4 sendok|4 sendok|4 sendok|4 sendok|4 sendok|4 sendok|4 sendok|4 sendok|4 sendok|
|Susu|Yes|Yes|Yes|Yes|Yes|Yes|Yes|Yes|Yes|Yes|Yes|Yes|
|Sirup|No|No|No|Karamel|Karamel|Karamel|Hazelnut|Hazelnut|Hazelnut|Vanila|Vanila|Vanila|

|Condition |73|74|75|76|77|78|79|80|81|82|83|84|
|----------|-|-|-|-|-|-|-|-|-|-|-|-|
|Kopi|Kecil|Sedang|Besar|Kecil|Sedang|Besar|Kecil|Sedang|Besar|Kecil|Sedang|Besar|
|Gula|1 sendok|1 sendok|1 sendok|1 sendok|1 sendok|1 sendok|1 sendok|1 sendok|1 sendok|1 sendok|1 sendok|1 sendok|
|Susu|No|No|No|No|No|No|No|No|No|No|No|No|
|Sirup|No|No|No|Karamel|Karamel|Karamel|Hazelnut|Hazelnut|Hazelnut|Vanila|Vanila|Vanila|

|Condition |84|86|87|88|89|90|91|92|93|94|95|96|
|----------|-|-|-|-|-|-|-|-|-|-|-|-|
|Kopi|Kecil|Sedang|Besar|Kecil|Sedang|Besar|Kecil|Sedang|Besar|Kecil|Sedang|Besar|
|Gula|2 sendok|2 sendok|2 sendok|2 sendok|2 sendok|2 sendok|2 sendok|2 sendok|2 sendok|2 sendok|2 sendok|2 sendok|
|Susu|No|No|No|No|No|No|No|No|No|No|No|No|
|Sirup|No|No|No|Karamel|Karamel|Karamel|Hazelnut|Hazelnut|Hazelnut|Vanila|Vanila|Vanila|

|Condition |97|98|99|100|101|102|103|104|105|106|107|108|
|----------|-|-|-|-|-|-|-|-|-|-|-|-|
|Kopi|Kecil|Sedang|Besar|Kecil|Sedang|Besar|Kecil|Sedang|Besar|Kecil|Sedang|Besar|
|Gula|3 sendok|3 sendok|3 sendok|3 sendok|3 sendok|3 sendok|3 sendok|3 sendok|3 sendok|3 sendok|3 sendok|3 sendok|
|Susu|No|No|No|No|No|No|No|No|No|No|No|No|
|Sirup|No|No|No|Karamel|Karamel|Karamel|Hazelnut|Hazelnut|Hazelnut|Vanila|Vanila|Vanila|

|Condition |109|110|111|112|113|114|115|116|117|118|119|120|
|----------|-|-|-|-|-|-|-|-|-|-|-|-|
|Kopi|Kecil|Sedang|Besar|Kecil|Sedang|Besar|Kecil|Sedang|Besar|Kecil|Sedang|Besar|
|Gula|4 sendok|4 sendok|4 sendok|4 sendok|4 sendok|4 sendok|4 sendok|4 sendok|4 sendok|4 sendok|4 sendok|4 sendok|
|Susu|No|No|No|No|No|No|No|No|No|No|No|No|
|Sirup|No|No|No|Karamel|Karamel|Karamel|Hazelnut|Hazelnut|Hazelnut|Vanila|Vanila|Vanila|

## Test Cases
Kombinasi test cases yang bisa digunakan minimal sebanyak 120 test case, sesuai dengan tabel diatas.
Expected setiap case adalah suhu kopi harus sesuai yaitu 78 derajat

1. Buat kopi dengan ukuran kecil tanpa gula, tanpa susu, dan tanpa sirup
2. Buat kopi dengan ukuran sedang tanpa gula, tanpa susu, dan tanpa sirup
3. Buat kopi dengan ukuran besar tanpa gula, tanpa susu, dan tanpa sirup
4. Buat kopi dengan ukuran kecil tanpa gula, tanpa susu, dan  dengan sirup karamel
5. Buat kopi dengan ukuran sedang tanpa gula, tanpa susu, dan dengan sirup karamel

    .
    
    .
    
    .

<!-- -->
119.  Buat kopi dengan ukuran sedang dengan gula 4 sendok, tanpa susu, dan sirup vanila (pastikan tidak bisa input sirup)
120.  Buat kopi dengan ukuran besar dengan gula 4 sendok, tanpa susu, dan sirup vanila (pastikan tidak bisa input sirup)

More Negative Case

121. Buat kopi tanpa kopi (kopi tray kosong)

## Bug

1. Summary Bug: Suhu air kopi dibawah 70 derajat saat menggunakan gula, susu dan sirup.

    Step reproduce:
    - Buat kopi dengan menggunakan gula, susu dan sirup

    Actual result: suhu kopi dibawah 70 derajat

    Expected Result: suhu kopi harus sesuai yaitu 78 derajat

2. Summary bug: Dapat menambahkan sirup pada mesin kopi ketika memilih takaran gula 4 sendok

   Step reproduce:
    - Buat kopi dengan menggunakan takaran gula 4 senddok
    - Tambahkan sirup

    Actual result: Sirup dapat ditambahkan pada kopi dengan takaran gula 4 sendok

    Expected Result: Sirup tidak dapat ditambahkan ketika takaran gula 4 sendok