### :octocat:Restoring-NET:dizzy:
```
Aircrack-ng suite menyediakan metode untuk menonaktifkan fungsi 
Network Manager melalui perintah airmon-ng check kill. 
Sayangnya mereka tidak memberi tahu Anda cara memulihkan Manajer 
Jaringan setelah mengaktifkan airmon-ng check kill.
Perintah sebenarnya dikubur di skrip airmon-ng.
Pernahkah anda mengalami masalah seperti diatas ?
```
![Hello:)](https://github.com/syssaturn404/LINUX-Troubleshooting/blob/master/Network/ss.jpg)
```
Tiga (3) perintah dibawah ini mungkin akan menyelesaikan masalahmu :

root@kali:~# service network-manager restart
root@kali:~# service NetworkManager restart
root@kali:~# service avahi-daemon restart

atau ~>
root@kali:~# /etc/init.d/network-manager
root@kali:~# /etc/init.d/network-manager start

```
![Done:)](https://github.com/syssaturn404/LINUX-Troubleshooting/blob/master/Network/Screenshot%20from%202021-01-18%2019-17-01.png)
