🔹 React JS
📌 Pengertian
React JS adalah pustaka JavaScript open-source yang digunakan untuk membangun antarmuka pengguna (User Interface / UI), terutama untuk aplikasi web. React dikembangkan oleh Facebook dan dirilis pertama kali pada tahun 2013.
React menggunakan pendekatan berbasis komponen, di mana UI dibagi menjadi bagian-bagian kecil dan dapat digunakan kembali. Ini membuat proses pengembangan lebih terstruktur dan efisien.
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



✅ Contoh Sederhana React JS
Kita akan buat aplikasi web kecil yang menampilkan nama dan tombol untuk mengubahnya.
📁 File: App.js
jsxSalinEditimport React, { useState } from 'react';
function App() {
const [name, setName] = useState('AiMSTARMan');
return (
<div style={{ textAlign: 'center', marginTop: '50px' }}>
<h1>Hello, {name}!</h1>
<button onClick={() => setName('ProPlayer')}>
Ganti Nama
</button>
</div>
);
}
export default App;

🧰 Tools:


Bisa dijalankan di https://codesandbox.io/


Atau jalankan dengan npx create-react-app namaproject



✅ Contoh Sederhana React Native
Kita akan buat aplikasi mobile kecil yang menampilkan teks dan tombol untuk mengubah teks tersebut.
📁 File: App.js
jsxSalinEditimport React, { useState } from 'react';
import { View, Text, Button, StyleSheet } from 'react-native';
export default function App() {
const [name, setName] = useState('AiMSTARMan');
return (
<View style={styles.container}>
<Text style={styles.text}>Hello, {name}!</Text>
<Button title="Ganti Nama" onPress={() => setName('ProPlayer')} />
</View>
);
}
const styles = StyleSheet.create({
container: {
flex: 1,
justifyContent: 'center',
alignItems: 'center'
},
text: {
fontSize: 24,
marginBottom: 20
}
});

🧰 Tools:


Jalankan di emulator menggunakan Expo Go atau dengan perintah:
sqlSalinEditnpx create-expo-app namaproject
cd namaproject
npx expo start
