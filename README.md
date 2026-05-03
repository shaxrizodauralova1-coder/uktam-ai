Yaxshi joyga kelibsiz, endi keyingi qadamlarni tartib bilan qilaylik. Hozircha sizda faqat `index.html` va `.gitignore` bor, README ham bo‘sh.

Avval savol:  
Sun’iy intellektni **noldan model yozmoqchimisiz**, yoki **ChatGPT, OpenAI, boshqa API**lardan foydalangan holda “AI sayt / bot” qilmoqchimisiz?

Ikkala variant bo‘yicha yo‘l ko‘rsatma beraman, siz qaysi yo‘lni tanlaganingizni yozing. Hozircha eng oson varianti – **veb-sahifaga AI chat qo‘shish** misolini ko‘rsataman.

---

## 1. Loyihani tuzish (frontend varianti)

GitHub’dagi papkangizga quyidagilarni qo‘shing:

- `index.html`
- `script.js`
- `style.css`
- `README.md`

### index.html (soddalashtirilgan misol)

```html
<!DOCTYPE html>
<html lang="uz">
<head>
  <meta charset="UTF-8" />
  <title>Utkam AI</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>
  <h1>Utkam AI Chat</h1>
  <div id="chat-box"></div>
  <div id="input-area">
    <input id="user-input" type="text" placeholder="Savolingizni yozing..." />
    <button id="send-btn">Yuborish</button>
  </div>

  <script src="script.js"></script>
</body>
</html>
```

### style.css (oddiy ko‘rinish uchun)

```css
body {
  font-family: Arial, sans-serif;
  max-width: 800px;
  margin: 0 auto;
  padding: 20px;
}
#chat-box {
  border: 1px solid #ccc;
  padding: 10px;
  height: 400px;
  overflow-y: auto;
  margin-bottom: 10px;
}
.message {
  margin: 5px 0;
}
.message.user {
  text-align: right;
  color: blue;
}
.message.ai {
  text-align: left;
  color: green;
}
#input-area {
  display: flex;
  gap: 10px;
}
#user-input {
  flex: 1;
  padding: 8px;
}
```

### 2. AI bilan ishlash (OpenAI API misoli)

`script.js` ichida API chaqiradigan kod bo‘ladi. Buning uchun:
1. openai.com’dan API kalit oling
2. Orqa tomonda (backend) server yozish yaxshi (Node.js yoki Python), chunki API kalitni frontendga qo‘yib bo‘lmaydi (yashirin bo‘lishi kerak).

Shuning uchun savol:

- Qaysi til/sistemada ishlamoqchisiz?  
  - Node.js (JavaScript, `server.js`)  
  - Python (`app.py`, FastAPI/Flask)  
  - Yoki hozircha faqat **HTML/JS o‘rganish** va keyin backend qo‘shish?

Siz tanlagan varianti bo‘yicha to‘liq kod namunalarini (backend + frontend) yozib beraman:

- Node.js bo‘lsa: `package.json`, `server.js`, OpenAI chaqiradigan endpoint, GitHub’ga qanday qo‘yish.
- Python bo‘lsa: `requirements.txt`, `app.py`, route’lar, qanday ishga tushirish.

---

## 3. README yozish (minimal)

`README.md`ga hozircha shuni yozib qo‘yishingiz mumkin:

```markdown
# Utkam AI

Bu loyiha – sun'iy intellekt yordamida foydalanuvchilar bilan suhbatlashuvchi veb-ilova.

## Ishga tushirish

1. Repozitoriyani klon qiling:
   ```bash
   git clone https://github.com/<sizning-nickingiz>/utkam-ai.git
   ```
2. Papkaga kiring va kerakli bog'liqliklarni o'rnating (tanlangan texnologiyaga qarab).
3. Loyihani ishga tushiring.
```

---

Endi navbat sizda:

1. Qaysi yo‘lni tanlaysiz:
   - A) OpenAI/API bilan ishlovchi web-chat  
   - B) O‘zingiz oddiy ML modeli yozib ko‘rish (Python + sklearn/torch)  
   - C) Faqat HTML/CSS/JS dizayn, keyin AI qo‘shamiz

2. Qaysi tilni bilasiz yoki o‘rganmoqchisiz: **JavaScript (Node.js)** yoki **Python**?

Shuni yozing, keyingi xabarda to‘liq qadam-baqadam kod bilan sizning GitHub loyihangizni davom ettirib beraman.
