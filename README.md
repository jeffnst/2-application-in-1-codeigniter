# 2in1
Membuat banyak aplikasi dengan 1 core framework codeigniter.

### PERSIAPAN
1. Download framework codeigniter dan ekstrak di folder kerjamu. Dalam contoh ini sudah disiapkan, dan diubah namanya menjadi dari `system/` menjadi `_system/` dan `application/` menjadi `_apps/` untuk mempermudah pengaturan isi folder.
2. Buat folder baru untuk apps bernama `home_app/` di root
3. Pindahkan semua file di folder `_apps/` ke folder `home_app/`
4. Pindahkan folder `home_app/` ke folder `_apps/`
5. Buat folder baru untuk url bernama `home/` di root
6. Salin file `index.php` ke folder `home/`
7. Lakukan langkah 2 - 6 jika ingin membuat apps lain, contoh : `_apps/blog_app/`

### MODIFIKASI FILE INDEX.PHP
Modifikasi file index.php di root :
```
$system_path = '_system';
$application_folder = '_apps/home_app';
```

Modifikasi file index.php di apps, contoh : `home/index.php` :
```
$system_path = '../_system';
$application_folder = '../_apps/home_app';
```

# Selesai