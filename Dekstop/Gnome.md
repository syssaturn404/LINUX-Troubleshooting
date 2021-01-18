### :octocat:Gnome Extension:dizzy:
```
Gnome Tweak Tool adalah aplikasi yang memudahkan kita untuk mengganti tampilan di Linux, 
khususnya yang menggunakan desktop Gnome. 
Defaultnya, aplikasi ini belum terpasang saat kalian menginstall Linux.
Mungkin ada beberapa orang awam yang masih bingung dengan 
suasana linux yang tidak didapatkan di windows.
saya mendapati pertanyaan dari salah satu problem yang ada di linux.
"Mengapa panel shortcut saya tidak muncul ?"
"Mengapa tiba2 panel dekstop menghilang ? padahal saya tidak melakukan apapun."
Hal itu adalah hal yang biasa, bagaimana mengatasinya ? 
coba anda cari aplikasi gnome tweak tool, yang sudah saya sebutkan diatas.
jika belum menginstalnya, ikuti intruksi dibawah.
jika sudah abaikan saja, lanjut ke tahap berikutnya.
> root@kali:~# sudo add-apt-repository universe
> root@kali:~# sudo apt-get update
> root@kali:~# sudo apt install gnome-tweak-tool
```
![Examples](https://github.com/syssaturn404/LINUX-Troubleshooting/blob/master/Dekstop/shell%20not%20enable.png)
```
Setelah saya buka, dan saya ingin meng-enable kan extension panel saya akan tetapi
saya mendapati error "Shell user-theme extension not enabled" bagaimana mengatasi ini ?
jika anda mendapati masalah yang seperti ini, berarti fitur ini belum aktif di 
device anda, bagaimana mengaktifkannya ? cara mengatasinya cukup mudah.
ketikan perintah dibawah ini ke dalam prompt :
> root@kali:~# sudo apt-get install chrome-gnome-shell
Selanjutnya install extensi User Theme. Klik link dibawah ini dan install ke browser kalian.
```
- [x] [Untuk Firefox](https://addons.mozilla.org/id/firefox/addon/gnome-shell-integration/)
- [x] [Untuk Chrome](https://chrome.google.com/webstore/detail/gnome-shell-integration/gphhapmejobijbbhgpjhcjognlahblep/)
- [x] [Jika Masalah Tidak Terselesaikan](https://qastack.id/ubuntu/142054/why-does-installing-gnome-shell-extensions-from-extensions-gnome-org-fail-silent)
```
Jika sudah, anda tinggal menyalakan / enable extension di dalam gnome tweak tool tsb
dan seting sesuka hati anda, masalah yang saya temui sejauh ini, hanya seperti ini.
mudah bukan ? lanjut oprekk
```
![Done:)](https://github.com/syssaturn404/LINUX-Troubleshooting/blob/master/Dekstop/Screenshot%20from%202021-01-18%2020-00-53.png)
