###  :octocat:Syssaturn404 Repo:dizzy:
![Examples](https://cdn-brilio-net.akamaized.net/news/2020/07/03/187600/1260939-meme-lupa-password-media-sosial.jpg)

### How to change password for linux ?
```
Pasti pernah sebagian dari kita terkadang melupakan kata sandi.
banyak faktor yang membuat kita melupakan kata sandi, faktor beban pikiran, dan lainnya
atau bisa jadi terkadang disaat selesai instalasi, malah password incorect ? banyak 
pertanyaan yang timbul, bagaimana cara mengatasi itu.
Bagaimana mengatasi itu semua ? Mudah kok, perhatikan gambar dibawah :
```
![Examples](https://www.linux.org/attachments/bildschirmfoto-2020-06-13-um-20-30-37-png.6535/)
```
Bagaimana mengatasi semua itu ? Hal itu membuat saya jengkel
Saya ingin mengembalikan seperti semula linux saya.
> Langkah pertama, restart PC / Komputer anda, lalu pada opsi GRUB loader seperti gambar dibawah :

```
![Examples](https://hackersterminal.com/wp-content/uploads/2019/12/Kali-Linux-Boot-Screen-1536x864.jpg)
```
> Tekan E, lalu muncul seperti dibawah :
```
![Examples](https://hackersterminal.com/wp-content/uploads/2019/12/quiet-splash-Kali-linux.jpg)
```
> Lalu pada statement / pernyataan ro single blabla.. ganti dengan :
> 'rw single init=/bin/bash' tanpa petik, lalu tekan enter & ctrl + x
komputer / pc mulai reboot dan masuk pada CLI(Command Line Interface).
```
![Examples](https://i.imgur.com/506U4VF.png)
```
> Ketikan di CLI perintah dibawah ini :
> passwd root (untuk mengganti kata sandi root)
> passwd nama-user (untuk mengganti kata sandi user)
Lalu masukan new password, dan ketikan ulang password.
Dan rebot ulang komputer anda / pc dengan perintah :
> exec /usr/sbin/init atau tekan tombol power dan aktifkan kembali.
dan masukan kembali username dan password anda. 
```
![Examples](https://github.com/syssaturn404/LINUX-Troubleshooting/blob/master/Dekstop/ex.png)
