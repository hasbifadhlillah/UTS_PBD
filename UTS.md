# UTS_PBD_195410234_FADHLILLAH HASBI ILYAS
UTS

1. Cari dan sebutkan 3 DBMS yang bisa digunakan untuk mengelola big data
   a. MYSQL
   b. Oracle
   c. Microsoft SQL SERVER
   
2. Carilah contoh masalah big data yang bisa dikelola menggunakan salah satu DBMS tersebut, jelaskan mulai dari instalasi sampai CRUD untuk data menggunakan DBMS tersebut.

masalah yang dikelola dengan database mMysql ini adalah penyewaan lapangan basket;

langkah menginstal MYSQL melalui xampp
1) download xamp pada https://www.apachefriends.org/
2) kemudian setelah download install xampp nya
3) langkkah menginstall nya cukup mengikuti aturan bawaan kemudian klik next sampai tahap akhir finish
4) setelah xampp terinstal kemudian bukalah aplikasi xampp control panel
5) kemudian menjalankan apache dan Mysqlnya
6) setelah itu untuk mengecek apakah berhasil di install dengan membuka browser dan mengetikan localhost pada browser

CRUD pada Mysql
1) pertama membuat database pada MySQL dengan perintah
   - create database lapangan;
   
2) kemudian perintah ini untuk menggunakan database yang telah dibuah
   - use lapangan;
   
3) kemudian untuk create tabel sewa dengan perintah
   CREATE TABLE `sewa` (
  `id` int(11) NOT NULL auto_increment,
  `name` varchar(100),
  `mobile` varchar(15),
  `alamat` varchar(50),
  `tanggal` date,
  `jam` time,
  `lama` varchar(5),
  PRIMARY KEY  (`id`)
  );   
  
4) kemudian menginput data dengan perintah
   INSERT INTO sewa VALUES ('001','Genji',2,' 08123456','Janti',now(), '13.00','2 jam');
   
5) kemudian setelah input data melihat data yang telah diinput;
   select * FROM sewa;
   
6) mengupdate data yang telah diinput
   UPDATE sewa SET mobile ='0812345678'
   WHERE name='Genji';
   
   perintah diatas mengupdate nomor telfon 
   
7) menghapus data pada padabase dengan perintah
   DELETE from sewa WHERE id = '001';
   diatas merupakan perintah menghapus data  melalui idnya sehingga id yang tertera datanya akan terhapus dari tabel
   
   untuk menghapus seluruh data pada tabel menggunakan perintah
   DELETE from sewa;
