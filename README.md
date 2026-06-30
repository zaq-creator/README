# README
# Team Manifesto & Kebijakan Komunikasi Tim

**Proyek:** Aplikasi Mobile Kantin Pintar Kampus.  
**Tim Konsultan:** Scrum Team Baru.  
**Tujuan Dokumen:** Memastikan konflik komunikasi internal dari tim lama (seperti format data JSON yang tidak konsisten dan saling menyalahkan) tidak terulang kembali, serta menjaga kesehatan mental tim dari *burnout*.

---

## 1. SOP Code Review (Komunikasi Konstruktif & Sopan)

Untuk mencegah konflik personal saat melakukan peninjauan kode (*code review*) di GitHub, seluruh anggota tim wajib mengikuti aturan komunikasi konstruktif berikut:

### A. Prinsip Umum
* **Fokus pada Kode, Bukan Personal:** Kritik ditujukan kepada baris kode yang ditulis, bukan pada kemampuan atau pribadi programmer.
* **Berikan Solusi atau Pertanyaan:** Jangan hanya menyalahkan, tetapi berikan saran perbaikan atau tanyakan alasan di balik penulisan kode tersebut.
* **Gunakan Pendekatan "I-Message" atau Saran Terbuka:** Hindari kalimat perintah yang menghakimi.

### B. Tabel Contoh Komunikasi

| Kalimat yang DILARANG (Destruktif) |  Kalimat yang DIANJURKAN (Konstruktif) |
| :--- | :--- |
| *"Kode apaan nih? Berantakan banget, bikin error di mana-mana!"*  | *"Halo ges, fungsi di baris ini menyebabkan error saat di-run. Tolong dicek kembali ya, apa perlu kita debug bersama?"*  |
| *"Format JSON-nya salah lagi. Lu niat ngerjain Backend nggak sih?"* | *"Izin konfirmasi, format JSON untuk endpoint `/api/menu` sepertinya ada perubahan dari kontrak awal. Apakah bisa disesuaikan kembali dengan dokumentasi API kita?"*  |
| *"Hapus fungsi ini, gak efisien banget. Ganti pakai looping!"* | *"Menurut saya, bagian ini akan jauh lebih efisien jika kita optimalkan menggunakan looping agar performanya lebih cepat. Bagaimana menurutmu?"* |

---

## 2. Protokol Komunikasi & Manajemen Diri (Anti-Burnout)

Guna menjaga produktivitas dan mencegah kejenuhan ekstrim (*burnout*), seluruh anggota tim wajib mematuhi batasan jam kerja koordinasi berikut:

### A. Aturan Jam Kerja & Koordinasi
* **Jam Kerja Standar:** Koordinasi aktif, diskusi teknis, dan *Daily Standup Meeting* dilakukan pada hari **Senin s.d. Jumat pukul 08.00 - 18.00 WIB**.
* **Batas Akhir Chat (Curfew Time):** Dilarang keras melakukan chat koordinasi, *mention* tugas baru, atau meminta revisi di atas **pukul 21.00 WIB**.

### B. Pengecualian Kondisi Darurat (System Down)
Aturan batas jam malam (pukul 21.00 WIB) dapat diabaikan **HANYA** jika terjadi kondisi kritis berikut:
1. **Server/Sistem Down:** Aplikasi mengalami *crash* total di lingkungan *staging* atau *production* menjelang rilis.
2. **Kebocoran Data Kritis:** Terjadi kegagalan keamanan pada API Authentication yang mengancam data pengguna.

> **Sanksi Pelanggaran:** Anggota tim yang melanggar batas jam komunikasi tanpa situasi darurat wajib membelikan kopi/minuman saat pertemuan evaluasi sprint berikutnya.

---

## 3. Kontrak Integrasi Data (Solusi Konflik JSON)

Belajar dari kesalahan tim lama yang bubar akibat format JSON yang sering berubah tanpa komunikasi, tim kami menetapkan aturan mutlak:
* **Single Source of Truth:** Semua format *request* dan *response* API wajib didokumentasikan di satu tempat (misal: Postman Collection atau Swagger).
* **Prosedur Perubahan:** Backend developer **dilarang keras** mengubah nama *key* atau struktur data JSON secara sepihak sebelum mendapatkan persetujuan dari Frontend developer melalui forum diskusi singkat.
