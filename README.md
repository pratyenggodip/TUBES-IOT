# TUBES IOT “PAKAN AYAM OTOMATIS BERBASIS IOT MENGGUNAKAN SENSOR ULTRASONIC

:::info
KELOMPOK X
- Pratyenggo Damar Iswara Putra (1103194141)
- Aditya Ramadhan (1103194161)
- Muhammad Iqbal (1103194114)
- Athmad Taufik Rahman (1103190028)
:::

## LATAR BELAKANG

Proyek pakan ayam otomatis berbasis Internet of Things (IoT) dengan menggunakan sensor 
ultrasonik memiliki latar belakang yang mencakup efisiensi pengelolaan pakan, pemantauan kesehatan ayam, penghematan energi, monitoring jarak jauh, optimasi produktivitas, tren teknologi pertanian, dan keberlanjutan lingkungan. Penggunaan sensor ultrasonik dalam proyek ini mencerminkan tren menuju pertanian pintar untuk meningkatkan efisiensi, produktivitas, dan keberlanjutan.

## TUJUAN PROJECT 
Tujuan dari project ini adalah pemenuhan nilai tugas besar untuk mata kuliah IoT (Internet Of Things) dan memahami cara kerja IoT.

## DASAR TEORI 
* Alat yang dibutuhkan:
1. Node MCU   

![image](https://hackmd.io/_uploads/rkuQIzHuT.png)

NodeMCU merupakan sebuah papan pengembangan (development board) berbasis mikrokontroler ESP8266, yang memiliki dukungan WiFi terintegrasi. ESP8266 adalah sebuah mikrokontroler yang sangat populer dalam pengembangan IoT karena kemampuannya untuk terhubung dengan jaringan WiFi. NodeMCU menggunakan firmware Lua, sebuah bahasa pemrograman scripting ringan yang memungkinkan pengembangan perangkat lunak untuk IoT menjadi lebih mudah.

2. Breadborard

![image](https://hackmd.io/_uploads/Hkw8UMrua.png)

Breadboard adalah perangkat atau papan percobaan yang digunakan dalam elektronika untuk merancang, menguji, dan menyusun prototipe rangkaian listrik tanpa harus melakukan soldering.

3.	Kabel Data Micro USB
    
![image](https://hackmd.io/_uploads/SyOKIMHuT.png)
    
Untuk menghubungkan laptop dengan wemos node MC

4.	HCS 04 Ultrasonic

![image](https://hackmd.io/_uploads/HymiUzBuT.png)

HC-SR04 Ultrasonic adalah sebuah sensor ultrasonik yang banyak digunakan dalam proyek-proyek elektronika, terutama dalam konteks pengukuran jarak.

5.	Paket Kabel Jumper

![image](https://hackmd.io/_uploads/rkNA8GSua.png) 

Kabel jumper adalah kabel pendek yang digunakan dalam elektronika dan prototyping untuk menghubungkan dua titik atau komponen dalam rangkaian listrik.


* Koneksi yang digunakan:

    -WiFi - WiFi adalah teknologi nirkabel yang memungkinkan perangkat elektronik, seperti komputer, smartphone, tablet, dan perangkat lainnya, untuk terhubung ke jaringan internet atau jaringan lokal (LAN) tanpa menggunakan kabel fisik.
    
    -MQTT - MQTT (Message Queuing Telemetry Transport) adalah protokol komunikasi ringan yang dirancang untuk digunakan pada kondisi jaringan yang tidak stabil atau dengan bandwidth terbatas.
    
    -SOURCE CODE
    
    1. NODE SENSOR 

    ![image](https://hackmd.io/_uploads/H1adPMS_T.png)
    
    ![image](https://hackmd.io/_uploads/BJUYvGHO6.png)

    ![image](https://hackmd.io/_uploads/H1ccPGHu6.png)

    ![image](https://hackmd.io/_uploads/SyOjvMS_p.png)

    2. NODE SERVO 

    ![image](https://hackmd.io/_uploads/HJyAPzBdp.png)
    
    ![image](https://hackmd.io/_uploads/Hku0vzHOa.png)

    ![image](https://hackmd.io/_uploads/HJNJOfrOp.png)




* ## RINCIAN BIAYA



|    **NO**   |          **Nama Barang**         | **Jumlah** | **Harga** | **Jumlah** |
|:-----------------:|:-------------------------:|:--------------:|:---------------:|:---------:|
|   1  | Node MCU |   2    |         Rp. 35.000        |   Rp. 75.000        |
|   2  | Micro Servo mg90 |   1    |         Rp. 25.000        |   Rp. 25.000        |
|   3  | Kabel Data Micro USB |   2    |         Rp. 7.500        |   Rp. 15.000        |
|   4  | HCS04 Ultrasonic |   2    |         Rp. 12.000        |   Rp. 24.000        |
|   5  | Paket Kabel Jumper |   1    |         Rp. 26.000        |   Rp. 26.000        |
|       Total                                             ||||  Rp. 163.000         |

* ## CARA KERJA ALAT

Node pertama (Node MCU terhubung dengan HCSR04) mengirim data berupa data jarak melalui mqtt dan di tampilkan melalui node red, dengan juga dikirim data berupa close dan open di waktu yang telah di tentukan, variable open dan close akan dibaca oleh Node kedua (Node MCU terhubung dengan servo motor) jika menerima mqtt open maka servo akan bergerak untuk membuka pakan jika close akan menutup jalur pakan. Tetapi kami disini menemukan kendala berupa alat tidak bisa manual dan sensor sering eror mendapatkan jarak

* ## KESIMPULAN

Kesimpulan dari laporan di atas adalah bahwa proyek pakan ayam otomatis berbasis Internet of Things (IoT) menggunakan sensor ultrasonik telah berhasil dikembangkan oleh Kelompok X. Latar belakang proyek mencakup berbagai aspek, termasuk efisiensi pengelolaan pakan, pemantauan kesehatan ayam, penghematan energi, monitoring jarak jauh, optimasi produktivitas, tren teknologi pertanian, dan keberlanjutan lingkungan. Tujuan proyek melibatkan pemenuhan tugas besar untuk mata kuliah IoT dan pemahaman tentang cara kerja IoT. Dalam pelaksanaannya, kelompok menggunakan NodeMCU, sensor ultrasonik HC-SR04, servo motor, dan komponen elektronik lainnya. Penggunaan NodeMCU sebagai platform pengembangan memungkinkan konektivitas WiFi, sementara sensor ultrasonik digunakan untuk mengukur jarak dan servo motor untuk mengendalikan pemberian pakan. Meskipun proyek ini memberikan pemahaman yang lebih dalam tentang aplikasi IoT, kelompok menghadapi kendala, seperti ketidakmampuan operasi manual dan masalah sensor ultrasonik yang sering eror dalam pengukuran jarak. Rincian biaya juga disajikan untuk memberikan gambaran tentang investasi yang dibutuhkan untuk mengembangkan proyek ini. Kesimpulannya, proyek ini mencerminkan upaya yang signifikan dalam menerapkan teknologi IoT untuk meningkatkan efisiensi dan otomatisasi dalam manajemen pakan ayam. Dengan memahami kelebihan dan kendala proyek, dapat dilakukan pengembangan lebih lanjut untuk meningkatkan kinerja dan ketangguhan sistem.

[link github](https://github.com/pratyenggodip/TUBES-IOT.git)
