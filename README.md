# myportofolio_mobile

A new Flutter project.

## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Learn Flutter](https://docs.flutter.dev/get-started/learn-flutter)
- [Write your first Flutter app](https://docs.flutter.dev/get-started/codelab)
- [Flutter learning resources](https://docs.flutter.dev/reference/learning-resources)

For help getting started with Flutter development, view the
[online documentation](https://docs.flutter.dev/), which offers tutorials,
samples, guidance on mobile development, and a full API reference.

### Tugas 7

1. Widget tree itu struktur pohon dari semua widget di aplikasi Flutter, di mana satu widget bisa membungkus widget lain. Widget yang membungkus disebut parent, yang dibungkus disebut child. Parent ngatur layout dan ngasih constraint ke child-nya, terus child ngebangun tampilannya sendiri di dalam batas itu. Misal Column jadi parent dari beberapa Text

2. MyHomePage: widget utama halaman beranda (StatelessWidget) yang nyusun seluruh tampilan.
   Scaffold: kerangka dasar halaman, nyediain slot buat appBar dan body.
   AppBar: bar di atas yang nampilin judul “MyPortfolio”.
   Text: nampilin teks, misal judul, sambutan, dan nama item.
   Padding: ngasih jarak di sekeliling widget lain.
   Column: nyusun widget ke bawah (vertikal).
   Row: nyusun widget ke samping (horizontal), dipakai buat deretan tiga InfoCard.
   SizedBox: spasi kosong dengan ukuran tertentu antar widget.
   Center: naruh child di tengah.
   GridView.count: nampilin item dalam bentuk grid, di sini 3 kolom buat tombol menu.
   InfoCard: widget buatanmu buat nampilin info NPM, nama, dan kelas.
   Card: kartu dengan bayangan (elevation) sebagai wadah isi InfoCard.
   Container: kotak buat ngatur lebar dan padding.
   ItemCard: widget buatanmu buat satu tombol menu di grid.
   Material: nyediain warna latar dan sudut membulat, sekaligus efek ripple buat InkWell.
   InkWell: bikin area bisa ditekan (onTap) dengan efek ripple.
   Icon: nampilin ikon di tiap tombol menu.
   SnackBar (lewat ScaffoldMessenger): pesan singkat di bawah layar yang muncul pas tombol ditekan.

3. MaterialApp itu widget yang nyiapin hal-hal dasar aplikasi bergaya Material Design, kayak tema, navigasi/routing, dan halaman awal (home). Makanya dia umum dipakai sebagai root, karena semua widget di bawahnya otomatis dapat akses ke tema, navigator, dan fitur Material lainnya

4. StatelessWidget nggak punya state yang berubah, jadi tampilannya tetap selama datanya sama. Cocok buat yang statis, misal teks judul atau ikon. StatefulWidget punya state yang bisa berubah dan memicu tampilan di-rebuild lewat setState. Pakai ini kalau ada interaksi atau data dinamis, misal counter, form, atau checkbox

5. BuildContext itu kayak penanda posisi sebuah widget di dalam widget tree. Pentingnya, lewat context ini kita bisa ngakses hal-hal dari widget di atasnya, misal Theme.of(context), Navigator.of(context), atau MediaQuery.of(context). Di method build, context dikasih sebagai parameter dan dipakai buat ngambil data atau layanan dari tree tersebut

6. Hot reload nyuntik perubahan kode ke aplikasi yang lagi jalan tanpa ngulang dari awal, jadi state-nya tetap kepegang (kalo misal angka counter nggak reset). Hot restart ngulang aplikasi dari awal, jadi semua state hilang. Kita harus full restart kalau ngubah hal yang cuma dieksekusi sekali di awal, kayak isi main(), nilai variabel global atau static, dan inisialisasi state di initState. Full restart juga perlu kalau ada perubahan native, misal nambah plugin/dependency baru atau ngubah konfigurasi Android/iOS

Dokumentasi: Saya menggunakan AI Gemini 4 Hydrogen untuk membantu saya mengerjakan Tugas 7. Terutama saat saya mentok dengan error dan bingung untuk mencari letak error nya.

Berikut log percakapan saya dengan Gemini: https://share.gemini.google/eQjSgfGTkWnP
