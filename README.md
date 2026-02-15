# web-alumni
Fokus pada **komunitas & informasi alumni**, bukan job board!

---

## ⚙️ Cara Instalasi di XAMPP

1. Copy folder `alumni_smk` ke `C:\xampp\htdocs\`
2. Buka **phpMyAdmin** → tab **SQL** → paste isi `database.sql` → klik **Go**
3. Akses: **http://localhost/alumni_smk**

---

## 🔑 Akun Login Default

| Role  | Email              | Password   |
|-------|--------------------|------------|
| Admin | admin@smk.sch.id   | `password` |
| Alumni| budi@email.com     | `password` |

---

## ✨ Fitur Lengkap v2

### Untuk Alumni
| Fitur | Keterangan |
|-------|-----------|
| 📅 Event & Reuni | Lihat event mendatang & yang sudah lewat |
| 📰 Berita & Pengumuman | Info dari sekolah (prestasi, pengumuman, dll) |
| 🖼️ Galeri Foto | Foto kenangan per angkatan |
| 💡 Info Karir | Tips karir, sertifikasi, beasiswa, magang |
| 👤 Edit Profil | Update data diri & password |

### Untuk Admin
| Fitur | Keterangan |
|-------|-----------|
| 👥 Kelola Alumni | CRUD + pencarian nama & tahun lulus |
| 📅 Kelola Event | Tambah/edit/hapus event |
| 📰 Kelola Berita | Tambah/edit/hapus berita & pengumuman |
| 🖼️ Kelola Galeri | Tambah/edit/hapus foto per angkatan |
| 💡 Kelola Info Karir | Tambah/edit/hapus info karir |

---

## 🔐 Keamanan
- Prepared Statement (anti SQL Injection)
- `password_hash()` (password terenkripsi)
- `htmlspecialchars()` (anti XSS)
- Session + Role Check (admin/user)
