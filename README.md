# 🐑 مراعي تيماء — متجر لحوم طازجة وذبائح

متجر إلكتروني عربي متجاوب بالكامل (RTL) لبيع اللحوم الطازجة والذبائح، مبني بـ **HTML + CSS + JavaScript** فقط، بدون أي إطار عمل أو خطوة بناء.

## ✨ المميزات

- تصميم عربي RTL بهوية نجدية (نقش السدو، خط Lalezar للعناوين وReadex Pro للنصوص)
- 12 منتجًا في 4 تصنيفات (نعيمي وحري، تيوس وماعز، عجول، لحوم مقطعة) مع فلترة فورية
- اختيار طريقة التقطيع لكل منتج
- سلة مشتريات كاملة: درج جانبي، تعديل الكميات، حساب الإجمالي تلقائيًا
- إتمام الطلب عبر واتساب برسالة تحوي تفاصيل الطلب
- متجاوب مع شاشات الجوال، وقائمة تنقل منسدلة
- دعم إمكانية الوصول: تباين الألوان، التنقل بلوحة المفاتيح، `prefers-reduced-motion`

## 📁 هيكل المشروع

```
marai-tayma/
├── index.html
├── assets/
│   ├── css/style.css
│   └── js/app.js
├── .nojekyll
├── .gitignore
├── LICENSE
└── README.md
```

## 🚀 التشغيل محليًا

افتح `index.html` مباشرة في المتصفح، أو شغّل خادمًا محليًا:

```bash
python3 -m http.server 8000
# أو
npx serve .
```

## 🌐 النشر على GitHub Pages

```bash
git init
git add .
git commit -m "Initial commit: مراعي تيماء store"
git branch -M main
git remote add origin https://github.com/USERNAME/marai-tayma.git
git push -u origin main
```

ثم من المستودع: **Settings ← Pages ← Source: Deploy from a branch ← Branch: `main` / `(root)` ← Save**

سيكون الموقع على: `https://USERNAME.github.io/marai-tayma/`

## ⚙️ التخصيص

| ماذا تعدّل | أين |
|---|---|
| رقم الواتساب | `assets/js/app.js` (زر إتمام الطلب) و`index.html` (التذييل) |
| المنتجات والأسعار | مصفوفة `PRODUCTS` في `assets/js/app.js` |
| ألوان الهوية | متغيرات `:root` أعلى `assets/css/style.css` |
| معلومات التواصل وأوقات العمل | قسم `<footer>` في `index.html` |

## 📄 الرخصة

MIT — انظر ملف [LICENSE](LICENSE).
