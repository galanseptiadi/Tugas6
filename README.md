# Tugas6
# Nama : Galan Septiadi

# Kelas : TI20D1

# NIM : 312010053

# Matkul: Sistem Basis Data

Masuk ke database nama_nim
![image](https://user-images.githubusercontent.com/101730390/171027946-246c70cb-2c77-47f7-a27d-0cbf213cef7d.png)


Lakukan proses backup dan recovery dengan sql dari database tugas seblumnya !
Backup

![image](https://user-images.githubusercontent.com/101730390/171028303-38ea4ddb-7c0f-4a05-85e1-d896df2e8807.png)


Jika proses backup berhasil maka akan muncul file backuppada direktori C:\xampp\mysql\data\nama database

![image](https://user-images.githubusercontent.com/101730390/171028600-9184ee8a-3e3e-4575-8891-af12946f4e6f.png)


Recovery

Data yang telah di-backup dapat dikembalikan kapan saja bila diperlukan. Sintaks SQL yang digunakan adalah LOAD DATA INFILE. Perintah yang dijalankan adalah

LOAD DATA INFILE ‘Nama_backup_file’ INTO TABLE nama_table ;

![image](https://user-images.githubusercontent.com/101730390/171032234-53047f64-a5e9-4d28-93c7-38ff3c0da19c.png)


Lakukan proses backup dan recovery dengan sqldump dari database tugas seblumnya !
![image](https://user-images.githubusercontent.com/101730390/171033191-fda55bfa-6fe0-4c48-a02e-a540e3b9fc6a.png)


![image](https://user-images.githubusercontent.com/101730390/171033287-652f3fa1-917d-4d10-bba7-1eb6f5420dce.png)
![image](https://user-images.githubusercontent.com/101730390/171033323-1ce885f9-29a6-4d7b-bcf9-c63a5e5754b0.png)


Tulisakan script cron job untuk melakukan backup otomatis setiap hari minggu jam 12 malam !
crontab –e

**12*7mysqldump -u root -p galan_312010053>galan_312010053_backup.sql
