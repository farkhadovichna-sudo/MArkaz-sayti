# Raqobat siyosati va iste'molchilar huquqlari tadqiqotlari markazi

Markazning rasmiy veb-sayti — raqobat siyosati, iste'molchilar huquqlari va bozor tahlillari bo'yicha tadqiqotlar va xizmatlarni taqdim etuvchi to'liq frontend.

🌐 **Demo:** sizning GitHub Pages havolangiz bu yerga keladi (masalan, `https://username.github.io/markaz-website/`)

---

## Xususiyatlar

- 🎯 **To'liq responsiv dizayn** — mobil, planshet va desktop uchun
- 🎠 **Avtomatik hero slayder** — 3 ta slayd, 6 soniya intervalda
- 📰 **Yangiliklar bo'limi** — featured + vertikal scroll bilan
- 📊 **Jonli statistika** — animatsiyali sonlar (counter animation)
- 🔍 **Qidiruv tizimi** — modal oynada, jonli filter (`/` tugmasi yoki search ikonkasi)
- 🎬 **Video kutubxona** — gorizontal infinite scroll
- 📈 **Bozor indikatorlari** — mini grafiklar va trendlar
- 🌐 **3 til** — UZ / RU / EN tanlash tugmalari
- ♿ **Accessibility** — shrift hajmi boshqaruvi (A-, A, A+)
- 🛠 **Admin panel (CMS)** — yuqori-o'ngdagi qulf ikonkasidan ochiladi
  - Boshqaruv paneli (dashboard) — statistika va so'nggi murojaatlar
  - Yangiliklar (CRUD jadval bilan)
  - Tadqiqotlar arxivi
  - Ekspertlar boshqaruvi
  - Murojaatlar (inbox)
  - Media kutubxona
  - Tizim sozlamalari

---

## Texnologiyalar

- **HTML5** — semantik markup
- **Tailwind CSS** (CDN orqali) — utility-first uslublash
- **Vanilla JavaScript** — hech qanday framework yo'q, tez ishlaydi
- **Material Symbols** — Google ikonkalar
- **Montserrat** — Google Fonts
- **Unsplash** — placeholder rasmlar

Build qadami **shart emas** — bu butunlay statik HTML fayl.

---

## Mahalliy ishga tushirish

```bash
# Repozitoriy klonlash
git clone https://github.com/USERNAME/markaz-website.git
cd markaz-website

# Faqat brauzerda ochish kifoya
open index.html
# yoki Linux'da
xdg-open index.html
```

Yoki oddiy mahalliy server orqali:

```bash
# Python 3
python3 -m http.server 8000

# Node.js (npx)
npx serve

# PHP
php -S localhost:8000
```

So'ngra brauzerda: `http://localhost:8000` ochiladi.

---

## GitHub Pages'ga deploy qilish

### 1-usul: Web interfeysi orqali (eng oson)

1. GitHub'da yangi repozitoriy yarating (masalan, `markaz-website`)
2. **Upload files** tugmasini bosing
3. Bu papkadagi barcha fayllarni torting yoki tanlang
4. **Commit changes** ni bosing
5. Repozitoriy **Settings → Pages** ga o'ting
6. **Source:** `Deploy from a branch` ni tanlang
7. **Branch:** `main` va `/ (root)` ni tanlab **Save** bosing
8. 1-2 daqiqa kuting — saytingiz `https://USERNAME.github.io/markaz-website/` manzilida ishlaydi

### 2-usul: Buyruq satri orqali

```bash
# Loyiha ichida
git init
git add .
git commit -m "Birinchi commit: Markaz sayti"
git branch -M main
git remote add origin https://github.com/USERNAME/markaz-website.git
git push -u origin main
```

So'ngra yuqoridagi 5–8 qadamlarni bajaring.

---

## Tuzilma

```
markaz-website/
├── index.html       # Asosiy va yagona sahifa
├── README.md        # Bu fayl
├── LICENSE          # MIT litsenziya
├── .gitignore       # Git tomonidan e'tiborsiz qoldiriladigan fayllar
└── .nojekyll        # GitHub Pages uchun (Jekyll'ni o'chiradi)
```

---

## Tezkor tugmalar

- **`/`** — Qidiruv oynasini ochish
- **`ESC`** — Modal oynalarni yopish
- **Admin panel** — yuqori-o'ngdagi 🛡 ikonkasi

---

## Sozlash

### Ranglarni o'zgartirish

`index.html` faylida `tailwind.config` bo'limini toping. `primary: "#002a78"` (asosiy navy rang) — bu yerda o'zgartiring.

### Yangilik qo'shish

`<!-- Latest News -->` bo'limini toping va yangi `<article>` blokini qo'shing.

### Rasmlarni almashtirish

Hozir Unsplash'dan placeholder rasmlar ishlatilmoqda. O'zingizning rasmlaringizni qo'shish uchun:

1. `images/` papkasi yarating
2. Rasmlarni shunga ko'chiring
3. `src="https://images.unsplash.com/..."` ni `src="images/yourimage.jpg"` ga almashtiring

---

## Litsenziya

MIT — istalgan tarzda foydalanish mumkin. Tafsilotlar uchun [LICENSE](./LICENSE) faylini ko'ring.

---

## Aloqa

Savol yoki taklif bo'lsa, GitHub issue oching yoki email: `info@markaz.uz`
