### :octocat:Syssaturn404 Repo:dizzy:
![Examples](https://github.com/syssaturn404/LINUX-Troubleshooting/blob/master/Apt/Configuration/contoh.png)
```
Error yang sering dijumpai masyarakat awam :
E: Unable to lock directory /var/cache/apt/archives/
E: Could not open lock file /var/cache/apt/archives/lock - open (13: Permission denied)
E: Unable to lock the download directory
```
```
Sebagian orang awam, disaat instalasi saya yakin ada pertanyaan yang timbul dengan masalah seperti diatas
- Apa ini..? Mengapa saya tidak melakukan apa - apa, tapi timbul seperti itu, saya jengkel sekali.
- Kenapa bisa begini, saya masih awam akan linux, jadi tidak mengerti apa yang dimaksud.
- etc.
Kenapa bisa seperti itu..? Dikarenakan kamu sedang melakukan proses instalasi / sedang membuka
manager, sedang kamu ingin membuka manager yang lain, maka dari itu otomatis 
manager depan mengunci / lock manager lain sebelum proses instalasi selesai
kamu tidak diizinkan untuk membuka manager lainnya.
Tetapi saya tidak membuka paket / manager apa - apa..?
Mengapa bisa seperti itu..? Bisa saja paket yang kamu install masih menginstal paket lainnya
Atau system tidak memperbolehkan user biasa masuk / harus menggunakan hak superuser, etc.
```
### HOW TO SOLVE PROBLEM ?
```
Cara mengatasinya adalah dengan kamu menghentikan semua proses. 
Bagaimana caranya..? Buka command prompt / CLI atau ketik bersamaan CTRL + ALT + T, jika menggunakan xfce.
Ketikan command / perintah dibawah :
root@kali:~# sudo su
[sudo] password for ***: (masukan passwd kamu)
root@kali:~# cd /var/lib/dpkg
root@kali:~# ls -la
Kamu bisa melihat file lock disini, ini yang membuat paket / manager lainnya terhenti
Cara agar manager bisa digunakan kembali adalah me-remove / hapus file tersebut, jika tidak ketemu file lock
coba ketikan command / perintah dibawah :
root@kali:~# locate lock-frontend 
/var/lib/dpkg/lock-frontend
kamu bisa melihat dimana directory lock tersimpan, lalu kamu masuk dan kembali ke directory sebelumnya
untuk melihat file lock
root@kali:~# cd /var/lib/dpkg/ && ls -la (tanpa lock-frontend)
-rw-r-----  1 root root       0 Jan 25 02:36 lock
-rw-r-----  1 root root       0 Jan 22 02:58 lock-frontend
Hapus file lock, kemudian jalankan ulang manager, ketikan command / perintah dibawah :
root@kali:~# sudo rm lock && sudo rm lock-frontend (kemudian jalankan ulang manager yang ingin kamu install / jalankan)

> Examples :
root@kali:~# sudo apt-get install neofetch -y && neofetch
Jika masih tida bisa jalankan command / peritah dibawah ini :
root@kali:~# sudo killall apt-get
root@kali:~# sudo rm /var/lib/apt/lists/lock && sudo rm /var/cache/apt/archives/lock && sudo rm /var/lib/dpkg/lock
root@kali:~# sudo dpkg --configure -a
```
![Examples](https://github.com/syssaturn404/LINUX-Troubleshooting/blob/master/Apt/Configuration/examples-done.png)
