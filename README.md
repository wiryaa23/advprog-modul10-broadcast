**Nama**: Wirya Dharma Kurnia  <br /> 
**Kelas**: AdPro B  <br />
**NPM**: 2306152115 <br />

## Reflection

### 2.1: Original code, and how it run

- Server
![broadcast1](images/broadcast1.png)

- Client 1
![broadcast2](images/broadcast2.png)

- Client 2
![broadcast3](images/broadcast3.png)

- Client 3
![broadcast4](images/broadcast4.png)

- How to run server? <br />
Jalankan command `cargo run --bin server` pada direktori broadcast.

- How to run 3 client? <br />
Jalankan command `cargo run --bin client` pada direktori broadcast. Kali ini, saya menjalankan command tersebut secara terpisah pada 3 terminal berbeda.

- What happens when you type some text in the clients? <br />
Dari screenshot di atas kita dapat melihat bahwa ketika server dijalankan, maka server akan terhubung pada request yang masuk di port 2000. Saat client 1, client 2, dan client 3 terhubung, maka pada server akan muncul log yang memberi informasi berupa `"New connection from (port client yang masuk)"`. Dari sisi client, ketika mereka sudah terhubung dengan server maka akan ada log yang berisi `"From server: Welcome to chat! Type a message"`. Client dapat mengirimkan pesan ke server, dan server akan menerima semua pesan yang dikirim oleh setiap client. Server juga akan mengeluarkan pesan `"From client (alamat port client): (pesan yang dikirim client)"`. Sementara itu, client juga akan menerima pesan yang dikirimkan oleh client-client lain melalui server karena server akan menyimpan connection dengan setiap client sehingga mereka saling terhubung satu sama lain. 