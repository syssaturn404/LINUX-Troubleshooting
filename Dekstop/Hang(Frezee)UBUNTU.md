### :octocat: Syssaturn404 Repo :dizzy:
![Image](https://i.ytimg.com/vi/pSHxBkHAcxg/maxresdefault.jpg)
```
Sering sekali saat bekerja kita mengalami masa dimana sistem operasi tidak merespon setiap input
dan tidak dapat melakukan operasi apapun atau yang sering dikenal dengan istilah not responding.
Saat komputer mengalami not responding di sistem operasi Windows
biasanya kita akan menekan tombol CTRL-ALT-DEL untuk membuka Task Manager
lalu melakukan memilih menu (meskipun tidak selalu berhasil). 
Namun di Linux, CTRL-ALT-DEL lebih sering tidak berhasil untuk dilakukan saat komputer hang
sehingga memaksa kita untuk mematikannya secara paksa lewat tombol power.
Mematikan komputer lewat tombol power sangat tidak disarankan, kenapa..? karena bisa merusak performa komputer itu sendiri. 
Hardisk yang dipaksa berhenti secara paksa dapat meningkatkan resiko mengalami kerusakan akibat bad sector. 
Oleh karena itu selalu usahakan untuk mematikan komputer dengan benar. 
Lalu bagaimana saat komputer betul-betul mengalami hang/not responding dan sama sekali
tidak bisa diapa-apakan lagi selain dimatikan paksa..?
Solusinya adalah dengan kita menggunakan REISUB. Apa itu..?
```
### WHAT THIS REISUB ?
```
Linux memiliki sebuah trik yang bisa memaksa sistem Linux melakukan restart meskipun sedang dalam kondisi not responding. 
Caranya ialah dengan menahan tombol ALT + PrntSct/SysRq diikuti tombol R + E + I + S + U + B 
(jika ingin melakukan shutdown, gunakan R + E + I + S + U + O). 
Dengan menggunakan kombinasi tombol tersebut, kita bisa melakukan restart dengan cara yang lebih aman tanpa menekan tombol
power secara paksa atau yang lebih parah, mencabut kabel power/baterai, itu akan sangat merusak bagian komponen pc.
Jadi, bagaimana REISUB / tombol kombinasi diatas ini bekerja..?
Diantara kombinasi - kombinasi diatas adalah REISUB dan REISUO. 
System kerja tombol kombinasi / REISUB adalah seperti dibawah ini :
    - R: Merubah sistem keyboard dari raw mode ke XLATE mode
    - E: Mengirim sinyal SIGTERM ke semua proses selain init (proses induk)
    - I: Mengirim sinyal SIGKILL ke semua proses selain init (proses induk)
    - S: Melakukan sinkronisasi semua filesystem yang di-mount
    - U: Melepas semua filesystem yang ter-mount dalam read-only mode
    - B: Melakukan proses reboot untuk sistem tanpa melepas partisi atau melakukan sinkronisasi filesystem yang terpasang
```
