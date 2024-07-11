Kali Linux kurulumunu hatasız bir şekilde yaptığınızı ele alalım. Ama Kali kurulumundan sorna Win11-10 sistemi boot sekmesinde görünmeyebilir. Bunun için: 

1) Kali sistemini aç
2) Komut satırına sırasıyla;

3)     $ sudo su (sonra şifreyi gir)
4)     $ cat /etc/os-release
5)     $ nano /etc/default/grub
6) Açılan defterde ki "GRUB_TIMEOUT=5" değerini 25 yap. (Böylece boot seçmek için vaktimiz olacak)
7) Ctrl+O ve Enter yap. Sonra Ctrl+X yapıp defterden çık. Terminala geri döndükten sonra; 
8)     $ update-grub
9)     $ reboot now
10) Komutlarını çalıştır ve sistemi yaniden başlat. Böylece boot ekranında hem Windows hem de Kali işletim sistemlerini görüp seçebileceksin. Kolay gelsin.

    Görseller
    ![Ekran görüntüsü 2024-07-11 094446](https://github.com/Poyqraz/Kali-Linux-Dual-Boot-Windows-A-amama/assets/48729799/9d2f7ef6-72be-481f-926a-5868f8de30ec)

    
