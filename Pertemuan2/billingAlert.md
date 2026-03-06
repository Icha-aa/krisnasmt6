# Membuat Billing Alert di AWS Untuk Menghindari Kelebihan Alokasi Data
1. Login AWS terlebih dahulu di Website resmi AWS

2. Scroll ke bawah lalu klik pada bagian Billing preferences
![alt text](image.png)

3. Di Alert preferences di klik lalu edit
![alt text](image-1.png)

4. Klik bagian Search lalu cari Cloudwatch dan klik
![alt text](image-2.png)

5. Setelah klik maka tampilan nya akan seperti ini. Jika sudah, lalu pilih yang bagian Create Alarms
![alt text](image-3.png)

6. Masuk dibagian ini lalu klik Create Alarm
![alt text](image-4.png)

7. Jika sudah seperti ini lalu klik bagian Select metric
![alt text](image-5.png)

8. Tampilan pada bagian setelah klik Select metric akan seperti ini, lalu klik Billing
![alt text](image-6.png)

9. Lalu klik Total Estimated Charge
![alt text](image-7.png)

10. Lalu ceklis bagian USD dan klik Select metric
![alt text](image-8.png)

11. Jika tampilan sudah seperti ini, sesuaikan nama kalian
![alt text](image-9.png)

12. Scroll dikit, pilih 1 saja dibagian than dan next
![alt text](image-10.png)

13. Tampilan akan seperti ini
![alt text](image-11.png)

14. Klik Create new topic, sesuaikan nama nya, dan masukkan email valid kalian dan Create topic
![alt text](image-12.png)

15. Lalu Next saja
![alt text](image-13.png)

16. Setelah Next sesuaikan nama nya lagi kosongkan saja bagian Alarm description dan Next
![alt text](image-14.png)

17. Jika sudah seperti ini scroll aja kebawah lalu klik Create alarm
![alt text](image-15.png)

18. Nah sudah selesai tampilan akan seperti ini jika berhasil
![alt text](image-16.png)