# CODING-CHALLANGE
Coding Challange Software Enginner

# JUDUL PROYEK
Piramida Fibonacci

# SCRIPT & PENJELASAN
### Script :

```php
<?php
function print_deret_fibonacci($jumlah)
{
  $angka_sebelumnya=0;
  $angka_sekarang=1;
  
  $hasil = "$angka_sekarang";
  for ($i=0; $i<$jumlah-1; $i++)
  {
    $output = $angka_sekarang + $angka_sebelumnya;
    
    $hasil = $hasil." $output";
  
    $angka_sebelumnya = $angka_sekarang;
    $angka_sekarang = $output;
  }
  return $hasil;
}

function piramida_fibonacci($tingkat){
  for ($i=1; $i<$tingkat+1; $i++)
  {
    echo print_deret_fibonacci($i);
    echo "<br>";
  }
}

piramida_fibonacci(8);

?>
```

### Penjelasan :

```php
$hasil = "$angka_sekarang";
```
Fungsinya agar $hasil menampilkan $angka_sekarang setiap sesudah pengulangan<br>

```php
for ($i=0; $i<$jumlah-1; $i++)
  {
    $output = $angka_sekarang + $angka_sebelumnya;
```
Untuk menghitung angka fibonacci<br>

```php
$hasil = $hasil." $output";
```
Agar hasilnya($output) ditambahkan ke string $hasil<br>

```php
$angka_sebelumnya = $angka_sekarang;
$angka_sekarang = $output;
```
Nilai yang di siapkan untuk perhitungan berikutnya<br>

```php
function piramida_fibonacci($tingkat){
  for ($i=1; $i<$tingkat+1; $i++)
  {
    echo print_deret_fibonacci($i);
    echo "<br>";
  }
}
```
Proses pengulangan untuk membentuk sebuah piramida<br>

```php
piramida_fibonacci(8);
```
Untuk menentukan berapa jumlah baris yang di perlukan<br>
