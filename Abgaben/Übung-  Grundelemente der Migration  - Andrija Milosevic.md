# Übung Pfade 

---

## 📁 Lokal (Windows-Dateisystem)

### Gegebene Verzeichnisstruktur

C:\Daten  
├─ Bilder  
│  ├─ Blume.jpg  
│  └─ test.html  
├─ CSS  
│  └─ main.css  
└─ index.html  

---

### 1) Absoluter Pfad von `main.css`

C:\Daten\CSS\main.css

---

### 2) Relativer Pfad (in `index.html`) zum Bild `Blume.jpg`

Bilder/Blume.jpg

---

### 3) Absoluter Pfad (von `main.css`) zum Bild `Blume.jpg`

C:\Daten\Bilder\Blume.jpg

---

### 4) Relativer Pfad (von `main.css`) zum Bild `Blume.jpg`

../Bilder/Blume.jpg

---

### 5) Relativer Pfad (von `test.html`) zum Bild `Blume.jpg`

Blume.jpg  
(Alternative: ./Blume.jpg)

---

## 🌐 Im Netz (Webserver)

### Gegeben

- Domain: ihreadresse.ch
- Lokaler Root-Pfad: /srv/var/www/htdocs
- Document Root: /htdocs

### Dateien (innerhalb von /htdocs)

- wp-content/uploads/2022/5/Dokument.pdf
- wp-content/plugins/neon/files/download.php

---

### 6) Lokaler & absoluter Pfad zu `Dokument.pdf`

/srv/var/www/htdocs/wp-content/uploads/2022/5/Dokument.pdf

---

### 7) Lokaler & absoluter Pfad zu `download.php`

/srv/var/www/htdocs/wp-content/plugins/neon/files/download.php

---

### 8) URL von `Dokument.pdf`

https://ihreadresse.ch/wp-content/uploads/2022/5/Dokument.pdf

---

### 9) URL von `download.php`

https://ihreadresse.ch/wp-content/plugins/neon/files/download.php

---

### 10) Relativer Pfad in `download.php` → `Dokument.pdf`

../../../uploads/2022/5/Dokument.pdf
