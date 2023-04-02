# Nama : Muhammad Farid Baehaqi (tim: FE-08)

# Penjelasan

## Jawaban Nomor 1
### Soal :
1. Kita sudah mengetahui bahwa banyaknya user maksimal adalah 100.
Buat sebuah program yang menampilkan teks ‘User ke - 1 … User ke - 100’ pada setiap baris di halaman HTML.
Lakukan FOR LOOP pada Javascript.

### Jawaban :
jawaban tertera pada file [Jawaban Nomor 1.html](https://github.com/faridbaehaqi20/Tugas_JS-Dasar-Looping/blob/main/Jawaban%20Nomor%201.html "Github Farid")

**Penjelasan ada pada comment pada kode berikut : **

```html
<h2>Jumlah User</h2>
    <ul id="list"></ul>
    <script>
        // Mengambil elemen ul #list
        const list = document.getElementById("list");
        // input nilai ke variabel user
        let user = 100;
        // Lakukan perulangan berdasarkan jumlah user
        for (let i = 1; i <= 100; i++) {
        // console.log('User ke - ' + i + '<br>');
        document.write('User ke - ' + i + '<br>');
        };
    </script>
```

## Jawaban Nomor 2
### Soal :
2. Lakukan pengulangan menggunakan FOR LOOP untuk melakukan penambahan nilai sebanyak 10 kali.

- Nilai awal = 0
- Pengulangan = 10 kali
- Nilai awal ditambah 2 setiap pengulangan
- Tampilan hasil penambahan pada setiap pengulangan


### Jawaban :
jawaban tertera pada file [Jawaban Nomor 2.html](https://github.com/faridbaehaqi20/Tugas_JS-Dasar-Looping/blob/main/Jawaban%20Nomor%202.html "Github Farid")

**Penjelasan ada pada comment pada kode berikut : **

``` html
 <script>
    // input nilai awal ke variabel nilai awal
    let nilaiAwal = 0;
    // lakukan perulangan sebanyak 10
    for (let i = 1; i <=10; i++ ) {
        // setiap perulangan nilai awal di tambah 2
        nilaiAwal += 2;
        // menampilkan perulangan dan total nilai awal
        console.log("Hasil penambahan pada pengulangan ke-" + i + " adalah " + nilaiAwal);
    }
</script>
```


## Jawaban Nomor 3
### Soal :
3.  Lakukan pengulangan dengan FOR LOOP yang melakukan iterasi dari 0..20.
- Setiap iterasi/pengulangan lakukan pengecekan apakah nilai tersebut ganjil atau genap.
- Tampilkan keterangan ganjil dan genap pada sebuah nilai setiap pengulangan


### Jawaban :
jawaban tertera pada file [Jawaban Nomor 3.html](https://github.com/faridbaehaqi20/Tugas_JS-Dasar-Looping/blob/main/Jawaban%20Nomor%203.html "Github Farid")

**Penjelasan ada pada comment pada kode berikut : **

``` html
 <script>
    // lakukan perulangan sebanyak 20
    for (let i = 1; i <= 20; i++) {
      // setiap perulangan melakukan pengecekan apakah perulangan ganjil atau genap lalu menampilkan nya
      if (i % 2 == 0) {
        console.log(i + " adalah bilangan genap");
      } else {
        console.log(i + " adalah bilangan ganjil");
      }
    }
  </script>
```




## Jawaban Nomor 4
### Soal :
4. Tampilkan sebuah Konfirmasi Pop Up kepada user menggunakan confirm();
-Berikan teks ‘Apakah anda mau mengulang’ pada box confirm
-Jika user memilih ‘OK’ maka program akan terus menampilan pop up yang sama
-Jika user memilih ‘Cancel’ maka program akan menampilkan teks ‘Perulangan sudah dilakukan sebanyak …(jumlah klik OK yang dilakukan user)




### Jawaban :
jawaban tertera pada file [Jawaban Nomor 4.html](https://github.com/faridbaehaqi20/Tugas_JS-Dasar-Looping/blob/main/Jawaban%20Nomor%204.html "Github Farid")

**Penjelasan ada pada comment pada kode berikut : **

``` html
 <script>
    // mendeklarasikan variabel jumlah perulangan
    let count = 0;
    // melakukan perulangan jika nilai true adalah benar
    while (true) {
      // menampilkan confirm dan menyimpan hasilnya ke variable confirmbox
      let confirmBox = confirm("Apakah anda mau mengulang?");
      // melakukan pengecekan nilai variabel confirmbox
      if (confirmBox == true) {
        count++;
      } else {
        // menampilkan jumlah perulangan
        alert("Perulangan sudah dilakukan sebanyak " + count + " kali.");
        break;
      }
    }
  </script>
```


## Jawaban Nomor 5
### Soal :
5. Buat sebuah program kuis.
Tampilkan prompt() untuk meminta inputan dari user. Tampilan teks ‘Sebutkan kepanjangan dari nama IB (Impact Byte)?’
- Lakukan pengecekan apakah jawaban dari user sudah benar
- Jika benar, tampilkan alert ‘Selamat jawaban kamu benar’
- Jika salah, lakukan pengulangan untuk menampilkan prompt() yg sama hingga jawaban dari user benar





### Jawaban :
jawaban tertera pada file [Jawaban Nomor 5.html](https://github.com/faridbaehaqi20/Tugas_JS-Dasar-Looping/blob/main/Jawaban%20Nomor%205.html "Github Farid")

**Penjelasan ada pada comment pada kode berikut : **

``` html
 <script>
    // Mendeklarasikan variabel answer dengan sebagai jawaban awal user
    let answer = "";
    // Mengkonversikan jawaban user menjadi huruf kecil
    while (answer.toLowerCase() != "impact byte") {
        // Menampilkan prompt
        answer = prompt("Sebutkan kepanjangan dari nama IB (Impact Byte)?");
        // Melakukan pengkondisian jawaban benar atau salah
        if (answer.toLowerCase() == "impact byte") {
          // Kalau benar akan menampilkan alert benar
          alert("Selamat jawaban kamu benar!");
        } else {
          // Kalau salah akan menampilkan alert salah
          alert("Jawaban kamu salah, coba lagi!");
        }
    }
  </script>
```