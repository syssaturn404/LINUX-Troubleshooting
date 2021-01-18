### :octocat:Software Center:dizzy:
![HelloWorld](https://github.com/syssaturn404/LINUX-Troubleshooting/blob/master/Apt/Screenshot%20from%202021-01-18%2005-08-51.png)

```
How to fix it, software center not data found ? Perhatikan gambar dibawah ini : 
```
![Syssaturn404](https://github.com/syssaturn404/LINUX-Troubleshooting/blob/master/Apt/ex.png)
```
Cara yang paling mudah untuk memperbaikinya adalah dengan menginstal beberapa package tambahan dari gnome
Ada banyak pilihan untuk manager perangkat lunak. 
Dua opsi yang sangat populer adalah Pusat Perangkat Lunak dan Manajer Paket Synaptic. 
Pusat Perangkat Lunak sangat sederhana dan merupakan aplikasi default pada beberapa distribusi seperti Ubuntu.
Synaptic adalah antarmuka GUI untuk APT, dan secara inheren lebih kuat daripada Pusat Perangkat Lunak. 
Belum lama ini, itu adalah aplikasi default di banyak sistem, 
tetapi tidak disukai karena kesederhanaan Pusat Perangkat Lunak.
Keduanya bekerja dengan sangat baik, dan Anda dapat menginstal mana saja yang Anda inginkan. 
Petunjuk untuk memasang keduanya disertakan di bawah ini.

> Install Software Center
Buka terminal dan ketikan command seperti di bawah ini : 

root@kali:~# sudo apt update
root@kali:~# sudo apt install gnome-software

Setelah penginstalan selesai, Anda harus menggunakan vi atau editor teks favorit Anda untuk 
mengedit file /etc/apt/sources.list agar aplikasi dapat berfungsi. 
Tambahkan baris berikut ke file.

root@kali:~# sudo vi /etc/apt/sources.list

deb http://kali.download/kali/ kali-rolling main non-free contrib
deb http://ftp.debian.org/debian stable main contrib non-free
deb http://http.kali.org/kali kali-rolling main non-free contrib
deb http://http.kali.org/kali kali-last-snapshot main non-free contrib
deb http://http.kali.org/kali kali-experimental main non-free contrib
deb-src http://http.kali.org/kali kali-rolling main non-free contrib

lalu lakukan update package dengan menjalankan perintah sudo apt-get update dari terminal.
Untuk membuka Pusat Perangkat Lunak, jalankan perintah gnome-software dari terminal. 
Sekarang Anda dapat mencari dan menginstal aplikasi baru, atau menghapus aplikasi saat ini dari sistem Anda.
```
![Examples-Software-Center](https://github.com/syssaturn404/LINUX-Troubleshooting/blob/master/Apt/Screenshot%20from%202021-01-18%2018-06-50.png)
```
> Install Synaptic Package Manager
Buka terminal, dan ketikan command / perintah berikut ini : 
root@kali:~# apt-get update
root@kali:~# apt install synaptic -y
root@kali:~# synaptic
Anda sekarang bisa menginstall atau menghapus aplikasi saat ini.
```
![Examples-Synaptic](https://github.com/syssaturn404/LINUX-Troubleshooting/blob/master/Apt/Screenshot%20from%202021-01-18%2018-16-03.png)
