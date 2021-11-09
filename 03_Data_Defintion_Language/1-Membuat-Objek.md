## **Membuat sebuah objek atau objek lainnya yang belum ada.**
> Query ini berfungsi untuk membuat object bisa berupa database ataupun table jika membuat database, maka hanya perlu melakukan query lalu buat nama database, jika membuat sebuah table maka diikuti juga dengan membuat sebuah kolom dan tipe data pada masing masing kolom

  `CREATE`

  ### Bentuk Umum : `CREATE` + Objek + Nama Object + `;`
  
  - Membuat Database : 
    > `CREATE DATABASE`+ Nama Database + `;`
    
  - Membuat Table : 
    > `CREATE TABLE `+ Nama tabel + `(` + Nama Kolom +` ` + Tipe Data Kolom +`(` + Panjang Data +`) `+ Key + ` AUTO INCREMENT NOT NULL); `
  
  ### Note 
  > - AUTO INCREMENT (Opsional): Berfungsi sebagai penambahan value secara otomatis setiap terjadinya input record baru
  > - NOT NULL (Opsional) : Query yang berfungsi untuk menentukan jika kolom tidak boleh kosong alias null
  > - Jika dalam penamaan terdapat lebih dari 1 kata maka gunakan tanda ``_`` sebagai pengganti spasi.
  
  ### Contoh : 
  
  - Membuat Database : 
    > `CREATE DATABASE Mahasiswa;`

  - Membuat Table : 
    >`CREATE TABLE NILAI (ID INT PRIMARY KEY AUTO INCREMENT);`
    
    >`CREATE TABLE NILAI (ID INT PRIMARY KEY, Nama_Mahasiswa VARCHAR(255) NOT NULL, Nilai INT , Mata_Kuliah VARCHAR(255), Tanggal_Input DateTime);`
   
    >`CREATE TABLE NILAI (ID INT PRIMARY KEY AUTO INCREMENT NOT NULL, ID_Mahasiswa INT NOT NULL, Nama_Mahasiswa VARCHAR(255) NOT NULL, Nilai INT , Mata_Kuliah VARCHAR(255), Tanggal_Input DateTime);`
