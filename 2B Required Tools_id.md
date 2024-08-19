# **Alat yang dibutuhkan**

### **Sinkronisasi db**

Petunjuk instalasi dapat ditemukan [di sini](https://github.com/IntersectMBO/cardano-db-sync/blob/master/doc/docker.md) .

Pastikan dbSync dan database PostgreSQL berjalan, dan database disinkronkan setelah pukul 10 malam UTC pada tanggal 23 Agustus 2023.

*Catatan: JIKA dbSync Anda tidak disinkronkan setidaknya hingga tanggal ini, hasil dari menjalankan snapshot akan tidak akurat. Ini karena snapshot diambil pada saat rollback pada blockchain tidak mungkin memengaruhi data snapshot, dan karenanya snapshot sepenuhnya dapat direproduksi dan stabil. Ini dijamin dengan menempatkan satu Epoch penuh antara batas waktu pendaftaran dan waktu paling awal snapshot final dapat diambil.*

### **Alat Snapshot Katalis**

Alat snapshot berasal dari [repo github Catalyst Core](https://github.com/input-output-hk/catalyst-core) . Kloning repo tersebut lalu buat alat yang diperlukan.

### **Membangun alat**

**alat_snapshot:**

> kargo membangun -r -p voting_tools_rs

**kotak peralatan katalis:**

> membangun kargo -r -p kotak alat katalis
