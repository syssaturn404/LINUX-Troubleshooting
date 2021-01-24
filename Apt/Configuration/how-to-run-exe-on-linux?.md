### :octocat: Syssaturn404 :dizzy:
![Examples](https://i0.wp.com/itsfoss.com/wp-content/uploads/2016/09/Complete-Beginners-Guide-run-Windows-Software-Linux.jpg?fit=800%2C450&ssl=1)
### HOW TO RUN EXE ON LINUX ?
```
Bagi orang awam yang belum terbiasa dengan suasana linux, mungkin akan bingung mengenai masalah :
- Bagaimana kita menjalankan program .exe di linux..?
- Bagaimana agar kita bisa menginstall program .exe di linux..?
- etc.
Saya sering mendapati pertanyaan seperti itu, terkadang juga saya menggunakannya
untuk menjalankan program yang ada di windows, ke linux, seperti halnya membuat
backdoor .exe di windows, kita membutuhkan .exe untuk dijalankan.
Akan tetapi, di linux tidak seperti di windows jika melakukan instalasi
harus menunggu mendownload, analisa keasliannya dahulu, tekan install
dan konfigurasi environment dulu, etc.
Berbeda dengan linux, dari awal instalasi hanya dengan cloning
PPA / Repository (apt-get) sudah bisa menginstall dan tinggal 
menunggu, hingga tahap konfigurasi bisa dilakukan di terminal
sedang di windows tidak bisa, menurut saya pribadi linux hanya untuk
orang - orang malas, yang tidak mau menunggu. 
Bagaimana mengatasi ini..? Gampang, kita membutuhkan wine.
```
![Examples-WINE-On-UBUNTU](https://3.bp.blogspot.com/-_B1zz15cu1Y/WIiL83lIt8I/AAAAAAAAYuQ/NNC0bebGH_0wXCCbYCwfmOjs_f8C5hHfACLcB/s1600/wine20stable.png)
### WHAT THIS MINE ?
```
Apa itu wine..? bagaimana wine bekerja di linux..?
Wine merupakan sebuah proyek yang bertujuan untuk membuat agar sistem operasi 
bertipe Unix (Unix-like) dan X11 yang berjalan pada suatu komputer pribadi
dapat menjalankan program yang khusus dibuat untuk Microsoft Windows.
Tapi tidak sepenuhnya, program windows berjalan sempurna di linux.
```
![Examples](https://github.com/syssaturn404/LINUX-Troubleshooting/blob/master/Apt/Configuration/ex.jpg)
### HOW TO INSTALL WINE ?
```
Cara menginstal wine tidak suit, buka terminal anda / tekan secara bersama CTRL + ALT + T
Ketikan command dibawah ini :
> sudo su
[sudo] password for ***: (masuk sebagai root, program ini membutuhkan hak superuser / root)
> sudo apt-get install wine
> sudo dpkg --add-architecture i386 -y && sudo apt-get update -y && sudo apt-get install wine32 -y (Tunggu hingga selesai)
Sekarang tinggal kalian jalankan programnya, bagaimana caranya ..? ketikan command / perintah dibawah :
> wine./Nama-Program.exe (atau tidak dengan ./)
Atau kalian bisa konfigurasi sendiri, caranya ketika comand / perintah dibawah : 
> sudo wine reconfigure
```
![Examples](https://github.com/syssaturn404/LINUX-Troubleshooting/blob/master/Apt/Configuration/IMG_20210125_022111.png)
