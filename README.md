
## **Lab 9 **


## **Lab 8**
### 1. Perbedaan `Navigator.push` dan `Navigator.pushReplacement`
`Navigator.push` : menambahkan `Route` ke *top of stack* dari `Navigator`.
`Navigator.pushReplacement`:  menambahkan route ke *top of stack* juga menghilangkan `Route` yang sebelumnya.

### 2. *Widget* yang Digunakan
* Text : Menampilkan sebuah *string* dengan *single style*.
* Column: Sebuah *widget* yang menampilkan *children*-nya secara vertikal.
* Row : Sebuah *widget* yang menampilkan *children*-nya secara horizontal.
* Scaffold : Menerapkan dasar dari *visual layout* Material Design.
* AppBar : *App bar* dari Material Design
* Padding : Memberi *padding* pada *child* yang diletakkan di dalamnya.
* Center : Sebuah *widget* yang *child*-nya akan berposisi di tengah.
* Drawer: Panel yang berdiri secara horizontal di pinggir `Scaffold` yang menampilkan tautan navigasi dalam aplikasi.
*  ListTile : Sebuah baris yang biasanya mengandung teks dan ikon.
* Navigator : Mengelola *child widgets* menggunakan prinsip *stack*.
* MaterialPageRoute: Rute modal yang menggantikan seluruh layar dengan transisi platform-adaptif.
* SingleChildScrollView : Digunakan agar *child*-nya bisa di-*scroll*.
* Container : *Widget* yang menggabungkan *widget* umum untuk *painting*, *positioning*, dan *sizing*.
* Card: Sebuah panel yang bisa digunakan untuk menampilkan informasi di dalamnya. Memiliki *style* dimana sudutnya sedikit bulat dan terdapat bayangan elevasi.
* CustomScrollView : Kurang lebih sama dengan `SingleChildScrollView` namun lebih fleksibel.
* SliverFillRemainingFill: Sebuah *sliver* yang mengandung sebuah *box child* yang mengisi sisa ruang pada *viewport*.
* Form: *Containter* untuk melakukan *grouping* terhadap beberapa *form field widget*.
* TextFormField: *Field* teks yang bisa digunakan untuk melakukan *input*.
* InputDecoration: Melakukan dekorasi pada sebuah *input field*.
* DropdownButtonFormField: Menu *dropdown*.
* Expanded: Melebarkan *child* dari `Row`, `Column`, atau `Flex` agar mengisi ruang yang masih tersedia.
* Align: Melakukan *aligining* terhadap *child*-nya.
* TextButton : Tombol yang berisi teks.

### 3. Jenis-jenis *event* pada FLutter
1. onPressed        : Terpanggil saat button ditekan
2. onLongPress      : Terpanggil saat button ditekan lama
3. onTap            : Terpanggil saat salah satu popup menu ditekan dan akan menjalankan actions yang telah ditentukan
4. onFocusChanged   : Terpanggil saat focus berganti
5. onSaved          : Terpanggil dengan final value saat form telah di save via FormState
6. onHover          : Terpanggil saat pointer masuk ke button response area
7. onChanged        : Terpanggil saat user meninisiasi sebuah perubahan kepada value TextField

### 4. Cara kerja `Navigator`
`Navigator` menggunakan prinsip stack dalam mengganti halaman. Halaman yang ditampilkan adalah yang berada pada top of stack.

### 5. Implementasi
* Membuat *form* beserta *input field* yang dinginkan mengacu pada tutorial.
* Data-data yang di-input disimpan kedalam sebuah `List`.
* Data yang disimpan berupa `Card`.
* Tampilkan data pada halaman Data Budget sesuai dengan yang sudah ditambahkan dengan memanfaatkan `List` yang tadi sudah dibuat.


## Tugas 7

### 1. Jelaskan apa yang dimaksud dengan *stateless widget* dan *stateful widget* dan jelaskan perbedaan dari keduanya
- Stateless widget : 
  - Widget yang  keadaanya yang tidak "berubah" ketika diberikan interaksi oleh user. 
  - Nilai dari stateless widget sendiri selalu mengikuti parent yang dimilikinya.
  
- Stateful widget :
  - Widget yang dapat "berubah" ketika diberikan interaksi oleh user. 
  - Stateful dapat menyimpan state dirinya untuk kebutuhan program, seperti perubahan nilai dan tampilan widget.
  - Bersifat Dinamis
  
- Contoh pada program, terdapat pada file main.dart. MyApp yang mengandung header & judul web = Stateless, sedangkan MyHomePage yang mengandung isi program = Stateful.

### 2. Sebutkan widget apa saja yang kamu pakai di proyek kali ini dan jelaskan fungsinya.
- Padding : Widget yang memberikan lapisan kosong dengan nilai tertentu (paddding) di sekitaran child dari padding.
- Icon : Widget yang menampilkan logo
- Floating Action Button : Widget untuk menampilkan tombol
- Column : Widget layout yang peletakan child widget sesuai arah vertikal (kolom) .
- Text : Widget untuk menampilkan suatu text serta style nya
- Center : Widget sebagai layout untuk membuat peletakan child menjadi di tengah. 
- Row : Widget layout untuk peletakan child widget sesuai arah horizontal (baris).

### 3. Apa fungsi dari **setState()**? Jelaskan variabel apa saja yang dapat terdampak dengan fungsi tersebut.
Panggilan ke setState ini memberi tahu framework Flutter bahwa ada sesuatu yang berubah di Status ini, yang menyebabkannya menjalankan kembali metode build di bawah ini
sehingga tampilan dapat mencerminkan nilai yang diperbarui. Jika kita berubah _counter tanpa memanggil setState(), maka metode build tidak akan dipanggil lagi, jadi sepertinya tidak ada yang terjadi.

### 4. Jelaskan perbedaan antara *const* dengan *final*.
- Const membuat variabel konstan dari waktu kompilasi saja.
- Final membuat nilai variabel dan tidak dapat diubah di masa mendatang
- Nilai dari keduanya tidak dapat berubah setelah diinisialisasi

### 5. Jelaskan bagaimana cara kamu mengimplementasikan *checklist* di atas.
- Menjalankan flutter create tugas
- Edit judul widget home
- Menambahkan fungsi decrementCounter yang mengurangi variable _counter dengan 1
- Menerapkan  conditional _counter tidak dapat menjadi negatif
- Membuat tombol yang berada di pojok kiri dan kanan bawah menggunakan campuran Padding dan Row terhadap Floating Action Button
- Membuat conditional untuk  variabel _counter agar style dan text pada body berubah tergantung ganjil/genap 

Bonus:
- Arah Row diubah dari kanan ke kiri sehingga kemunculan pertama adalah tombol (+), lalu (-) 
- Terapkan conditional tombol (-) untuk tidak dapat menghilang



