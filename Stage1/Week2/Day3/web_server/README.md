# 1. Instalasi nginx melalui apt
# 2. menjalankan aplikasi dumbflix menggunakan PM2
# 3. buatlah konfigurasi reverse proxy!
# (Gunakan 2 server untuk memenuhi challenge, tidak wajib)
--- 
Jawaban :

1. Pertama install nginx terlebih dahulu `sudo apt install nginx`

    ![Alt text](img/1.png)

2. Lihat nginx dengan perintah `nginx -v`

    ![Alt text](img/2.png)

3. Selanjutnya masuk ke folder `cd dumbflix-frontend` install npm `npm install` 

    ![Alt text](img/3.png)

4. Jalanakn npmnya dengan perintah `npm run build`

    ![Alt text](img/4.png)

5. Sebelum ke step berikutnya install pm2 dengan perintah `npm install -g pm2`

    ![Alt text](img/15.png)

6. ketik perintah `serve -s build` untuk mengathui command untuk menjalankan serve. ketik perintah `npm  snap install serve`  dan `npm install -g serve`

    ![Alt text](img/5.png)

7. ketik perintah `pm2 serve build` untuk menjalankan pm2 nya. disini aplikasi berjalan di port 8080.

    ![Alt text](img/6.png)

8. masuk ke crhome dan masukan ipserver dan port 8080.

    ![Alt text](img/7.png)

9. keluar dari folder dumbflix-frontend dan masuk ke folder nginx `cd /etc/nginx` buat folder dengan nama dumbways `mkdir dumbways` dan masuk ke foldernya dengan perintah `cd dumbways` dan buat file bernama my.reverse-proxy.conf `sudo nano my.reverse-proxy.conf`.

    ![Alt text](img/8.png)

10. masukan di bagian proxy "ipserver:8080" dan server name "dumbflix-namapanggilan.xyz".

    ![Alt text](img/10.png)

11. masukan ipserver:8080 dan nama domain kedalam hosts pc kita

    ![Alt text](img/11.png)

12. Keluar dulu dari folder dumbways `cd ..` dan bikin file baru `sudo nano nginx.conf`  masukan folder yang bernama dumbways dengan perintah `include /etc/nginx/dumbways/*;`

    ![Alt text](img/16.png) 

13. lihat file yang kita tambahkan dengan perintah `sudo nginx -t`

    ![Alt text](img/17.png)

14. Reload dan cek status nginx

    ![Alt text](img/18.png)

15. jalankan domain kita `dumbflix-arif.xyz` ke crhome dan kita sudah berhasil seting aplikasinya.

    ![Alt text](img/12.png)

16. untuk menjalankan load balancing kita akan mengatur my.reverse-proxy seperti pada gambar. kita akan melanjutkannya pada pembahasan load balancing dengan 2 vm.

    ![Alt text](img/14.png)