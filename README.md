# 🏛️ Соёмбо сурах самбар

Монгол бичиг сурахад зориулсан интерактив quiz, үсгийн сан, XP болон level системтэй сургалтын сайт.

**Онцлог:**
- 📖 23 үндсэн үсэг + 10 Монгол тоо
- 🎮 Quiz game — 4 сонголттой асуулт, XP болон level систем
- 🔊 Дуу авиа — зөв/буруу хариулт дээр дуу
- 🎊 Confetti animation — quiz дуусахад
- ⌨️ Гар товчлол — 1–4 товч сонгох, Enter дараагийнх
- 🔥 Өдөр дараалсан streak
- 💾 LocalStorage — XP, level хадгалагдана
- 📱 PWA — утсанд апп болгож суулгах боломжтой
- 🌐 Offline горимд ажиллана

---

## 🚀 GitHub Pages дээр deploy хийх заавар

### Алхам 1 — GitHub аккаунт үүсгэх
1. [github.com](https://github.com) руу орж **Sign up** дарна
2. Username сонгохдоо энгийн, богино нэр ашиглаарай (жишээ: `munkh`, `soymbo`)

### Алхам 2 — Repository үүсгэх
1. GitHub-д нэвтэрсний дараа баруун дээр **+** → **New repository** дарна
2. Repository name: `soymbo` гэж бичнэ
3. **Public** сонгоно (Private бол GitHub Pages ажиллахгүй)
4. **Create repository** дарна

### Алхам 3 — Файлуудаа upload хийх
Repository үүсэлсний дараа:
1. **uploading an existing file** холбоос дарна
2. Дараах файлуудыг БҮГДИЙГ нэг дор чирч оруулна:
   - `index.html` ← `soymbo.html`-ийг **index.html** болгож нэрлэнэ!
   - `robots.txt`
   - `sitemap.xml`
   - `404.html`
   - `og-image.svg`
3. **Commit changes** дарна

> ⚠️ **Чухал:** `soymbo.html` файлыг `index.html` болгож нэрлэнэ — GitHub Pages нь `index.html` файлыг автоматаар нүүр хуудас болгоно.

### Алхам 4 — GitHub Pages идэвхжүүлэх
1. Repository дотор **Settings** таб руу орно
2. Зүүн талын цэснээс **Pages** дарна
3. **Source** хэсэгт → **Deploy from a branch** сонгоно
4. **Branch** → `main` сонгоод `/root` → **Save** дарна
5. Хэдэн минут хүлээнэ

### Алхам 5 — Сайтаа нээх
Deploy дууссаны дараа:
```
https://YOUR_USERNAME.github.io/soymbo/
```
Жишээ: `https://munkh.github.io/soymbo/`

---

## 🔧 URL солих (чухал!)

`index.html` файл дотор `YOUR_USERNAME` гэсэн хэсгийг өөрийн GitHub username-аар солино:

```
https://YOUR_USERNAME.github.io/soymbo/
```
→
```
https://munkh.github.io/soymbo/
```

`sitemap.xml` болон `robots.txt` файлд мөн адил солих хэрэгтэй.

---

## 🌐 Google дээр гарах (SEO)

Deploy хийсний дараа Google Search Console-д бүртгэнэ:

1. [search.google.com/search-console](https://search.google.com/search-console) руу орно
2. **Add property** → URL prefix → сайтынхаа URL оруулна
3. Эзэмшлийг батлах (HTML tag аргыг ашиглаарай)
4. **Sitemaps** → `sitemap.xml` submit хийнэ

Google индексэд орох хугацаа: **3–14 хоног**

---

## 📁 Файлын бүтэц

```
soymbo/
├── index.html        ← Үндсэн сайт (soymbo.html-ийг ингэж нэрлэнэ)
├── robots.txt        ← Хайлтын системд зориулсан
├── sitemap.xml       ← Google индексэд орох
├── 404.html          ← Буруу хуудас руу ороход redirect
├── og-image.svg      ← Social media preview зураг
└── .github/
    └── workflows/
        └── deploy.yml ← Auto-deploy (GitHub Actions)
```

---

## 💡 Нэмэлт зөвлөгөө

- **Custom domain** авахыг хүсвэл: `.mn` domain нь жилд ~30,000₮ болдог
- **Analytics** нэмэхийг хүсвэл: Google Analytics эсвэл Plausible ашиглаж болно
- **Шинэчлэлт хийхэд:** Файлуудаа GitHub дотор шууд edit хийж commit хийхэд автоматаар deploy болно
