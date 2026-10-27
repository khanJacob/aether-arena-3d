# ⚔️ Aether Arena 3D

**Aether Arena 3D**, mobil ve masaüstü tarayıcılar için geliştirilmiş, yüksek vuruş hissi (screen shake, damage flash, knockback), 200° kavisli savurma mekaniği, seviye atlama yetenek ağacı ve silah sandıkları (lootbox) içeren izometrik bir aksiyon RPG arena oyunudur.

---

## 🎮 Temel Özellikler

- **200° Kavisli Savurma Mekaniği (Cleave):** Yakın dövüş silahlarında (Dev Titan Kılıcı, Kıyamet Baltası) nişan aldığın yöne doğru 200 derecelik geniş bir kavisle hilal kesiş dalgası patlatır.
- **Yüksek Vuruş Hissi (Game Juice):**
  - **Ekran Sarsıntısı (Camera Shake):** Darbe anında dinamik kamera titremesi.
  - **Hasar Parlaması (Hit Flash):** Canavarlar darbe aldığında bembeyaz parlayarak geriye fırlar.
  - **Uçan Hasar Sayıları:** Kritik (`CRIT!`) ve element hasar göstergeleri.
  - **Dahili Ses Sentezleyici:** Tok metal çarpmaları ve sub-bass vuruş sesleri (Web Audio API).
- **Run İçi Seviye Atlama & Yetenek Ağacı:**
  - Düşmanlardan düşen 3D mor XP kristalleri toplanır.
  - Seviye atlandığında 3 rastgele yetenek kartı seçilir:
    - ⚡ *Zincirleme Şimşek* (Elektrik alan hasarı)
    - 🔥 *Alev Dalgaları* (Saniyede Yanma Hasarı)
    - ❄️ *Buzul Kilidi* (Dondurma & Yavaşlatma)
    - 🩸 *Kan Emici* (Vampirizm - can çalma)
    - 💨 *Fırtına Hızı* (+%35 saldırı hızı)
    - 💥 *Ölümcül Darbe* (+%25 kritik şansı, x2.2 hasar)
- **Geniş Silah Envanteri & Kademeli Sandıklar:**
  - Kılıçlar, Baltalar, Yaylar ve Asalar.
  - 📦 Bronz, 🔮 Gümüş ve 👑 Altın Sandıklar (Lootbox).
  - Sadece **🪙 Altın** para birimi ve kalıcı bakiye sistemi.
- **İkili Dokunmatik Kontrol (Twin-Stick):**
  - Sol Joystick: Hareket
  - Sağ Joystick: Manuel Nişan
  - ⚡ DASH: Anlık ileri fırlama.
- **Çoklu Run Modları:** 3 Tur (Blitz), 5 Tur (Standart), 10 Tur (Warlord) ve Ranksız (Casual).

---

## 🚀 Çalıştırma

Yerel bir HTTP sunucusu başlatarak doğrudan tarayıcıdan oynayabilirsiniz:

```bash
cd arena-rpg
python3 -m http.server 8082
```

Ardından tarayıcınızdan açın: `http://localhost:8082`

---

## 🛠️ Teknolojiler
- **Motor:** WebGL / Three.js (r128)
- **Ses:** Web Audio API (Harici ses dosyası gerektirmez)
- **Platform:** Mobil & Masaüstü (Android, iOS, Chrome, Safari)
