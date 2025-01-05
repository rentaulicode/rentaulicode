# TodoList Sederhana dengan PHP &amp; MySQL + jQuery Ajax


### Fitur

1. Tambah TodoList
2. Tandai selesai TodoList
3. Arsipkan TodoList
4. Hapus TodoList
5. Tanpa reload menggunakan jquery + ajax 

### Instalasi
Untuk cara instalasi dan konfigurasi caranya sangat mudah

1. Kalian download atau clone repositori ini
2. Selanjutnya kalian bisa buka file `connection.php` 
3. Sesuaikan `db_host`, `db_user`, `db_pass` dan `db_name` sesuai konfigurasi web server kalian.
4. import `todo.sql` ke database 



=== Tugas Query DDL 

1. Pembuatan Tabel

CREATE TABLE `tasks` (
  `id` int(11) NOT NULL,
  `task` varchar(100) DEFAULT NULL,
  `description` varchar(255) DEFAULT NULL,
  `start` varchar(20) DEFAULT NULL,
  `finish` varchar(20) DEFAULT NULL,
  `is_finish` int(1) DEFAULT 0,
  `is_archive` int(1) DEFAULT 0
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4;


2. Pembuatan Index

ALTER TABLE `tasks`
  ADD PRIMARY KEY (`id`);

3. Mengatur Auto Increment Pada Tabel

ALTER TABLE `tasks`
  MODIFY `id` int(11) NOT NULL AUTO_INCREMENT, AUTO_INCREMENT=12;


== Fungsi Fungsi PHP yang berhubungan Dengan Database

- Connection.php
- index.php
- get_task.php
- restore.php
- save_task.php

