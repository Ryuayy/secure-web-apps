
# Secure Web App - UTS RPL Lanjutan

## 👩‍🎓 Nama: Sri Rahayu  
## 🆔 NIM: 2023140074  

Aplikasi web sederhana berbasis Django yang dikembangkan sebagai bagian dari Ujian Tengah Semester (UTS) untuk mata kuliah Rekayasa Perangkat Lunak Lanjutan.

---

## 🚀 Fitur Utama

- ✅ Registrasi dan Login User
- 🔐 Password Hashing (default Django hasher)
- 🛡️ Perlindungan dari SQL Injection (ORM-based)
- 🔑 JSON Web Token (JWT) Authentication
- 📁 RESTful API menggunakan Django REST Framework

---

## 📦 Instalasi

```bash
git clone https://github.com/Ryuayy/secure-web-app.git
cd secure-web-app
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```

---

## 🧪 Pengujian API

Gunakan Postman untuk menguji endpoint berikut:

- `POST /register/` – Registrasi pengguna baru
- `POST /token/` – Login dan dapatkan JWT token
- `GET /profile/` – Akses data pengguna (dengan JWT)

---

## 📂 Struktur Folder

```
secure-web-app/
├── manage.py
├── requirements.txt
├── README.md
└── core/
    ├── models.py
    ├── serializers.py
    ├── views.py
    ├── urls.py
```

---

## 📌 Catatan Keamanan

- Password di-hash secara default oleh Django (`make_password`)
- Semua input divalidasi menggunakan DRF Serializer
- Endpoint dilindungi oleh JWT dari `djangorestframework-simplejwt`
- Tidak menggunakan raw SQL → bebas dari SQL Injection

---

## 📃 Lisensi

Hak cipta oleh Sri Rahayu - 2025
