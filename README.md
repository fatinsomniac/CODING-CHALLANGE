# CODING-CHALLANGE
Coding Challange Software Enginner

# JUDUL PROYEK
Piramida Fibonacci

# SCRIPT & PENJELASAN
## Script :

```html
<?php
function print_deret_fibonacci($jumlah)
{
  $angka_sebelumnya=0;
  $angka_sekarang=1;
  
  $hasil = "$angka_sekarang"; // agar yang di tampilkan adalah angka_sekarang
  for ($i=0; $i<$jumlah-1; $i++)
  {
    $output = $angka_sekarang + $angka_sebelumnya; // hitung angka fibonacci
    
    $hasil = $hasil." $output"; // hasilnya($output) ditambahkan ke string $hasil
  
    //siapkan angka untuk perhitungan berikutnya
    $angka_sebelumnya = $angka_sekarang;
    $angka_sekarang = $output;
  }
  return $hasil;
}

//proses pengulangan untuk membentuk sebuah piramida
function piramida_fibonacci($tingkat){
  for ($i=1; $i<$tingkat+1; $i++)
  {
    echo print_deret_fibonacci($i);
    echo "<br>";
  }
}

//Untuk menentukan berapa jumlah baris yang di perlukan
piramida_fibonacci(8);

?>
```
