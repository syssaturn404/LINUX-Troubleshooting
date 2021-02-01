### :octocat:Syssaturn404 Repo:dizzy:

![Examples](https://miro.medium.com/max/1200/1*ucJJzOQqul_g09vzOVUI4Q.jpeg)
```
Katakan anda sedang mengedit file di Linux dan saat menyimpannya 
malah muncul pesan error No space left on device.
padahal anda yakin masih banyak kapasitas harddisk yang tersisa. 
Masalah ini pernah saya alami karena mencopy file iso 
untuk bootable agar tidak corrupt.
Juga ada pertanyaan sekilas mengenai bagaimana mengatasi ini.
Faktor diatas adalah kurangnya penyimpanan / partisi penuh.
Caranya mudah, pahami dan cermati dengan seksama !
```
![Examples](https://i.stack.imgur.com/okaSG.png)
```
> Buka CLI / Command prompt anda / tekan CTRL + ALT +  T secara bersama

ketikan command / perintah dibawah ini :
> df -h (berfungsi untuk memeriksa penyimpanan tersisa / free space)
Lalu dihapus bagian mana yang memakan banyak ram. 
Atau bisa cek inodes anda
> df -i
Bisa dihapus jika memakan banyak ram.

Atau anda juga bisa mencari banyak dan besarnya jumlah file 
dengan command yang sudah saya racik ini : 
> sudo du -ahx / | sort -rh | head -10
Akan diurutkan berdasarkan ukuran foldernya
Jadi kita akan langsung tahu dimana saja yang patut dicurigai. 
Perintah ini saya batasi cuma 10, tapi bisa anda gantikan ke angka 
yang lebih besar dengan mengubah nilai parameter perintah head diatas.

> find / -xdev -type f -size +10M -exec du -sh {} ';' | sort -rh | head -n10
Command diatas untuk mengambil file berukuran 10MB
sama seperti diatas, jika ingin lebih besar, ganti nilai parameter (size)
lalu hapus, dan lihat sisa penyimpanan anda, lalu lakukan update package.
> sudo apt-get update
```
![Examples](https://github.com/syssaturn404/LINUX-Troubleshooting/blob/master/Apt/Configuration/Screenshot_2021-02-01_20-03-34.png)
