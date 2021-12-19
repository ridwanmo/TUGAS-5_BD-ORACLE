# TUGAS-5_BD-ORACLE
 
 # 1. Membuat Koneksi Oracle Menggunakan PHP

<?php
$user="ridwan_123";
$pass="123";
$database="LOCALHOST/XE";

$con = oci_connect($user, $pass, $database);
if($con){
	echo "";

}
else{ 
	$err = oci_error();
echo "Gagal". $err['text'];
}
?>
<img width="960" alt="koneksi 2" src="https://user-images.githubusercontent.com/46704219/146666548-d7305c3e-992a-423f-b551-10cd6ec1f330.png">

# 2. membuat view
 
 create or replace view total_barang as select * from pembeli where total_barang = '10';
 
 create or replace view total_bayar as select * from transaksi where total_bayar = '7000';
 
 
 <img width="388" alt="total barang" src="https://user-images.githubusercontent.com/46704219/146666632-279c4799-87e5-49a9-991f-62d908ced56c.png">
<img width="307" alt="total bayar" src="https://user-images.githubusercontent.com/46704219/146666634-a83b7b6e-48f8-4340-bcfc-d9b163ef6237.png">

# 3. Membuat Halaman Home/Beranda

<img width="960" alt="dasbor" src="https://user-images.githubusercontent.com/46704219/146666723-dc2164e4-7d62-4058-a65a-8417e9655bd3.png">

# 4. Membuat Tabel Master

<img width="960" alt="pembeli" src="https://user-images.githubusercontent.com/46704219/146666745-066b9735-d2af-4a29-8db2-da039d1476f7.png">
<img width="960" alt="penjual" src="https://user-images.githubusercontent.com/46704219/146666750-6bbbfe68-2fc7-4a4e-ae31-2e28683137e6.png">
<img width="960" alt="transaksi" src="https://user-images.githubusercontent.com/46704219/146666755-ebdcddd9-2f86-408e-abe5-1abde4389a8b.png">
