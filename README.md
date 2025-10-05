# CI/CD Demo — Deploy Otomatis ke GitHub Pages

Demo proyek ini memperlihatkan penggunaan **CI/CD (Continuous Integration & Continuous Deployment)** menggunakan **GitHub Actions** untuk secara otomatis membangun dan mendeploy website statis ke **GitHub Pages**.

🔗 [Lihat hasil deploy](https://joselumbanraja.github.io/TRY-CI-CD/)

---

##  Cara Kerja (Workflow CI/CD)

1. Kode dipush ke branch `main` → workflow otomatis jalan  
2. Tahap build & test dijalankan (CI)  
3. Jika berhasil, artifact hasil build akan dideploy ke GitHub Pages (CD)  

---

##  Komponen Penting

- `actions/checkout@v4` → mengambil kode dari repo  
- `actions/setup-node@v4` → menyiapkan environment Node.js  
- `actions/upload-pages-artifact@v3` → menyimpan hasil build  
- `actions/configure-pages@v5` (+ `enablement: true`) → mengaktifkan konfigurasi Pages  
- `actions/deploy-pages@v4` → melakukan deploy ke GitHub Pages  

---
