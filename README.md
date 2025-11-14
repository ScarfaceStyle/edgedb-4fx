# edgedb-4fx

# ⚡ Bash Automation Toolkit

Koleksi script Bash untuk mempercepat pekerjaan harian, melakukan otomatisasi, dan menjaga sistem tetap efisien. Dibuat dengan fokus pada kesederhanaan, kecepatan, dan kemudahan penggunaan.

## 🔧 Fitur Utama
- Otomatisasi tugas berulang
- Logging bawaan
- Mode verbose untuk debugging
- Struktur modular (mudah dikembangkan)
- Ringan, tanpa dependency tambahan

## 🚀 Instalasi

Clone repository:
git clone https://github.com/username/bash-automation-toolkit.git
cd bash-automation-toolkit

Beri izin eksekusi:
chmod +x run.sh

## ▶️ Cara Menggunakan

Menjalankan script:
./run.sh

Menjalankan dengan parameter:
./run.sh --task backup --verbose

Menampilkan bantuan:
./run.sh --help

## 🧪 Contoh Output
[START] Menjalankan task: backup
[INFO] Memeriksa direktori...
[SUCCESS] Proses selesai dalam 1.02 detik.

## ⚙️ Konfigurasi
File konfigurasi opsional:
config.env

Contoh isi:
TARGET_DIR=/home/user/data
LOG_LEVEL=debug
AUTO_CLEAN=true

Load konfigurasi otomatis jika file config.env tersedia.

## 📂 Struktur Direktori
bash-automation-toolkit/
├── run.sh
├── core/
│   ├── utils.sh
│   ├── logger.sh
│   └── tasks.sh
├── config.env.example
└── README.md

## 🔥 Contoh Isi Script Utama
#!/bin/bash
source core/logger.sh

log_info "Memulai proses..."

if [[ "$1" == "--verbose" ]]; then
  log_debug "Verbose mode aktif"
fi

log_success "Selesai."

## 🤝 Kontribusi

Fork repository ini:
git fork https://github.com/username/bash-automation-toolkit.git

Buat branch baru:
git checkout -b fitur-baru

Push perubahan:
git push origin fitur-baru

Buka Pull Request di GitHub.

## 📄 Lisensi
Lisensi MIT
