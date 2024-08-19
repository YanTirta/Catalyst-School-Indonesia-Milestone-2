# **Mereproduksi Snapshot**

Mengaudit Snapshot berarti mereproduksi snapshot langsung dari data blockchain dan membandingkannya dengan data snapshot yang diterbitkan secara resmi.

### **Mendapatkan nomor slot Batas Waktu Pendaftaran**


<img width="670" alt="Mereproduksi snapshot 1" src="https://github.com/user-attachments/assets/1a3bae6e-2b2a-4b0f-9be9-f3e1afe962d9">

### **Menjalankan snapshot Raw**

Bagian pertama dari snapshot mengumpulkan registrasi mentah dan informasi ADA yang dipertaruhkan dan memvalidasinya sesuai dengan [CIP-15](https://cips.cardano.org/cip/CIP-15) dan [CIP-36](https://cips.cardano.org/cip/CIP-36) .

*Catatan: Beberapa delegasi, sebagaimana ditetapkan oleh CIP-36, tidak didukung. Ini akan dideteksi sebagai pendaftaran yang tidak valid. Hanya pendaftaran yang berisi satu kunci pemungutan suara yang didukung dan valid.*


<img width="672" alt="Mereproduksi snapshot 2" src="https://github.com/user-attachments/assets/7a88cf8f-8d12-4941-81ea-4a276e27e20e">

### **Memproses snapshot dengan parameter Fund 10**

Ini menyaring pendaftaran berdasarkan kekuatan suara minimum yang diizinkan:


<img width="672" alt="Mereproduksi snapshot 3" src="https://github.com/user-attachments/assets/5d838496-e9c5-4693-846e-0f1823a0721d">

### **Artefak Snapshot Resmi**

Segera setelah artefak snapshot resmi yang akan digunakan untuk Dana 10 tersedia, artefak tersebut akan ditautkan ke sini.

Dimungkinkan untuk menjalankan snapshot secara independen hingga dipublikasikan.
