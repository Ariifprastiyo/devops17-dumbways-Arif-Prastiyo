# 1. Perbandingan antara Monolith & Microservices
- Arsitektur Microservices
Arsitektur microservices adalah model arsitektur aplikasi yang memisahkan aplikasi menjadi beberapa komponen yang independen yang dapat di-deploy dan diubah tanpa mempengaruhi komponen lainnya. 


- Arsitektur Monolitik
Arsitektur monolitik adalah cara pembuatan sistem yang menempatkan semua fungsi dan fitur dalam satu aplikasi tunggal yang besar. 


Perbandingan Arsitektur Monolitik dan Microservices
Arsitektur monolitik dan microservices adalah dua model arsitektur aplikasi yang berbeda yang memiliki kelebihan dan kekurangan masing-masing. Secara keseluruhan, arsitektur microservices lebih kompleks dibandingkan arsitektur monolitik, tetapi memberikan fleksibilitas dan skalabilitas yang lebih baik dalam pengembangan dan deployment aplikasi.

Arsitektur monolitik menempatkan semua komponen aplikasi dalam satu proyek atau satu kontainer. Ini membuat aplikasi lebih sederhana dan mudah diatur, serta memudahkan proses pengembangan dan deployment. Namun, karena semua komponen aplikasi terpisah dalam satu unit yang sederhana, ini dapat menyebabkan masalah skalabilitas dan fleksibilitas dalam jangka panjang.

Arsitektur microservices, di sisi lain, memisahkan aplikasi menjadi beberapa komponen yang independen yang dapat di-deploy dan diubah tanpa mempengaruhi komponen lainnya. Ini memungkinkan para pengembang untuk mengelola dan mem-deploy setiap microservice secara independen, serta mengelola skala dan performa setiap microservice dengan lebih baik. Namun, karena aplikasi dibagi menjadi beberapa microservices yang independen, ini dapat menjadi lebih kompleks dan rumit untuk dikembangkan dan di-deploy dibandingkan arsitektur monolitik.

---
# 2. Deploy Aplikasi wayshub-frontend (NodeJS)

1. Sebelum menginstal Nodes js jangan lupa ketik perintah 'sudo apt update'

    ![Alt text](img/Nodejs/1.png)

2. Selanjutnya install engine yang digunakan node js terlebih dahulu dengan mengetik 'curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.38.0/install.sh | bash'

    ![Alt text](img/Nodejs/2.png)

3. Setelah instal enginya kemudian ketik ’exec bash’ untuk memulai perintah baru

    ![Alt text](img/Nodejs/3.png)

4. Selanjutnya instal NVM nya dengan ketik 'nvm install 16'

    ![Alt text](img/Nodejs/4.png)

5. Setelah selesai instal cek nvm nya sudah benar belum dengan mengetik 'nvm use 16'

    ![Alt text](img/Nodejs/5.png)

6. Cek juga nodejs nya dengan perintah 'node -v' dan 'npm -v'

    ![Alt text](img/Nodejs/6.png)
    [Alt text](img/Nodejs/7.png)

7. Selanjutnya bikin file baru dengan nama package.json, package.json ini berisikan isi informasi dari aplikasi yang akan kita buat. Perintahnya 'npm init -y'
    
    ![Alt text](img/Nodejs/8.png)

8. Selanjutnya kita akan menginstall Express JS. Express JS  dengan mengetik 'npm install express –save'

    ![Alt text](img/Nodejs/9.png)

9. Selanjutnya bikin file yang berisi source code untuk menampilkan di tulisan Hello World! di web. Ketik perintah 'nano index.js'
    
    ![Alt text](img/Nodejs/10.png)

10. Tulis source code seperti gambar dibawah ini, setelah selesai tekan tombol CTRL + X lalu tombol y selanjutnya tombol enter.
    
    ![Alt text](img/Nodejs/11.png)

11. Setelah selesai ketik 'node index.js' perintah ini untuk mengetahui port mana yang digunakan 
    
    ![Alt text](img/Nodejs/Screenshot%202023-06-08%20114135.png)

12. Setelah mengetahui port mana yang digunakan coba masukan di search engine dengan ip_user@:3000
    
    ![Alt text](img/Nodejs/12.png)

13. Selanjutnya kita copy paste link github 'https://github.com/dumbwaysdev/wayshub-frontend' copy link ke terminal.

    ![Alt text](img/Nodejs/13.png)

14. Selanjutnya coba lihat filenya sudah tersedia atau belum ke dalam server kita dengan menegetik ‘ls’
    
    ![Alt text](img/Nodejs/14.png)

15. Masuk kedalam directory dengan mengetik 'cd wayshub-frontend/'

    ![Alt text](img/Nodejs/15.png)

16. Setelah masuk lihat isi directory nya dengan perintah 'ls'
    
    ![Alt text](img/Nodejs/16.png)

17. Setelah itu kita lihat terlebih dahulu isi file README.md nya dengan perintah 'cat README.md'

    ![Alt text](img/Nodejs/17.png)

18. Kita juga lihat isi file di package.json sudah ada file atas nama wayshubnya dengan perintah 'cat package.json'
    
    ![Alt text](img/Nodejs/21.png)

19. Setelah ada file package.json atas nama wayshubnya kita instal npmnya dengan perintah 'npm install'
    
    ![Alt text](img/Nodejs/18.png)

20. Setelah selesai instal npmnya kemudia nyalakan nmp nya dengan perintah 'npm start'
    
    ![Alt text](img/Nodejs/22.png)

21. Setelah  selesai muncul gambar yang ada di bawah ini
    
    ![Alt text](img/Nodejs/24.png)

22.Kemudia kita masuk ke web lagi jalankan perintah ip_user:3000 kembali
    
    ![Alt text](img/Nodejs/25.png)

---
# Deploy Pyhton3

1.	pertama ketikan sudo apt update terlebih dahulu untuk update system yang ada di server ubuntu
    
    ![Alt text](img/python3/1.png)

2. Buat folder tempat python3 nantinya dengan cara mengetik perintah 'mkdir namafolder'
3. masuk kembali kefolder yang kita buat dengan perintah 'cd namafolder'

4. selanjutnya ketik perintah 'python3 -v' untuk instal pythonnya

    ![Alt text](img/python3/2.png)

5.	Sekarang kita install package manager dari python3, dengan perintah 'sudo apt install python3-pip'. pip digunakan untuk menginstal flask
    
    ![Alt text](img/python3/5.png)

6.	Selanjutnya kita instal framework pythonnya dengan perintah ‘pip install flask’
    
    ![Alt text](img/python3/6.png)

7.	selanjutnya bikin file yang berisikan source code dengan perintah ‘nano index.py’
    
    ![Alt text](img/python3/Screenshot%202023-06-08%20124813.png)

8.	Masukan source codenya dan tambahkan bagian app.run(host='0.0.0.0.0') lalu tekan CTRL + K tekan Y dan tekan enter.
    
    ![Alt text](img/python3/7.png)

9.	Selanjutnya ketik ’python3 index.py’ untuk mengetahui dimana port yang digunakan 
    
    ![Alt text](img/python3/Screenshot%202023-06-08%20125126.png)

10.	buka search engine dan masukan ip_user:5000
    
    ![Alt text](img/python3/8.png)

---
# Deploy Golang

1.	Jalanakn perintah ‘sudo apt update’ terlebih dahulu.
2.	buat folder directoryna dengan perintah ‘ mkdir namafolder’
    
    ![Alt text](img/Golang/1.png)

3.	Masuk ke folder directory yang kita bikin tadi dengan perintah ‘ cd namafolder’
    
    ![Alt text](img/Golang/2.png)

4.	Masukan perintah ‘wget https://golang.org/dl/go1.16.5.linux-amd64.tar.gz && sudo su’ untuk menginstal enginya.
    
    ![Alt text](img/Golang/3.png)

5.	Ketik perintah ‘rm -rf /usr/local/go && tar -C /usr/local -xzf go1.16.5.linux-amd64.tar.gz && exit’ dibagian root@arf
    
    ![Alt text](img/Golang/5.png)

6.	Kemudian keluar terlebih dahulu dari folder dengan perintah ‘cd’
    
    ![Alt text](img/Golang/7.png)

7.	Kemudian masukan path go nya ketik perintah ‘sudo nano .bashrc’
    
    ![Alt text](img/Golang/8.png)

8.	Masukan source code ‘export PATH=$PATH:/usr/local/go/bin’ dibagian bawah sendiri lalu CTRL+X klik Y dan lalu enter
    
    ![Alt text](img/Golang/6.png)

9.	Selanjutnya ketik perintah go version untuk melihat versinya

    ![Alt text](img/Golang/10.png)

10. Masukan perintah 'nano index.go' diterminal, untuk membuat isi file

11.	Masukan source code dan tulisan yang akan di munculkan
    
    ![Alt text](img/Golang/16.png)

12.	Masukan perintah ‘go run index.go’ digunakan untuk menampilkan file yang sduafah di simpan index.go tadi.
    
    ![Alt text](img/Golang/11.png)

13.	Kemudian ketik ‘go build index.go’ untuk ngebuild filenya
    
    ![Alt text](img/Golang/12.png)
 
14.	Selanjutnya ketik ‘ls’ untuk melihat list directory yang tesimpan didalam folder
    
    ![Alt text](img/Golang/13.png)

15.	Selanjutnya ketik ‘./index’ untuk menjalankan aplikasi.
    
    ![Alt text](img/Golang/15.png)