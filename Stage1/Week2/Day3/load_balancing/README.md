# 1. Buat 2 VM untuk penggunaan :
# - aplikasi Dumbflix
# - nginx & Dumbflix secara bersamaan
# 2. Gunakan konfigurasi Load Balancing, lalu tes apakah bekerja dengan baik atau tidak
---
Jawaban :

1. Disini saya memakai 2 Vm yang satu dengan ip `192.168.1.124`

    ![Alt text](img/3.png)

2. Tambahkan ip yang digunakan dengan masuk ke `/etc/hosts`

     ![Alt text](img/4.png)

3. Masuk file hosts di dalam pc kita dan tambahkan ipserver dan somain kita

    ![Alt text](img/5.png)

4. Cek juga nginx nya dengan `nginx -v` karena server 2 ini saya tidak pakai nginx maka akan muncul seperti dibawah ini. nginx hanya diinstall di server 1.

    ![Alt text](img/6.png)

5. Masuk kedalam folder dumbflix-frontend dan install npm

     ![Alt text](img/2.png)

6. Masukan run build untuk membundle Aplikasinya dengan perintah `npm run build`

    ![Alt text](img/7.png)

7. Install pm2 nya

     ![Alt text](img/8.png)   

8. Install `sudo snap install serve` dan juga install juga `npm install -g serve`

    ![Alt text](img/9.png)

9. Jalankan pm2 nyadengan perintah `pm2 serve build`

    ![Alt text](img/10.png)
    
    ![Alt text](img/11.png)

10. Jalankan ip_server dan port 8080 di chrome

    ![Alt text](img/13.png)

11. Dengan pengaturan nginx di server 1 kita tadi maka tidak masalah server 1 kita mati aplikasi masih tetap bisa berjalan di dengan domain yang sama.

    ![Alt text](img/12.png)

    ![Alt text](img/15.png)

    ![Alt text](img/14.png)