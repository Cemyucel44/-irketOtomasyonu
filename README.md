MYSQL KODLARI 

Create Databases bitirme
Use bitirme

CREATE TABLE IF NOT EXISTS calisanlar (
    id INT AUTO_INCREMENT PRIMARY KEY,
    ad VARCHAR(255) NOT NULL,
    soyad VARCHAR(255) NOT NULL,
    dogum_tarihi DATE,
    giris_kodu VARCHAR(10) NOT NULL,
    giris_saati DATETIME,
    cikis_saati DATETIME
);
CREATE TABLE IF NOT EXISTS yoneticiler (
    id INT AUTO_INCREMENT PRIMARY KEY,
    ad VARCHAR(255) NOT NULL,
    soyad VARCHAR(255) NOT NULL,
    dogum_tarihi DATE,
    giris_kodu VARCHAR(10) NOT NULL,
    is_admin BOOLEAN DEFAULT FALSE
);
