### :octocat:Syssaturn404 Repo:dizzy:

![Examples](https://3.bp.blogspot.com/-dOQVrNvr4AY/VuL_DgK0UfI/AAAAAAAAF9U/4jutGiSgEqkExplGYVGTvXaLsqqvGU8iQ/s320/P_20160311_233120_HDR.jpg)
```
Pasti pernah sebagian orang yang masih awam mengalami masalah seperti diatas saat
pertama menggunakan linux, saya mendapati beberapa pertanyaan tentang
Bagaimana cara mengatasi stuck dan tidak bisa masuk mode GUI
Itu sangat mengganggu bagi yang masih awam menggunakan linux.
Faktor tidak bisa masuk ke GUI bisa jadi settingan yang berubah
atau partisi penuh, dan lainnya.
Bagaimana mengatasi masalah seperti diatas ? gampang, perhatikan dan pahami.
```
![Examples](https://lh3.googleusercontent.com/-pVjcA8SiQ-I/XlL2EDJH1sI/AAAAAAAAMl4/s0luFNm-NdYee9s58r6SJZY0csenyqNgQCLcBGAsYHQ/s1600/1582495244527295-5.png)
```
> Solve problem :
Ketikan command / perintah seperti dibawah :
  - startx 
Jika masih sama seperti diatas (command not found) coba cara dibawah :
  - sudo apt-get update
  - sudo apt-get install gdm3 
Pada bagian instalasi ulang KDE (K Desktop Environment)
terserah kita mau instalasi kde apa, ada banyak varian kde di linux
bisa cek website di bawah ini : 
```
* [`Varian KDE`](https://ketikbagi.blogspot.com/2016/06/jenis-jenis-desktop-environment-linux.html)
```
Setelah anda menginstal dan memilih KDE (K Desktop Environment)
Silahkan reboot ulang Laptop / PC anda, ketikan perintah dibawah :
  - sudo reboot atau bisa dengan
  - sudo systemctl reboot
Dan lihat Environment baru anda, mudah bukan ?
```
![Examples](https://raw.githubusercontent.com/syssaturn404/LINUX-Troubleshooting/master/Dekstop/ex.png?token=AROMCFSN6HHLRCD65OUGJXDAC7C7A)
