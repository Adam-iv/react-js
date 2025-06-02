🔹 React JS

📌 Pengertian

React JS adalah pustaka JavaScript open-source yang digunakan untuk membangun antarmuka pengguna (User Interface / UI), terutama untuk aplikasi web. React dikembangkan oleh Facebook dan dirilis pertama kali pada tahun 2013.
React menggunakan pendekatan berbasis komponen, di mana UI dibagi menjadi bagian-bagian kecil dan dapat digunakan kembali. Ini membuat proses pengembangan lebih terstruktur dan efisien.

🔍 React JS (React.js) 

🔧 1. Arsitektur React JS

React JS menggunakan arsitektur berbasis komponen. Ini berarti UI dibagi menjadi potongan-potongan kecil yang disebut komponen, yang dapat digunakan kembali.
Contohnya:

function Button(props) {
  return <button>{props.label}</button>;
}

🔁 2. Virtual DOM

Alih-alih memanipulasi DOM langsung (yang lambat), React membuat salinan virtual dari DOM (Virtual DOM). Ketika state berubah, React membandingkan virtual DOM sebelumnya dengan yang baru, lalu hanya mengubah bagian yang berbeda (diffing algorithm) — ini meningkatkan performa.

💡 3. State dan Props

State: Menyimpan data internal dalam komponen.

Props: Digunakan untuk mengirim data dari satu komponen ke komponen lain.

Contoh:

function Greeting({ name }) {
  return <h1>Hello, {name}</h1>;
}

🧠 4. Hooks (React 16.8 ke atas)

Hooks memungkinkan kamu untuk menggunakan state dan lifecycle method di dalam komponen fungsi:

Contoh useState:

const [count, setCount] = useState(0);

Contoh useEffect:

useEffect(() => {
  console.log('Component mounted or updated');
}, [count]);


🧱 5. React Ecosystem (Tambahan)

React hanya fokus pada View Layer (V pada MVC). Untuk fitur tambahan:

Routing: react-router-dom

State Management: Redux, Zustand, Recoil

Form Handling: Formik, React Hook Form

Testing: Jest, React Testing Library


🌐 6. Penggunaan React JS di Industri

Digunakan oleh banyak perusahaan besar:

Facebook (Meta)

Instagram

Netflix

Airbnb

Tokopedia

Gojek (untuk web)

⚙️ Fitur Utama

Component-Based Architecture
UI dibagi menjadi komponen kecil yang dapat digunakan ulang.
Virtual DOM
Performa aplikasi meningkat karena React hanya memperbarui elemen yang berubah, bukan seluruh halaman.
Unidirectional Data Flow
Aliran data hanya dari parent ke child, mempermudah debugging dan pelacakan data.
JSX (JavaScript XML)
Sintaks seperti HTML yang digunakan dalam JavaScript untuk mendefinisikan UI.

✅ Kelebihan React JS

Reusable components.
Kinerja tinggi dengan Virtual DOM.
Komunitas besar dan ekosistem kaya (Redux, React Router, dll).
Cocok untuk SPA (Single Page Application).

❌ Kekurangan React JS

Butuh waktu belajar (terutama bagi pemula).
Seringnya pembaruan membuat developer harus terus mengikuti perkembangan.
Hanya menangani bagian view (butuh library tambahan untuk routing dan state management).

📌 Penggunaan React JS

Digunakan untuk membangun aplikasi web interaktif seperti:

Dashboard

E-commerce

Aplikasi media sosial

Admin panel



🔹 React Native

📌 Pengertian

React Native adalah framework open-source yang dikembangkan oleh Facebook pada tahun 2015. React Native memungkinkan developer membangun aplikasi mobile (iOS & Android) menggunakan JavaScript dan React.
React Native menerjemahkan komponen React ke dalam komponen native di masing-masing platform (Android/iOS), sehingga aplikasi terasa seperti aplikasi asli (native).

📱 React Native 

🏗️ 1. Arsitektur React Native

React Native memungkinkan kamu menulis komponen dengan JavaScript, tetapi saat dijalankan, komponen tersebut diubah menjadi komponen native sesuai platform:
Misalnya:

<Button title="Tekan Aku" onPress={handleClick} />

Akan diterjemahkan menjadi UIButton (iOS) atau Button (Android).

🔌 2. Bridge Architecture

React Native menggunakan Bridge: jembatan antara JavaScript dan Native Modules. Saat aplikasi berjalan:

UI ditulis dalam JavaScript

JS dikompilasi ke native code menggunakan bridge (asynchronous dan serialized)

Kelemahan: bisa menjadi bottleneck jika komunikasi JS-Native terlalu sering (contohnya animasi kompleks).

🧰 3. Native Modules

Jika ada fitur yang tidak didukung langsung oleh React Native (misalnya akses ke fitur khusus perangkat), kamu bisa menulis kode native di Java/Kotlin (Android) atau Swift/Objective-C (iOS) dan menghubungkannya ke JavaScript.

🔁 4. Live Reload vs Hot Reload

Live Reload: muat ulang seluruh aplikasi ketika file berubah.

Hot Reload: hanya mengganti bagian kode yang berubah tanpa kehilangan state.

💼 5. React Native di Dunia Nyata

React Native digunakan oleh:

Facebook

Instagram

Discord (iOS)

Skype

Bloomberg

Shopee (beberapa bagian)

Gojek (di beberapa fitur)

⚙️ Fitur Utama

Write Once, Use on iOS and Android
Satu basis kode untuk dua platform.
Access to Native APIs
Bisa menggunakan API asli melalui Native Modules.
Live & Hot Reloading
Perubahan kode langsung terlihat tanpa harus membangun ulang seluruh aplikasi.
Bridging
Bisa menjembatani antara kode JavaScript dan native (Swift/Obj-C/Java/Kotlin).

✅ Kelebihan React Native

Efisiensi waktu dan biaya karena 1 kode untuk 2 platform.
Performa mendekati native.
Komunitas aktif dan banyak plugin.
Dukungan kuat dari Meta (Facebook).

❌ Kekurangan React Native

Tidak cocok untuk aplikasi dengan logika dan grafik kompleks (misalnya game 3D).

Terkadang masih perlu penulisan kode native.

Performa tidak selalu setara dengan aplikasi full-native.

Debugging bisa lebih rumit (karena melibatkan dua lapisan: JavaScript & Native).

📌 Penggunaan React Native

Aplikasi mobile yang tidak memerlukan performa ekstrem.
MVP (Minimum Viable Product) atau prototipe cepat.
Aplikasi sosial, e-commerce, atau produktivitas.

🔁 Perbandingan React JS vs React Native



Aspek
React JS
React Native




Platform
Web browser
Android & iOS


Bahasa
JavaScript + HTML (JSX)
JavaScript + Native Components


DOM
Virtual DOM
Native APIs & komponen asli


Styling
CSS
StyleSheet (seperti CSS dalam JS)


Navigasi
React Router
React Navigation


Output
Halaman web
Aplikasi mobile


Akses ke perangkat
Terbatas (melalui browser)
Langsung ke perangkat (kamera, GPS)


