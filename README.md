# TUGAS MENJELASKAN REACT JS
## Nama Kelompok
1. Adam Izmu Vriezgi
2. Fathurrahman
3. Wahyu Saputra
4. Alisia Maulidina
5. Robby Sugara

## Pengertian React JS

React JS adalah pustaka JavaScript open-source yang digunakan untuk membangun antarmuka pengguna (User Interface / UI), terutama untuk aplikasi web. React dikembangkan oleh Facebook dan dirilis pertama kali pada tahun 2013.
React menggunakan pendekatan berbasis komponen, di mana UI dibagi menjadi bagian-bagian kecil dan dapat digunakan kembali. Ini membuat proses pengembangan lebih terstruktur dan efisien.

## Fitur-Fitur React JS

1.  JavaScript XML (JSX)
Fitur ini merupakan ekstensi syntax JavaScript yang digunakan dalam pembuatan elemen React. Developer menggunakan untuk menyematkan kode HTML pada objek JavaScript, JSX memungkinkan pengembang untuk menggabungkan logika JavaScript dengan tampilan HTML secara lebih mudah dan intuitif.

2. Document Object Model (DOM) Virtual
Fitur ini berfungsi untuk menyajikan halaman web dalam tampilan struktur data (tree/poho), ReactJS menyimpan struktur data DOM Virtual dalam memorinya, sehingga jika terdapat perubahan pada bagian tertentu dalam struktur data tersebut tidak perlu merender ulang semua datanya. ReactJS menggunakan konsep Virtual DOM untuk mempercepat proses rendering. Dengan menggunakan Virtual DOM, ReactJS hanya memperbarui komponen yang benar-benar berubah, daripada melakukan rendering ulang keseluruhan tampilan.

3.  Komponen dan Properti React
ReactJS memungkinkan pengembang untuk memisahkan antarmuka pengguna menjadi komponen-komponen kecil yang dapat digunakan kembali. Setiap komponen memiliki logika dan tampilan sendiri, sehingga memudahkan pengembangan dan pemeliharaan kode. Elemen React yang dihasilkan akan menentukan bagaimana tampilan antarmuka pengguna yang dilihat oleh user (sisi klien).

4. Manajemen State
State atau keadaan merupakan objek JavaScript yang mewakili satu bagian dari sebuah komponen. Setiap kali user berinteraksi dengan aplikasi, state juga akan berubah dengan merender UI baru untuk menampilkan perubahan dari interaksi tersebut. Library manajemen state memiliki peran penting dalam memfasilitasi komunikasi dan berbagi data antara komponen-komponen React. Saat ini, terdapat beberapa library manajemen state pihak ketiga yang tersedia, dan antara lain yang paling terkenal adalah Redux dan Recoil. Library-library ini memungkinkan pengembang untuk dengan mudah mengelola state aplikasi dan memperbarui komponen secara efisien. Redux dan Recoil telah menjadi populer di komunitas pengembangan React karena kemampuan mereka dalam mengatur dan menyimpan state, serta menyediakan aliran data yang jelas dan terstruktur di seluruh aplikasi.

5. Navigasi Terprogram
Navigasi terprogram adalah situasi di mana serangkaian kode menghasilkan sebuah tindakan yang mengarahkan pengguna ke area tertentu. Contohnya adalah dalam proses login dan mendaftar akun, dimana secara terprogram tindakan tersebut akan mengarahkan pengguna ke halaman baru.
React Router merupakan library standar react untuk perutean yang menyediakan berbagai metode navigasi terprogram yang aman antar komponen tanpa mengharuskan user mengklik link apa pun.

## Cara Kerja React


Salah satu manfaat utama untuk menggunakan React adalah Anda bisa memasukkan kode HTML dengan JavaScript.
User bisa membuat representasi node DOM dengan mendeklarasikan fungsi Element di React.kode di bawah ini, yang berisi kombinasi HTML dan JavaScript:

```
React.createElement("div", { className: "red" }, "Children Text");
React.createElement(MyCounter, { count: 3 + 5 });
```

Anda mungkin menyadari bahwa sintaksis kode HTML di atas mirip dengan XML. Nah, tapi, bukannya menggunakan class DOM tradisional, React menggunakan className.
Tag JSX memiliki nama, turunan, dan atribut. Ekspresi dan nilai numerik harus ditulis di dalam kurung kurawal. Tanda kutip dalam atribut JSX mewakili string, mirip dengan JavaScript.
Biasanya, React ditulis menggunakan JSX dan bukan JavaScript standar untuk menyederhanakan komponen dan menjaga tampilan kode agar tetap rapi.
Berikut adalah contoh kode React yang ditulis menggunakan JSX:
```
MyCounter count={3 + 5} />;
var GameScores = {player1: 2,player2: 5};
DashboardUnit data-index="2">
h1>Scores/h1>Scoreboard className="results" scores={GameScores} />
/DashboardUnit>;
```
Penjelasan tag HTML di atas adalah seperti berikut:

```MyCounter>``` mewakili variabel yang disebut count yang nilainya adalah ekspresi numerik.
GameScores adalah object literal yang memiliki dua pasangan prop-value.
```DashboardUnit>```adalah block XML yang dirender di halaman.
```scores={GameScores}``` adalah atribut skor, yang mendapatkan nilainya dari object literal GameScores tadi.
Aplikasi React biasanya memiliki satu node DOM root. Merender elemen ke dalam DOM akan mengubah UI halaman.

Sebagai contoh, kode berikut menampilkan “Hello World” di halaman dengan merender elemen menjadi node DOM yang disebut root.
```
div id="root">/div>
const element = h1>Hello, world/h1>;
ReactDOM.render(element, document.getElementById('root'));
```
Setiap kali sebuah komponen React menghasilkan satu elemen, Virtual DOM akan memperbarui DOM asli agar sesuai.

## Cara Instal React

Pastikan NodeJS telah terinstall sebelumnya, karena React JS nantinya berjalan sebagai UI, dengan NodeJS sebagai runtime.

Link Download ```https://nodejs.org/en```
   ```
   node -v
   npm -v
   npm install -g create-react-app
   ```
   ![Tampilan UI](https://github.com/Adam-iv/react-js/blob/main/img/Screenshot%202025-06-07%20021343.png)

Apabila proses install package selesai, Anda dapat melakukan pemeriksaan package menggunakan perintah berikut:

   ```
   $ create-react-app --version
   ```
   ![Tampilan UI](https://github.com/Adam-iv/react-js/blob/main/img/Screenshot%202025-06-07%20021353.png)

