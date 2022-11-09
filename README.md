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